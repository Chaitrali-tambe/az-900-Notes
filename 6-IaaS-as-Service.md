::::::: Infrastructure as a Service (IaaS) in Azure :::::::

																      PaaS 
Responsibility             |--	Information and data                    ◼        		 
Always retained          --|    Devices (mobiles & PCs)                 ◼        
by customer		           |	Accounts and Identities                 ◼       		    
				           |--	Identity and directory infrastructure   ◩       		   
Responsibility             |	Applications                            ◩       		   
varies by type           --|	Network Controls                        ◩       		   
				           |--	Operating System                        ☐       		    
Responsibility transfers   |	Physical hosts                          ☐       		   
to cloud providers		   |	Physical network                        ☐       
						   |--	Physical Datacenter

IaaS provides on-demand access to fundamental computing resources like virtual machines (VMs), storage, and networking, serving as a virtualized version of a traditional datacenter.
▫ How it Works: You rent infrastructure from Azure. You are responsible for managing the operating system, middleware, runtime, applications, and data.
▫ Azure Examples: Azure Virtual Machines (VMs), Azure Virtual Network, Azure Disk Storage.
▫ Pros:
  ► Maximum Control: Full control over infrastructure, OS, and applications.
  ► Flexibility: Ideal for migrating legacy apps to the cloud without re-architecting.
  ► High Scalability: Easily scale resources up or down based on demand.
▫ Cons:
  ► High Management Overhead: You are responsible for patching, security, and maintenance.
  ► Complexity: Requires specialized IT expertise to manage.
