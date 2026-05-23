# Cloud Benefits

## High Availability (HA) - _"Always On"_:
**Simple Idea:** Preventing downtime. If one part of your app breaks, another takes over.
Azure Tools:
<dl>
	<dd>▫ <strong>Availability Zones:</strong> Spreading apps across physically separate, data centers within a region.</dd>
	<dd>▫ <strong>Fault Domains:</strong> Ensuring VMs are on different racks (power/network) to avoid simultaneous failure.</dd>
	<dd>▫ <strong>Load Balancers:</strong> Spreading traffic across healthy servers. </dd>
</dl>


## Scalability - _"Always Just Right"_:
**Simple Idea:** Handling growth. Adding more power (scale up) or more servers (scale out) when busy.
<dl>
**Types:**
	<dd>▸ <strong>Vertical Scaling _(Scale Up/Down)_:</strong> Increasing the size of a single instance, such as moving from 4GB RAM to 16GB RAM.</dd>
	<dd>▸ <strong>Horizontal Scaling _(Scale Out/In)_:</strong> Increasing or decreasing the number of instances (VMs), such as going from 2 servers to 5.</dd>
</dl>
<dl>
Azure Tools:
	<dd>▫ <strong>Virtual Machine Scale Sets:</strong> Automatically adding/removing virtual machines based on demand.</dd>
	<dd>▫ <strong>App Service Auto-scaling:</strong> Adjusting web app resources automatically.</dd>
</dl>


## Reliability - _"Keeping it Running"_:
Reliability in Azure means your applications stay running even if servers fail, using backups and global data centers to prevent downtime
<dl>
	<dd>▫ <strong>Azure Availability Zones:</strong> Physically separate datacenters within a region; if one fails, your apps failover to another.</dd>
	<dd>▫ <strong>Azure Regions:</strong> Deploying across multiple geographical areas to ensure global availability.</dd>
	<dd>▫ <strong>Azure Site Recovery:</strong> A disaster recovery service that keeps apps working during outages.</dd>
	<dd>▫ <strong>Azure Chaos Studio:</strong> A tool to intentionally induce failures to test and improve application resilience. </dd>
	
</dl>


## Predictability - _"Knowing What Will Happen"_:
Predictability means you can forecast costs and performance, using tools to manage, monitor, and scale resources automatically, so you know exactly what to expect
<dl>
	<dd>▫ <strong>Azure Advisor:</strong> Provides recommendations to optimize resources for better performance and lower costs.</dd>
	<dd>▫ <strong>Azure Cost Management + Billing:</strong> Tools to monitor, allocate, and forecast your cloud spend.</dd>
	<dd>▫ <strong>Azure Virtual Machines (SKUs):</strong> Standardized, well-defined machine sizes that guarantee specific performance levels (CPU, memory, storage).</dd>
	<dd>▫ <strong>Azure Load Balancer & Autoscale:</strong> Automatically distributes traffic and adjusts resources to maintain consistent performance, even during high traffic.</dd>
</dl>


## Security:
Security is about protecting data and resources from threats.
<dl>
	<dd>▫ <strong>Microsoft Entra ID (Formerly Azure Active Directory):</strong> The identity security guard.
  eg. Requires Multi-Factor Authentication (MFA) before allowing users to log in to the Azure Portal, stopping stolen passwords.</dd>
	<dd>▫ <strong>Microsoft Defender for Cloud:</strong> A security monitor that gives you a "score" and tells you how to fix risks.
  eg. It scans your Virtual Machines (servers) and alerts you if they are not properly patched or are open to the public internet.</dd>
	<dd>▫ <strong>Azure Firewall:</strong> A digital security guard at the perimeter of your network.
  eg. Blocks all incoming traffic from specific countries and only allows traffic from trusted IP addresses to reach your servers.</dd>
	<dd>▫ <strong>Azure NSG (Network Security Group):</strong> A firewall for a single, specific resource (like a VM).
  eg. You create a rule to only allow port 443 (HTTPS) traffic into your web server and block everything else.</dd>
</dl>


## Governance:
Governance is about setting rules to ensure everyone follows company standards (e.g., only using certain regions to save costs or comply with laws).
<dl>
	<dd>▫ <strong>Azure Management Groups:</strong> Folders to organize multiple subscriptions.
  eg. Grouping all "Production" subscriptions under one Management Group, and all "Testing" under another, to apply different policies to each.</dd>
	<dd>▫ <strong>Azure Role-Based Access Control (RBAC):</strong> A tool to assign permissions based on job roles (Least Privilege).
  eg. Giving a developer "Contributor" access to a specific project folder, but only "Reader" access to the production database.</dd>
</dl>






 







