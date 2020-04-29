# calico-demo
This repository contains all the yaml-files that are needed for our Calico policy demo.

To set up the demo: 

- Create a calico cluster with enabled network policies, there's a lot of different ways to do this. Choose what you like.
- Navigate to the folder with the yaml-files.
- `kubectl create -f 00-namespace.yaml`
- `kubectl create -f 01-management-ui.yaml`
- `kubectl create -f 02-backend.yaml`
- `kubectl create -f 03-frontend.yaml`
- `kubectl create -f 04-client.yaml`
- `watch kubectl get pods --all-namespaces` and wait until every pod is running

It should now be ready to go.
