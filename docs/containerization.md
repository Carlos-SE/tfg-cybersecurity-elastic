# Containerization vs Virtualization

Alternative to consider:
1. Docker/Docker-Compose
2. Vagrant

| Features | Docker | Vagrant |
|-----------------|--------|---------|
| Containerization | ✔️ | :x: |
| Virtualization | :x:| ✔️ |
| Orchestration | ✔️ | :x: |
| Network Management | ✔️ | ✔️ |
| Volume Management | ✔️ | ✔️ |
| Multiplatform | ✔️ | ✔️ |
| Load balancing | :x: | ✔️ |
| Graphical Interface | ✔️ | :x: |
| File sharing | ✔️ | ✔️ | 
| Monitoring tools | ✔️ |:x:| 

Translated with www.DeepL.com/Translator (free version)

These are solid alternatives to implement the environment. Vagrant is suited for large projects, and it can take longer to configure. However, the VMs that vagrant creates are replicable and portable due to the files Vagrant creates to deploy the VM.

Docker is best suited for lightweight jobs/services instead of a whole VM. Docker allows developers to deploy services in seconds with an easy configuration.

With these things in mind, we can consider running the Elastic Stack separately in different containers. The layers of the stack are lightweight, and running them on docker containers will allow the environment to develop freely because of the independence of the system.
