# simple-taiko-node + dashboard

Spin up the taiko node including the dashboard to monitor the node with these steps:

1. `git clone https://github.com/wolfderechter/taiko-node-dashboard-docker`
2. `cp .env.sample .env` and fill out `L1_ENDPOINT_HTTP` and `L1_ENDPOINT_WS`
3. `docker compose up`
4. visit localhost:8082 to access the dashboard

**Proposers and provers**

5. In the .env file make sure to change the `VITE_ENABLE_PROVER`, `VITE_ENABLE_PROPOSER` and `VITE_L1_PRIVATE_KEY` variables