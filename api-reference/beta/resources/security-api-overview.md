---
title: 使用 Microsoft Graph 安全性 API
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.localizationpriority: high
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 86a26afb9bba3421fa2ceaa8fbad035e2f47b6fa
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129265"
---
# <a name="use-the-microsoft-graph-security-api"></a>使用 Microsoft Graph 安全性 API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph 安全性 API 提供了统一的界面的架构，用于与 Microsoft 和生态系统合作伙伴的安全性解决方案集成。 这使客户能够简化安全性操作和更好地抵御日益增多的网络威胁。 Microsoft Graph 安全性 API 将查询与所有已上架的安全性提供商进行联接并生成相关响应。 使用 Microsoft Graph 安全性 API 构建具有以下优势的应用程序：

- 合并和关联多个来源的安全警报
- 解锁上下文数据，以提供信息帮助调查
- 自动处理安全任务、业务流程、工作流和报告
- 发送 Microsoft 产品威胁指示器供自定义检测
- 采取操作来应对新的威胁
- 直观显示安全数据，实现主动风险管理

Microsoft Graph 安全性 API 包括以下关键实体。

## <a name="actions-preview"></a>操作（预览版）

利用 Microsoft Graph 安全性 [securityAction](securityaction.md) 实体立即采取行动来抵御威胁。 当安全分析师发现新的指示器（如恶意文件、URL、域或 IP 地址）时，可立即在你的 Microsoft 安全解决方案中启用保护。 针对特定提供商采取操作，查看所采取的全部操作，还可在需要时取消操作。 尝试使用 [Microsoft Defender for Endpoint](/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) (以前是 Microsoft Defender ATP) 的安全操作，以使用警报中发现的属性或在调查期间识别的属性阻止 Windows 终结点上的恶意活动。

  > **注意：** 安全操作当前仅支持应用程序权限。

## <a name="alerts"></a>警报

警报是指 Microsoft 或其合作伙伴安全解决方案在客户的租户中识别并标记要进行操作或发送通知的潜在安全问题。 借助 Microsoft Graph 安全性[警报](alert.md)实体，你可对所有集成解决方案中的安全问题进行统一和简化。 此外，这还能使应用程序关联警报和上下文，从而提升威胁防护和响应。 利用警报更新功能，你可以更新[警报](alert.md)实体，从而同步与 Microsoft Graph 安全性 API 集成的不同安全产品和服务中的特定警报状态。

Microsoft Graph 安全性 API 提供来自以下提供商的警报。 下表显示了对 GET 警报、PATCH 警报和订阅（通过 webhooks）的支持。

| 安全提供商 | <p align="center">GET 警报</p>| <p align="center">PATCH 警报</p>| <p align="center">订阅订阅</p>|
|:------------------|:---------|:-----------|:------------------|
|[Azure 安全中心](/azure/security-center/security-center-alerts-type)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/playbook) | <p align="center">&#x2713;</p> | <p align="center">[提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
| [Microsoft Defender for Cloud Apps](/cloud-app-security/monitor-alerts) (以前是 Microsoft Cloud App Security)  | <p align="center">&#x2713;</p> | <p align="center">[提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|[Microsoft Defender for Endpoint](/windows/security/threat-protection/microsoft-defender-atp/attack-simulations) (以前是 Microsoft Defender ATP) **| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Microsoft Defender for Identity](/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories) (以前是 Azure 高级威胁防护) ***| <p align="center">&#x2713;</p> | <p align="center">[提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|Microsoft 365 <ul><li> [默认](/office365/securitycompliance/alert-policies#default-alert-policies)</li> <li>[Cloud App Security](/office365/securitycompliance/anomaly-detection-policies-in-ocas)</li><li>自定义警报</li></ul> | <p align="center">&#x2713;</p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Azure 信息保护](/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive)**（预览版）**| <p align="center">&#x2713;</p> | <p align="center">[提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|[Azure Sentinel](/azure/sentinel/quickstart-get-visibility)**（预览版）**| <p align="center">&#x2713;</p> | <p align="center">在 Azure Sentinel 中不受支持 </p> | <p align="center">&#x2713;</p> |
> **注意：** 新的提供商将会不断加入 Microsoft Graph 安全生态系统。 要请求新的提供商或从现有提供商处获取更长时间的支持，请[在 Microsoft Graph 安全性 GitHub 存储库中提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new)。

\* 文件问题：警报状态在 Microsoft Graph 安全性 API 集成应用程序中得到更新，但不反映在供应商的管理经验中。

\*\*与 Microsoft Graph 安全性 API 相比，Microsoft Defender for Endpoint 所需的[用户角色](/windows/security/threat-protection/microsoft-defender-atp/user-roles)更多。 只有同时具备 Microsoft Defender for Endpoint 和 Microsoft Graph 安全性 API 角色的用户才可访问 Microsoft Defender for Endpoint 数据。 由于仅限应用程序的身份验证不受此约束限制，我们建议使用仅限应用程序的身份验证令牌。

\*\*\* Microsoft Defender for Identity 警报通过 Microsoft Defender for Cloud Apps 集成提供。 这意味着只有在加入了 Unified SecOps 并将 Microsoft Defender for Identity 连接到 Microsoft Defender for Cloud Apps 时，才会收到 Microsoft Defender for Identity 警报。 了解有关[如何集成 Microsoft Defender for Identity 和 Microsoft Defender for Cloud Apps](/azure-advanced-threat-protection/atp-mcas-integration) 的详细信息。

## <a name="attack-simulation-and-training-preview"></a>攻击模拟和培训（预览版）

[攻击模拟和培训](/microsoft-365/security/office-365-security/attack-simulation-training)是 [Microsoft Defender for Office 365](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true) 的一部分。 此服务可让租户中的用户体验真实的恶意钓鱼攻击，并从中学习。 最终用户的社交工程模拟和培训体验有助于降低用户被这些攻击技术入侵的风险。 攻击模拟和培训 API 使租户管理员能够查看启动的[模拟](simulation.md)练习和培训，并获取有关网络钓鱼模拟中用户在线行为的派生见解的[报告](report-m365defender-reports-overview.md)。

## <a name="information-protection"></a>信息保护

**标签** - 信息保护标签提供有关如何正确地将敏感度标签应用到信息的详细信息。 信息保护标签 API 描述对某一用户或租户应用的敏感度标签配置。

**威胁评估** - Microsoft Graph 威胁评估 API 可帮助组织评估租户中任何用户收到的威胁。 这样，客户就可将其收到的垃圾电子邮件、网络钓鱼 URL 或恶意软件附件报告给 Microsoft。 策略检查结果和重新扫描结果可帮助租户管理员了解威胁扫描判定并调整其组织策略。

## <a name="secure-score"></a>安全功能分数

[Microsoft 安全功能分数](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358)是一款安全分析解决方案，可让你了解安全项目组合以及如何改进这些组合。 只需一个分数，你就可以更好地了解已采取了哪些措施来降低 Microsoft 解决方案中的风险。 此外，你还可以将你的分数与其他组织比较，以了解你的分数趋势。 Microsoft Graph 安全性 [secureScore](securescores.md) 和 [secureScoreControlProfile](securescorecontrolprofiles.md) 实体可以帮助你实现组织的安全性与生产力需求之间的平衡，同时支持相应的安全功能混合。 你也可以计划采取安全功能之后的分数。

## <a name="threat-intelligence-indicators-preview"></a>威胁情报指示器（预览版）

威胁指示器也称为泄露指示器 (IoC)，它们表示已知威胁的相关数据，例如恶意文件、URL、域和 IP 地址。 客户可通过内部威胁智能收集功能生成指示器，也可从威胁智能社区、经过许可的源或其他来源获取指示器。 这些指示器随后可在各种安全工具中用来防御相关威胁。

借助 Microsoft Graph 安全性 [tiIndicator](tiindicator.md) 实体，客户可向 Microsoft 安全解决方案提供威胁指示器，以便阻止（并发出警报）或允许恶意活动操作，这会遏制被判定为与某组织无关的指示器的操作。 发送指示器时，会指定要使用这些指示器的 Microsoft 解决方案以及要对指示器执行的操作。

你可将 [tiIndicator](tiindicator.md) 实体集成到应用程序中，或者使用下述集成威胁智能平台 (TIP) 之一：

- [Palo Alto 网络 MineMeld 威胁智能共享](https://www.paloaltonetworks.com/products/secure-the-network/subscriptions/minemeld)
- [MISP 开源威胁智能平台](http://www.misp-project.org/)（通过 [TI 示例](https://aka.ms/tipmispsample)提供）

现在可从以下产品获取通过 Microsoft Graph 安全性 API 发送的威胁指示器：

- [Azure Sentinel](/azure/sentinel/overview) – 可以将威胁指示器与日志数据关联在一起，获取恶意活动警报。
- [Microsoft Defender for Endpoint](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-advanced-threat-protection) – 使你能够针对与恶意活动关联的威胁指示器发出警报和/或进行阻止。 还可以允许指示器，以忽略此指示器，免于对其进行自动调查。 有关支持的指示器类型以及每个租户的指示器数限制的详细信息，请参阅[管理指示器](/windows/security/threat-protection/microsoft-defender-atp/manage-indicators)。

即将在其他 Microsoft 安全服务中提供支持。


## <a name="common-use-cases"></a>常见用例

以下是使用 Microsoft Graph 安全性 API 的一些热门的请求。

| **用例**   | **REST 资源** | **在 Graph 浏览器中试调用** |
|:---------------|:--------|:----------|
| **操作（预览版）**|||
| 获取安全操作 | [获取安全操作](../api/securityaction-get.md)|[https://graph.microsoft.com/beta/security/securityActions/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|列出安全操作| [列出安全操作](../api/securityactions-list.md)|[https://graph.microsoft.com/beta/security/securityActions](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|创建安全操作|[创建安全操作](../api/securityactions-post.md)|[https://graph.microsoft.com/beta/security/securityActions](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|取消安全操作|[取消安全操作](../api/securityaction-cancelsecurityaction.md)| [https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions/{id}/cancelSecurityAction&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
| **警告**|||
| 列出警报 | [List alerts](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| 更新警报 | [更新警报](../api/alert-update.md) </br> [更新多个警报](../api/alert-updatealerts.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) </br> [https://graph.microsoft.com/beta/security/alerts/updateAlerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/updateAlerts&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
| **攻击模拟和培训（预览版）**|||
|列出模拟|[列出模拟](../api/attacksimulationroot-list-simulations.md)|[https://graph.microsoft.com/beta/security/attackSimulation/simulations](https://developer.microsoft.com/graph/graph-explorer?request=security/attackSimulation/simulations&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|获取模拟概述报告|[获取模拟概述报告](../api/simulationreportoverview-get.md)|[https://graph.microsoft.com/beta/security/attackSimulation/simulations/{id}/report/overview](https://developer.microsoft.com/graph/graph-explorer?request=security/attackSimulation/simulations/{id}/report/overview&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|列出模拟用户报告|[列出模拟用户报告](../api/usersimulationdetails-list.md)|[https://graph.microsoft.com/beta/security/attackSimulation/simulations/{id}/report/simulationUsers](https://developer.microsoft.com/graph/graph-explorer?request=security/attackSimulation/simulations/{id}/report/simulationUsers&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
| **安全功能分数**|||
|列出安全功能分数|[列出 secureScores](../api/securescores-list.md)|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
| **安全功能分数控制配置文件**|||
|列出安全功能分数控制配置文件|[列出 secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|更新安全功能分数控制配置文件|[更新 secureScoreControlProfiles](../api/securescorecontrolprofiles-update.md)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|
| **威胁情报指示（预览版）**|||
|获取 TI 指示器|[获取 tiIndicator](../api/tiindicator-get.md)| [https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|列出 TI 指示器 | [列出 tiIndicator](../api/tiindicators-list.md) | [https://graph.microsoft.com/beta/security/tiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|创建 TI 指示器|[创建 tiIndicator](../api/tiindicators-post.md)|[https://graph.microsoft.com/beta/security/tiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|提交 TI 指示器|[提交 tiIndicator](../api/tiindicator-submittiindicators.md)| [https://graph.microsoft.com/beta/security/tiIndicators/submitTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/submitTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
|更新 TI 指示器|[更新 tiIndicator](../api/tiindicator-update.md) </br>[更新多个 tiIndicator](../api/tiindicator-updatetiindicators.md)| [https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) </br>[https://graph.microsoft.com/beta/security/tiIndicators/updateTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/updateTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|删除 TI 指示器|[删除 tiIndicator](../api/tiindicator-delete.md) </br>[删除多个 tiIndicator](../api/tiindicator-deletetiindicators.md) </br>[按 externalId 删除 tiIndicator](../api/tiindicator-deletetiindicatorsbyexternalid.md)| DELETE </br>[https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=DELETE&version=beta&GraphUrl=https://graph.microsoft.com) </br>POST</br>[https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/deleteTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)</br>POST</br>[https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/deleteTiIndicatorsByExternalId&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|

你可使用 Microsoft Graph [Webhook](/graph/webhooks) 来订阅和接收 Microsoft Graph 安全性 API 实体更新的相关通知。

## <a name="whats-new"></a>最近更新
了解这些 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="next-steps"></a>后续步骤

Microsoft Graph 安全性 API 可以为你提供使用 Microsoft 和合作伙伴的不同安全解决方案的新方式。请按照以下步骤操作开始使用：

- 深入了解[警报](alert.md)、[tiIndicator](tiindicator.md)（预览版）、[securityAction](securityaction.md)（预览版）、[secureScore](securescores.md) 和 [secureScoreControlProfiles](securescorecontrolprofiles.md)。
- 在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。 在“**示例查询**”中，选择“**显示更多示例**”并将“安全类别”设为“**开启**”。
- 请尝试[订阅和接收实体变更通知](/graph/webhooks)。

需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/partners)。

## <a name="see-also"></a>另请参阅

Microsoft Graph 安全性 API 示例的[代码和贡献情况](https://github.com/microsoftgraph/security-api-solutions/blob/master/CONTRIBUTING.md)：

- [ASP.NET (C#) 示例](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python 示例](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript) 示例](https://github.com/microsoftgraph/nodejs-security-sample)
- [PowerShell 示例](https://aka.ms/graphsecuritypowershellsample)
- [其他示例或贡献新的示例](https://aka.ms/graphsecurityapicode)

了解可与 Microsoft Graph 安全性 API 连接的其他选项：

- [适用于 Logic Apps、Flow 和 PowerApps 的 Microsoft Graph 安全性连接器](/azure/connectors/connectors-integrate-security-operations-create-api-microsoft-graph-security)
- [Jupyter Notebook 示例](https://aka.ms/graphsecurityjupyternotebooks)

与社区互动：

- [加入技术社区](https://techcommunity.microsoft.com/t5/microsoft-graph-security-api/bd-p/SecurityGraphAPI)
- [在 StackOverflow 上讨论](https://stackoverflow.com/questions/tagged/microsoft-graph-security)