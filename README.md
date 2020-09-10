# Jenkins k8s Plugin Test

## References
[this article](https://medium.com/vivid-seats-engineering/how-to-kubernetes-pods-as-jenkins-build-agents-a726d3886861)

[this documentation](https://github.com/jenkinsci/kubernetes-plugin#declarative-pipeline)


## Helm Install

~~~
helm search hub jenkins
helm repo add jenkinsci https://charts.jenkins.io
helm repo update
helm install test-jenkins jenkinsci/jenkins 
~~~

