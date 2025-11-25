# Kubernetes distros


|                                     |                         Minikube                                  |                           kind                                      |                                       k3d                                                   |                                   
|-------------------------------------|-------------------------------------------------------------------|---------------------------------------------------------------------|---------------------------------------------------------------------------------------
|     Intro                         | Minikube is a tool that creates a single-node Kubernetes cluster on your local machine for development and testing purposes.  | This is a command-line tool designed for running local Kubernetes clusters using Docker containers as "nodes.         | k3d is a lightweight tool designed to run K3s clusters within Docker containers.                                                  
|     Characteristics                   | Uses a VM or container to run a single-node cluster, though it now supports multi-node setups.               | Runs Kubernetes cluster nodes as Docker containers.        | A lightweight, single-binary Kubernetes distribution that can use SQLite as a data store for simplicity.                            
|     Pros and Cons                       | Pros: Simple installation, cross-platform support, and a rich feature set for learning.<br />Cons: Tends to be heavier on resources and can have slower startup times due to VM overhead.  | Pros: Very fast startup because it uses Docker containers for nodes, allowing for multi-node clusters.<br /> Cons: Not a full node-level simulation and is not ideal for testing production environments due to its container-based nature. | Pros: Extremely lightweight, fast to start, and production-ready.<br /> Cons: Has a more limited set of add-ons compared to Minikube. 

# Demo

![Image](.doc/demo.gif)


# Summary

Agree with Dev Team to use k3d distribution due to very fast startup and low resource usage