##  1. Running a Container

To run a container from an image:

```bash
docker run redis
```

This will download the **latest Redis image** (if not present) and run it.

If you want a **specific version**:

```bash
docker run redis:4.0
```

 Here, `4.0` is the version (tag).

---

##  2. Interactive Mode (STDIN)

By default, Docker containers run in **non-interactive mode**
 That means they **don’t accept input from keyboard**

### 🔹 Run in interactive mode:

```bash
docker run -i redis
```

 `-i` = keeps STDIN open (you can give input)

---

##  3. Terminal Access (Pseudo TTY)

If you want a proper terminal (like Linux shell):

```bash
docker run -it redis
```

 `-it` = interactive + terminal
 Now you get a **prompt inside the container**

---

##  4. Port Mapping

Containers run in isolation, so we map ports to access them from outside.

###  Example:

```bash
docker run -p 80:5000 redis
```

 Format:

```
host_port : container_port
```

 Access app via **host port (80)** → internally goes to **5000**

---

###  MySQL Example:

```bash
docker run -p 3306:3306 mysql
```

 Same port mapping for database access

---

 Note:

* One host port can be mapped to **only one container at a time**

---

## 💾 5. Volume Mapping (Data Persistence)

By default:
 If container is deleted → **data is lost**

###  To persist data:

```bash
docker run -v /opt/datadir:/var/lib/mysql mysql
```

 Format:

```
host_directory : container_directory
```

 Data will be saved in `/opt/datadir` even if container is removed

---

##  6. Inspect Container

To see detailed information about a container:

```bash
docker inspect redis
```

 Shows:

* IP address
* Config
* Volumes
* Network details

---

##  7. Container Logs

To check logs of a container:

```bash
docker logs redis
```

👉 Useful for:

* Debugging errors
* Checking application output
