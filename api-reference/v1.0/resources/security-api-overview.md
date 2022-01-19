---
title: 使用 Microsoft Graph 安全性 API
description: Microsoft Graph 安全性 API 提供了统一的界面的架构，用于与 Microsoft 和生态系统合作伙伴的安全性解决方案集成。
ms.localizationpriority: high
author: preetikr
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 47dccb5f8c4bf71ce5814b8f50d7ed2625f7ca01
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072647"
---
# <a name="use-the-microsoft-graph-security-api"></a>使用 Microsoft Graph 安全性 API

Microsoft Graph 安全性 API 提供了统一的界面的架构，用于与 Microsoft 和生态系统合作伙伴的安全性解决方案集成。 这使客户能够简化安全性操作和更好地抵御日益增多的网络威胁。 Microsoft Graph 安全性 API 将查询与所有已上架的安全性提供商进行联接并生成相关响应。 使用 Microsoft Graph 安全性 API 构建具有以下优势的应用程序：

- 合并和关联多个来源的安全警报
- 解锁上下文数据，以提供信息帮助调查
- 自动处理安全任务、业务流程、工作流和报告
- 发送 Microsoft 产品威胁指示器供自定义检测
- 采取操作来应对新的威胁
- 直观显示安全数据，实现主动风险管理

Microsoft Graph 安全性 API 包括以下关键实体。

## <a name="alerts"></a>警报

警报是指 Microsoft 或其合作伙伴安全解决方案在客户的租户中识别并标记要进行操作或发送通知的潜在安全问题。 借助 Microsoft Graph 安全性[警报](alert.md)实体，你可对所有集成解决方案中的安全问题进行统一和简化。 此外，这还能使应用程序关联警报和上下文，从而提升威胁防护和响应。 利用警报更新功能，你可以更新[警报](alert.md)实体，从而同步与 Microsoft Graph 安全性 API 集成的不同安全产品和服务中的特定警报状态。

Microsoft Graph 安全性 API 提供来自以下提供商的警报。 下表显示了对 GET 警报、PATCH 警报和订阅（通过 webhooks）的支持。

| 安全提供商 | <p align="center">GET 警报</p>| <p align="center">PATCH 警报</p>| <p align="center">订阅订阅</p>|
|:------------------|:---------|:-----------|:------------------|
|[Microsoft Defender for Cloud](/azure/defender-for-cloud/alerts-overview)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/playbook) | <p align="center">&#x2713;</p> | <p align="center">[提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
| [Microsoft Defender for Cloud Apps](/cloud-app-security/monitor-alerts) | <p align="center">&#x2713;</p> | <p align="center">[提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|[Microsoft Defender for Endpoint](/windows/security/threat-protection/microsoft-defender-atp/attack-simulations) **| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Microsoft Defender for Identity](/defender-for-identity/understanding-security-alerts#security-alert-categories) ***| <p align="center">&#x2713;</p> | <p align="center">[提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|Microsoft 365 <ul><li> [默认](/office365/securitycompliance/alert-policies#default-alert-policies)</li> <li>[Cloud App Security](/office365/securitycompliance/anomaly-detection-policies-in-ocas)</li><li>自定义警报</li></ul> | <p align="center">&#x2713;</p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Azure 信息保护](/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive)**（预览版）**| <p align="center">&#x2713;</p> | <p align="center">[提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|[Azure Sentinel](/azure/sentinel/quickstart-get-visibility)**（预览版）**| <p align="center">&#x2713;</p> | <p align="center">在 Azure Sentinel 中不受支持 </p> | <p align="center">&#x2713;</p> |
> **注意：** 新的提供商将会不断加入 Microsoft Graph 安全生态系统。 要请求新的提供商或从现有提供商处获取更长时间的支持，请[在 Microsoft Graph 安全性 GitHub 存储库中提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new)。

\* 文件问题：警报状态在 Microsoft Graph 安全性 API 集成应用程序中得到更新，但不反映在供应商的管理经验中。

\*\*与 Microsoft Graph 安全性 API 相比，Microsoft Defender for Endpoint 所需的[用户角色](/windows/security/threat-protection/microsoft-defender-atp/user-roles)更多。 只有同时具备 Microsoft Defender for Endpoint 和 Microsoft Graph 安全性 API 角色的用户才可访问 Microsoft Defender for Endpoint 数据。 由于仅限应用程序的身份验证不受此约束限制，我们建议使用仅限应用程序的身份验证令牌。

\*\*\* Microsoft Defender for Identity 警报通过 Microsoft Defender for Cloud Apps 集成提供。 这意味着只有在加入了 Unified SecOps 并将 Microsoft Defender for Identity 连接到 Microsoft Defender for Cloud Apps 时，才会收到 Microsoft Defender for Identity 警报。 了解有关[如何集成 Microsoft Defender for Identity 和 Microsoft Defender for Cloud Apps](/defender-for-identity/mcas-integration) 的详细信息。

## <a name="information-protection"></a>信息保护

Microsoft Graph 威胁评估 API 可帮助组织评估租户中任何用户收到的威胁。 这样，客户就可将其收到的垃圾电子邮件、网络钓鱼 URL 或恶意软件附件报告给 Microsoft。 策略检查结果和重新扫描结果可帮助租户管理员了解威胁扫描判定并调整其组织策略。

## <a name="secure-score"></a>安全功能分数

[Microsoft 安全功能分数](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/A-new-home-and-an-all-new-look-for-Microsoft-Secure-Score/ba-p/529641)是一款安全分析解决方案，可让你了解安全项目组合以及如何改进这些组合。 只需一个分数，你就可以更好地了解已采取了哪些措施来降低 Microsoft 解决方案中的风险。 此外，你还可以将你的分数与其他组织比较，以了解你的分数趋势。 Microsoft Graph 安全性 [secureScore](securescore.md) 和 [secureScoreControlProfile](securescorecontrolprofile.md) 实体可以帮助你实现组织的安全性与生产力需求之间的平衡，同时支持相应的安全功能混合。 你也可以计划采取安全功能之后的分数。

## <a name="common-use-cases"></a>常见用例

下面是为使用 Microsoft Graph 安全性 API 而提出的最常见请求：

| **用例**   | **REST 资源** | **在 Graph 浏览器中试调用** |
|:---------------|:--------|:----------|
| 列出警报 | [List alerts](../api/alert-list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| 更新警报 | [Update alert](../api/alert-update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |
|列出安全功能分数|[列出 secureScore](../api/security-list-securescores.md) |[https://graph.microsoft.com/v1.0/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com)|
|获取安全功能分数|[获取 secureScore](../api/securescore-get.md) |[https://graph.microsoft.com/v1.0/security/secureScores/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores/{id}&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com)|
|列出安全功能分数控制配置文件|[列出 secureScoreControlProfiles](../api/security-list-securescorecontrolprofiles.md) |[https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com)|
|获取安全功能分数控制配置文件|[获取 secureScoreControlProfile](../api/securescorecontrolprofile-get.md) |[https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com)|
|更新安全功能分数控制配置文件|[更新 secureScoreControlProfile](../api/securescorecontrolprofile-update.md) |[https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com)|


可使用 Microsoft Graph [Webhook](/graph/webhooks) 订阅和接收与 Microsoft Graph 安全性实体更新相关的通知。

## <a name="resources"></a>资源

Microsoft Graph 安全性 API 示例的代码和贡献情况：

- [ASP.NET (C#) 示例](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python 示例](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript) 示例](https://github.com/microsoftgraph/nodejs-security-sample)

与社区互动：

- [加入技术社区](https://aka.ms/graphsecuritycommunity)
- [在 StackOverflow 上讨论](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="whats-new"></a>最近更新
了解这些 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="next-steps"></a>后续步骤

Microsoft Graph 安全性 API 可以为你提供使用 Microsoft 和合作伙伴的不同安全解决方案的新方式。请按照以下步骤操作开始使用：

- 向下滚动至 [alerts](alert.md)、[secureScore](securescore.md) 和 [secureScoreControlProfiles](securescorecontrolprofile.md)。
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