# Accelerator Log

## Options
```json
{
  "deploymentType" : "kontinue",
  "projectName" : "hello-kontinue"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Combo, UniquePath)
┃ ┏ engine.transformations[0] (Combo)
┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ engine.transformations[0].merge (Chain)
┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┏ engine.transformations[0].merge.transformations[0] (Merge)
┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude)
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/skaffold.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/DEPLOYING.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/service.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/skaffold.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/kontinue/DEPLOYING.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/kontinue/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃  Info Will exclude [README.md, kubernetes/**]
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md, kubernetes/**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [README.md, kubernetes/**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [README.md, kubernetes/**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md, kubernetes/**] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md, kubernetes/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md matched [README.md, kubernetes/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile matched [README.md, kubernetes/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml matched [README.md, kubernetes/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml matched [README.md, kubernetes/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/skaffold.yaml matched [README.md, kubernetes/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/DEPLOYING.md matched [README.md, kubernetes/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/service.yaml matched [README.md, kubernetes/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/skaffold.yaml matched [README.md, kubernetes/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/kontinue/DEPLOYING.md matched [README.md, kubernetes/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/kontinue/workload.yaml matched [README.md, kubernetes/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md, kubernetes/**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md, kubernetes/**] -> included
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md, kubernetes/**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [README.md, kubernetes/**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md, kubernetes/**] -> included
┃ ┃ ┃ ┗ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [README.md, kubernetes/**] -> included
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/skaffold.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/DEPLOYING.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/service.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/skaffold.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/kontinue/DEPLOYING.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/kontinue/workload.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [hello-fun->hello-kontinue]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'k8s-simple') evaluated to false
┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'k8s-simple') evaluated to false
┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'knative') evaluated to false
┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[5] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'knative') evaluated to false
┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[6] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'kontinue') evaluated to true
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[6].<combo> (Chain)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'kontinue') evaluated to true
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[6].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [kubernetes/kontinue/workload.yaml]
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/skaffold.yaml didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/DEPLOYING.md didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/service.yaml didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/skaffold.yaml didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/kontinue/DEPLOYING.md didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/kontinue/workload.yaml matched [kubernetes/kontinue/workload.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [kubernetes/kontinue/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[6].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, ReplaceText, ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[6].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [: hello-fun->: hello-kontinue]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[6].<combo>.transformations[1].transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [https://github.com/sample-accelerators/hello-fun.git->https://github.com/sample-accelerators/hello-fun.git]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[6].<combo>.transformations[1].transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [branch: main->branch: main]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[6].<combo>.transformations[1].transformations[3] (RewritePath)
┃ ┃ ┃ ┗ ┗ ┗ Debug Path 'kubernetes/kontinue/workload.yaml' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.yaml, folder=kubernetes/kontinue/, filename=workload.yaml, g0=kubernetes/kontinue/workload.yaml, g1=kubernetes/kontinue/, g2=workload.yaml, g3=workload.yaml, g4=.yaml} and was rewritten to 'kubernetes/workload.yaml'
┃ ┃ ┃ ┏ README (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(Append))
┃ ┃ ┃ ┃ README.merge (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┏ README.merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ ┃ ┃ README.merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/skaffold.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/DEPLOYING.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/service.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/skaffold.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/kontinue/DEPLOYING.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/kontinue/workload.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [hello-fun template repo->hello-kontinue]
┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'k8s-simple') evaluated to false
┃ ┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'knative') evaluated to false
┃ ┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'kontinue') evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ ┃ ┃ README.merge.transformations[0].sources[3].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'kontinue') evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[3].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [kubernetes/kontinue/DEPLOYING.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/MavenWrapperDownloader.java didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/skaffold.yaml didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/DEPLOYING.md didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/service.yaml didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/knative/skaffold.yaml didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/kontinue/DEPLOYING.md matched [kubernetes/kontinue/DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/kontinue/workload.yaml didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [kubernetes/kontinue/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[3].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[3].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [hello-fun->hello-kontinue]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[3].<combo>.transformations[1].transformations[1] (RewritePath)
┃ ┃ ┃ ┃ ┗ ┗ ┗ ┗ Debug Path 'kubernetes/kontinue/DEPLOYING.md' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.md, folder=kubernetes/kontinue/, filename=DEPLOYING.md, g0=kubernetes/kontinue/DEPLOYING.md, g1=kubernetes/kontinue/, g2=DEPLOYING.md, g3=DEPLOYING.md, g4=.md} and was rewritten to 'README.md'
┃ ┃ ┃ ┃ ┏ README.merge.transformations[1] (UniquePath)
┃ ┃ ┗ ┗ ┗ Debug Multiple representations for path 'README.md', will concatenate them together
┃ ┃ ┏ engine.transformations[0].merge.transformations[1] (UniquePath)
┃ ┗ ┗ Debug Multiple representations for path 'pom.xml', will use the one appearing last 
┗ ╺ engine.transformations[1] (UniquePath)
```
