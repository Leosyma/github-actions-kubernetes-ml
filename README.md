# Training and image validation with GitHub Actions

The training script produces versioned quality models. Changes to paths listed in the workflow trigger training, an image build and Kubernetes manifest validation. Run the deployment locally in Minikube.

## Run locally

```sh
minikube image build -t dsa-p6-app:latest .
kubectl apply -f k8s/
minikube service dsa-p6-app-service
```
