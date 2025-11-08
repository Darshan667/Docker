# Docker
### 1. What is Docker
* A container is a lightweight, standalone package that includes an application and all dependencies(libraries, binaries and configuration files).
* Unlike virtual machines, containers don't include a full operating system - they share the host OS kernel.
* This makes the container faster, smaller and more efficient.

### Difference between Hypervisor and Container
| Feature            | Virtual Machine (VM)                           | Container                                   |
| ------------------ | ---------------------------------------------- | ------------------------------------------- |
| **OS**             | Has its own full Guest OS                      | Shares host OS kernel                       |
| **Size**           | ~1–2 GB (due to full OS)                       | ~100–500 MB                                 |
| **Startup Time**   | Minutes                                        | Seconds                                     |
| **Resource Usage** | Heavy (each VM runs a full OS)                 | Lightweight                                 |
| **Technology**     | Uses **Hypervisor** (e.g., VMware, VirtualBox) | Uses **Docker Engine** or container runtime |

### Architecture of Docker
+---------------------------------------------------+
|                   Docker CLI / API                |
+---------------------------------------------------+
|                  Docker Engine                    |
|   - Docker Daemon (dockerd)                       |
|   - REST API                                      |
|   - Container Runtime (containerd / runc)         |
+---------------------------------------------------+
|              Host Operating System (Linux/Windows)|
+---------------------------------------------------+
|                   Hardware                        |
+---------------------------------------------------+

### Components
* Docker CLI -> you give a command.
* Docker Engine -> Core part that builds and runs the containers.
* Docker Daemon -> Manages images, containers, network and volume.
* Container Runtime -> Actually runs the container process.

  
| Term          | Description                                                                    |
| ------------- | ------------------------------------------------------------------------------ |
| **Image**     | A read-only template with app and environment configuration (like a blueprint) |
| **Container** | A running instance of an image (like a live process)                           |

### Docker Life Cycle:
Dockerfile -> Image -> Container -> Stop/Remove

<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/e8144372-be49-4f9c-acd1-5813e104444e" />


