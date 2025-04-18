---
title: Tenant Isolation1
date: 2025-01-14
tags: ["hugo","blog"]
image : "/img/posts/copilotfeature.png"
Description  : "In 2025, Microsoft Copilot Studio is introducing several new features to enhance the creation and management of autonomous AI agents. These updates include the ability to build agents that respond to events and complete workflows in the background, improving efficiency and automation. These features aim to simplify the creation, deployment, and management of AI agents, boosting productivity and collaboration."
featured: true
---

Configuring Copilot settings optimizes governance, security, and operational efficiency across your organization. This article provides an overview of key configuration settings at the tenant, environment, and agent levels. Settings are categorized based on their purpose and location (Azure PowerShell, Power Platform admin center or PPAC, or Copilot Studio), along with the required privileges for making changes.

Tenant-level settings


<!--{{<table "table table-striped table-bordered">}}		
Setting	Purpose	Location Privilege
Trial	License Control	Block
{{</table>}}	-->	

			
 	 free trial sign-ups without admin permission	Azure PowerShell	Azure PowerShell admin
Control agents with AI Features	Block generative AI usage in Copilot agents	PPAC > Settings	Power Platform admin
Copilot Studio authors control	Restrict Copilot Studio usage to a security group	PPAC > Settings	Power Platform admin
Set up environment routing	Route makers to specific environment groups	PPAC > Settings	Power Platform admin
AI Builder credits control	Decide if tenant-level AI credits can be used by environments	PPAC > Settings	Power Platform admin
Copilot data collection	Enable or block sharing prompts/requests with Microsoft	PPAC > Settings	Power Platform admin
Copilot feedback control	Enable or block feedback to Microsoft	PPAC > Settings	Power Platform admin
Tenant or environment-level settings (via DLP policies or capacity)
Setting [Name]	Purpose	Location	Privilege
Message capacity	Allocate Copilot message capacity to each environment	PPAC > Capacity	Power Platform admin
Telemetry logging / AppInsights control
[Application insights in Copilot Studio]	Block agent makers from connecting to Application Insights	PPAC > DLP Policies	Power Platform admin
Authentication control
[Chat without Microsoft Entra ID authentication in Copilot]	Disable "No-Auth" and "Generic OAuth" as Copilot auth providers	PPAC > DLP Policies	Power Platform admin
Channel control
[Microsoft Teams + Microsoft 365 Channel in Copilot Studio]
[Direct Line Channels in Copilot Studio]
[Facebook Channel in Copilot Studio]
[OmniChannel in Copilot Studio]	Block channels (Microsoft Teams, Direct line, Facebook, Microsoft 365, OmniChannel)	PPAC > DLP Policies	Power Platform admin
Knowledge source control
[Knowledge source with SharePoint and OneDrive in Copilot Studio]
[Knowledge source with Public website and data in Copilot Studio]
[Knowledge source with documents in Copilot Studio]	Block SharePoint, OneDrive, documents, or public websites to be used as a knowledge source in agents	PPAC > DLP Policies	Power Platform admin
Skills control
[Skills with Copilot Studio]	Block Copilot makers from using skills in Copilot Studio	PPAC > DLP Policies	Power Platform admin
HTTP requests control
[HTTP]	Prevent HTTP requests to reduce data exfiltration risk	PPAC > DLP Policies	Power Platform admin
Event triggers control (Autonomous)
[Microsoft Copilot Studio]	Block autonomous/event-driven agent triggers	PPAC > DLP Policies	Power Platform admin
Environment-level settings
Setting	Purpose	Location	Privilege
Generative AI control (Bing search)	Allow or block Bing search in Copilot agents	PPAC > Environment > Generative AI features	Environment admin
AI prompts control	Enable or block AI prompts in Power Platform	PPAC > Environment > Features	Environment admin
Copilot in Power Apps	Enable or block Copilot in Power Apps	PPAC > Environment > Features	Environment admin
Block solutions w/ Unmanaged Custom.	Prevent importing unmanaged customizations	PPAC > Environment > Features	Environment admin
Sharing agents (editor/viewer)	Manage if agents can be shared with editor or viewer roles	PPAC > Environment groups (Managed Environments)	Environment admin
Environment auditing	Enable auditing in production environments	PPAC > Environment settings > Auditing	Environment admin
Maker welcome message	Display privacy/compliance message to makers	PPAC > Environment groups (Managed Environment)	Power Platform Admin
Agent-level settings (in Copilot Studio)
Setting	Purpose	Location	Privilege
Agent authentication	Configure (no auth, Microsoft Entra ID, certificates)	Copilot Studio > Your agent > Settings > Security > Auth	Agent author
Agent web channel security	Manage secrets/tokens for Direct Line web channel	Copilot Studio > Your agent > Settings > Security > Auth	Agent author
