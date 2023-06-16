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
6. Fill in the node address in the settings

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

4. Fill in the node address in the settings

#### Notes

- If you are already running the node, you'll need to install one of the following extensions
    - [firefox extension](https://addons.mozilla.org/en-US/firefox/addon/cors-everywhere/)
    - [chrome extension](https://chrome.google.com/webstore/detail/cors-unblock/lfhmikememgdcahcdlaciloancbhjino)
    - Safari doesn't have an extension but you can do: Safari -> Preferences -> Advanced.
    At the bottom tick `Show Develop Menu` in menu bar, then in the Develop Menu tick `Disable Cross-Origin Restrictions`.
    - Or you can simply re-install using [this guide](https://github.com/wolfderechter/taiko-node-dashboard-docker#taiko-node--dashboard)
