## Docker Overview - Zabbix

This dashboard enabled the use of zabbix as a datasource for Docker metrics, in order to use this data source you will need to install the [Zabbix plugin for Grafana](https://grafana.com/grafana/plugins/alexanderzobnin-zabbix-app)

This dashboard is also available to download directly from the Grafana dashboard repository [Here](https://grafana.com/grafana/dashboards/13028).

Or by inporting the following ID ``13028``

![enter image description here](https://user-images.githubusercontent.com/26186145/93467113-347c9300-f8e5-11ea-88ad-9e8b67b7a2cf.png)

> As of 17/09/2020 the instructions on the plugin page did not work for me on the latest version of Grafana, so replace the provived command to install with `sudo grafana-cli plugins install alexanderzobnin-zabbix-app 3.12.4`

In order to tweak this to your needs I would advise you to change the group and host variables, replace the value `/Zabbix servers/` with the Zabbix Group that your docker host resided in.


![](https://user-images.githubusercontent.com/26186145/93467237-655cc800-f8e5-11ea-948c-72033dc25372.png)Following this you will likely also need to change the host variable, in this change the value `/Zabbix server/`with the host name of your docker host.


![enter image description here](https://user-images.githubusercontent.com/26186145/93467453-aa80fa00-f8e5-11ea-85d2-5d28489b08f7.png)



