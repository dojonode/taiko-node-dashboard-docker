# Taiko node dashboard using docker

### Taiko node + dashboard

Quickly get started and spin up the taiko node + dashboard to monitor the node with these steps:

1. `git clone https://github.com/wolfderechter/taiko-node-dashboard-docker`
2. `cd taiko-node-dashboard-docker`
3. `cp .env.sample .env` and fill out `L1_ENDPOINT_HTTP` and `L1_ENDPOINT_WS`
4. `docker compose up`
5. visit localhost:7744 to access the dashboard

**Proposers and provers**

5. In the .env file make sure to change the `VITE_ENABLE_PROVER` and `VITE_ENABLE_PROPOSER` variables
6. Fill in the ethereum address(es) used for the node in the settings to view all the metrics

<br/>

---

<br/>

### Dashboard only

If you are already running the node and want to only spin up the taiko node dashboard follow these steps:

1. `git clone --single-branch --branch dashboard-only https://github.com/wolfderechter/taiko-node-dashboard-docker`
2. `cd taiko-node-dashboard-docker`
3. `docker compose up`
4. visit localhost:7744 to access the dashboard

**Provers and proposers**

4. Fill in the ethereum address(es) used for the node in the settings to view all the metrics
