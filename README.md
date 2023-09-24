# Taiko node dashboard using docker
![Docker Pulls](https://img.shields.io/docker/pulls/wolfderechter/taiko-node-dashboard)

This repository is a dockerized version of the [taiko-node-dashboard](https://github.com/wolfderechter/taiko-node-dashboard).

![Cover_Image](https://github.com/wolfderechter/taiko-node-dashboard/assets/60930264/8a18073f-848c-421f-9e81-4aae5482737e)

### Dashboard only

If you are already running the node and want to only spin up the taiko node dashboard follow these steps:

1. `git clone https://github.com/wolfderechter/taiko-node-dashboard-docker`
2. `cd taiko-node-dashboard-docker`
3. `docker compose up`
4. visit http://localhost:7744 to access the dashboard
5. *_⚠️ NOTE:_*  you might need to change the IP address in the connections (📡 button) to the IP address of your VPS.

**Provers and proposers**

6. Fill in the ethereum address(es) used for the node in the settings (⚙️ button) to view all the metrics

### Integrate the dashboard into the node

Append the following code snippet to the `docker-compose.yml` of the taiko node to combine the two applications.

   ```docker-compose
  taiko-node-dashboard:
     image: wolfderechter/taiko-node-dashboard:latest
     ports:
       - "7744:80"
  taiko-node-systeminfo:
     image: wolfderechter/taiko-node-systeminfo:latest
     ports:
       - "3009:3009"
   ```
