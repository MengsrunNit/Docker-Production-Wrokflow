# Docker

## Development Dockerfile (Dockerfile.dev)

**Purpose:**  
Make development easy and convenient for developers.

**Typical Characteristics:**
- Includes all dependencies 
- Supports live reload/debugging
- Simpler build process 
- May count local files as volumes 
- Larger image size is acceptable

## Development Dockerfile (Dockerfile.dev)

**Purpose:**  

**Typical Characteristics:**
- Samller image 
- Only production dependencies 
- Optimized builds 
- Optimized builds
- Often use multi-stage builds 
- No development tool use



Containers are designed to be **ephemeral (temporary)**. This means that when a container stops or is removed, any data stored inside the container is lost. Docker volumes solve this problem by storing data in a location managed by Docker on the host machine.

You can think of a Docker volume as **persistent storage managed by Docker**.

### Why use Docker volumes?

- Persist data even when containers are removed
- Share data between multiple containers
- Separate application data from container lifecycle
- Improve performance compared to writing directly inside the container

### Example

```bash
docker volume create my_volume
