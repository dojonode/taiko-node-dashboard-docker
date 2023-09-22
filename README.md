# Taiko node dashboard using docker

> *_⚠️ NOTE:_*  currently only supports L2 nodes


### Dashboard only

If you are already running the node and want to only spin up the taiko node dashboard follow these steps:

1. `git clone --single-branch --branch dashboard-only https://github.com/wolfderechter/taiko-node-dashboard-docker`
2. `cd taiko-node-dashboard-docker`
3. `docker compose up`
4. visit http://localhost:7744 to access the dashboard
5.  *_⚠️ NOTE:_*  you might need to change the IP address in the connections (📡 button) to the IP address of your VPS.


**Provers and proposers**

6. Fill in the ethereum address(es) used for the node in the settings (⚙️ button) to view all the metrics
