# SurfGuard
An open source solution to supervise the web sites (or pages) one can aceess from home network

## Primary Components

1. In house proxy server (allow / deny access to particular site / page).
2. Dictionary of classified sites. Each known site have some tags which represent the groups that site belongs to.
3. A NLP (Natural Language Proccessing) system which have the ablity to categorize a web page based on it's content.
  That system have to add each categorized page to the dictionary above.
4. Home networking components like DHCP, and a package of script which can configure every router in the market so the whole network access to the internet will have to go via the proxy. So we can sure that only the proxy have direct access to the internet.
5. Management interface to manage all the above components.

### Current state
I will appreciate any help.
### Current tasks
1. Find an open source, free to use proxy server. The proxy must support filterring of sites or pages.
2. Find appropriate open source NLP system.
3. Build initial stock of categorized sites and pages.
4. Combine the NLP to appropriate dictionary. Probably it will stored on some cloud provider. In addition it will contain an expaired date to each tag of each page, so the information will remain relevant over time.
5. Connect the proxy filttering system and the dictionary.
6. Develop the management interface.
7. Find an open source DHCP server. It will repalce the default DHCP in the router so the devices whose connected to the the network have no need to connect to the router at all and they will get the proxy server as their default gateway. Only the proxy will have the router as default gateway. Actually, only the proxy will be connected directly to the router.
8. Write scripts to various routers. The router will configure so only the proxy server could be connected to the router. In addition, the default password of the router will be replaced by random password so one can access the router configurations just in case he have access to the management interface.
