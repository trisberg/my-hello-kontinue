# hello-kontinue

This repo provides a simple Hello web app based on Spring Boot and Spring Cloud Function.

It can be deployed as a standalone web app, as a Kubernetes Deployment and Service, or as a Knative Service.

## The code

> **NOTE**: The project is configured for Java 11, if you are using Java 8, then modify the `java.version` property in `pom.xml`.

The project contains the following code layout:

```text
.
├── README.md
├── mvnw
├── mvnw.cmd
├── pom.xml
└── src
    ├── main
    │   ├── java
    │   │   └── com
    │   │       └── example
    │   │           └── helloapp
    │   │               └── HelloAppApplication.java
    │   └── resources
    │       └── application.properties
    └── test
        └── java
            └── com
                └── example
                    └── helloapp
                        └── HelloAppApplicationTests.java
```

It also contains some deployment manifests, depending on the deploymentType selected when generating the project.

You can modify the source code using [Visual Studio Code](https://code.visualstudio.com/):

```bash
code .
```

The Function that is used by this app is located at `src/main/java/com/example/helloapp/HelloAppApplication.java`

You can build the project using the provided Maven wrapper:

```bash
./mvnw clean package
```

## Standalone app with embedded Tomcat server

To run the app using the embedded Tomcat server you can run this command:

```bash
./mvnw spring-boot:run
```

You can access the function using `curl`:

```bash
curl -w'\n' -H 'Content-Type: text/plain' localhost:8080 -d "Fun"
```
## Deploying to Kubernetes as a Kontinue Workload

You need to have Kontinue and Cloud Native Runtimes installed on your cluster.

### Deploying to local cluster using Kubectl

To build and deploy the app run:

```
kubectl apply -f ./kubernetes/workload.yaml
```

To uninstall the app run:

```
kubectl delete -f ./kubernetes/workload.yaml
```


### Accessing the app deployed to local cluster

If you don't have `curl` installed it can be installed using downloads here: https://curl.se/download.html

You need to look up the Ingress endpoint for the Knative Serving install. See the [Install a networking layer](https://knative.dev/docs/install/install-serving-with-yaml/#install-a-networking-layer) and [Configure DNS](https://knative.dev/docs/install/install-serving-with-yaml/#configure-dns) sections for instructions for the different netwoking layers.

For _Kourier_ we can simply run the following port-forward command:

```
kubectl port-forward --namespace kourier-system service/kourier 8080:80
```

For _Contour_ we can simply run the following port-forward command:

```
kubectl port-forward --namespace contour-external service/envoy 8080:80
```

To invoke the deployed function run the following `curl` command in another terminal window:

```
curl localhost:8080 -w'\n' -H 'Content-Type: text/plain' -H 'Host: hello-kontinue.default.example.com' -d Fun
```
