# [Dashy Dashboard](https://github.com/Lissy93/dashy) LXC Installer Scripts

- Install Dashy automatically
- Removes the need to use Docker
- Builds directly from source
- Uses the same resources as Docker (Alpine)

### Container Requirements:
- LXC Container (Script Does NOT support Proxmox VMs yet)
- 4096mb of memory needed for build -> deflate to 512mb after script
- 2 virtual cores needed for build -> deflate to 1 after script

# Install On Alpine (recommended)

### Tested Alpine LXC Templates:
|    LXC Template     | Support |
| ------------------- | ------- |
| alpine-3.14-default | ❌     |
| alpine-3.15-default | ✅     |
| alpine-3.16-default | ✅     |
| alpine-3.17-default | ❌     |
| alpine-3.19-default | ❌     |


### Oneliner:

```
wget https://raw.githubusercontent.com/rokdd/DashyDashboardForLXC/main/Alpine%20Scripts/install-dashy-alpine3.19.sh && chmod +x install-dashy-alpine3.19.sh && ./install-dashy-alpine3.19.sh
```

The Alpine installer is highly recommended due to the incredibly low resource usage. After install you can expect to see this container use less than 75-100MB of memory. This is the same you would expect to use if you ran Dashy in docker. 

