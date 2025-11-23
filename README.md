Kubernetes Assessment

This is a simple Kubernetes project to run a demo app locally using Minikube and Docker.

Prerequisites

You need the following installed:

Ubuntu or any Linux system

Docker

Minikube

kubectl

Setup

Start Docker service on your system.

Delete any old Minikube cluster if it exists, and start a new Minikube cluster with Docker driver. Allocate 4 CPUs and 4GB of memory.

Configure your terminal to use Minikube’s Docker environment.

Build and Run App

Build the Docker image for your app from the app folder.

Deploy the app to Kubernetes using the deployment and service YAML files.

Check if your pods are running.

Open the app in your browser through Minikube service.

Useful Commands (Explained)

To delete Minikube cluster, run minikube delete.

To restart your deployment after updating the image, use kubectl rollout restart deployment followed by your deployment name.

To view logs of a pod, use kubectl logs followed by the pod name.

To open a shell inside a pod, use kubectl exec followed by the pod name and -- /bin/sh.

Tips

Add the Minikube Docker environment setup to your .bashrc to avoid retyping every time.

If Minikube fails to start, clean Docker by removing unused containers, images, and volumes, and restart Docker service.
