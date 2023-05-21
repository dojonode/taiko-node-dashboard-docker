# simple-taiko-node + dashboard

Spin up a taiko node alongside the node dashboard to monitor the node with these steps:

1. `git clone https://github.com/wolfderechter/taiko-node-dashboard-docker`
2. `cp .env.sample .env` and fill out `L1_ENDPOINT_HTTP` and `L1_ENDPOINT_WS`
3. `docker compose up`
4. visit localhost:8082 to see the dashboard
