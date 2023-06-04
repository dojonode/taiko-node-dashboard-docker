# simple-taiko-node + dashboard

Quickly get started and spin up the taiko node + dashboard to monitor the node with these steps:

1. `git clone https://github.com/wolfderechter/taiko-node-dashboard-docker`
2. `cp .env.sample .env` and fill out `L1_ENDPOINT_HTTP` and `L1_ENDPOINT_WS`
3. `docker compose up`
4. visit localhost:8082 to access the dashboard

**Proposers and provers**

1. In the .env file make sure to change the `VITE_ENABLE_PROVER`, `VITE_ENABLE_PROPOSER` and `VITE_L1_PRIVATE_KEY` variables

### Dashboard only

If you are already running the node and want to only spin up the taiko node dashboard follow these steps:

1. `git clone --single-branch --branch dashboard-only https://github.com/wolfderechter/taiko-node-dashboard-docker`
2. `docker compose up`
3. visit localhost:8082 to access the dashboard

**Provers and proposers**

4. Set the node address in the settings
