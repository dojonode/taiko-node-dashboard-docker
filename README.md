# taiko node dashboard

Spin up the taiko node dashboard to monitor the node with these steps:

1. `git clone --single-branch --branch dashboard-only https://github.com/wolfderechter/taiko-node-dashboard-docker`
2. `docker compose up`
3. visit localhost:7744 to access the dashboard

**Provers and proposers**

4. Fill in the node address in the settings

#### Notes

- If you are already running the node, you'll need to install one of the following
    - [firefox extension](https://addons.mozilla.org/en-US/firefox/addon/cors-everywhere/)
    - [chrome extension](https://chrome.google.com/webstore/detail/cors-unblock/lfhmikememgdcahcdlaciloancbhjino)
    - Safari doesn't have an extension but you can do: Safari -> Preferences -> Advanced.
    At the bottom tick `Show Develop Menu` in menu bar, then in the Develop Menu tick `Disable Cross-Origin Restrictions`.
    - Or you can simply re-install using [this guide](https://github.com/wolfderechter/taiko-node-dashboard-docker#taiko-node--dashboard)
