# Bansira_DevOpsHelm
**Kubernetes Deployment:**
Step 1: Generate a Kubernetes Helm Chart

Navigate to the Helm directory: cd Bansira_DevOpsHelm

Formulate a chart in the directory node-hello for working with Helm: helm create node-hello-chart

Modify the Helm templates to suit your application:
Update this template “deployment.yaml” with values from “values.yaml”.

Produce and package the chart:
helm package node-hello-chart


Step 2: Deploy The Helm Chart Via ArgoCD

helm push node-hello-0.1.1.tgz oci://registry-1.docker.io/ayushi0316
Apply the ArgoCD application manifests: kubectl apply -f ArgoCD_node-hello.yaml
