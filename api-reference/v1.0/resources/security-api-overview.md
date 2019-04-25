---
title: 使用 Microsoft Graph 安全性 API
description: Microsoft Graph 安全性 API 提供了统一的界面的架构，用于与 Microsoft 和生态系统合作伙伴的安全性解决方案集成。 这使客户能够简化安全性操作和更好地抵御日益增多的网络威胁。 Microsoft Graph 安全性 API 可用作联合安全聚合服务，向所有已启用的安全提供程序提交查询，以获得聚合响应。 使用 Microsoft Graph 安全性 API 构建可实现以下操作的应用程序：
localization_priority: Priority
author: preetikr
ms.prod: security
ms.openlocfilehash: bd208067c2194766bb5f3d93d0caa21be086dca0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579182"
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

Microsoft Graph 安全性 API 提供来自以下提供商的警报。 下表中显示了对 GET 警报、PATCH 警报（可通过 Microsoft Graph 安全性 API 使用更新，但这些更新可能未在提供商的管理体验中公开）和“订阅”功能（通过 Webhook）。

| 安全提供商 | <p align="center">GET 警报</p>| <p align="center">PATCH 警报</p>| <p align="center">订阅订阅</p>|
|:------------------|:---------|:-----------|:------------------|
|[Azure 安全中心](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Azure Active Directory Identity Protection](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook) | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
| [Microsoft Cloud App Security](https://docs.microsoft.com/cloud-app-security/monitor-alerts) | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Windows Defender 高级威胁防护](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Azure 高级威胁防护](https://docs.microsoft.com/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories)| <p align="center">&#x2713;</p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|Office 365 <ul><li> [默认](https://docs.microsoft.com/zh-CN/office365/securitycompliance/alert-policies#default-alert-policies)</li> <li>[Cloud App Security](https://docs.microsoft.com/zh-CN/office365/securitycompliance/anomaly-detection-policies-in-ocas)</li></ul> | <p align="center">&#x2713;</p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Azure 信息保护](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive)**（预览版）**| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Azure Sentinel](https://docs.microsoft.com/azure/sentinel/quickstart-get-visibility)**（预览版）**| <p align="center">&#x2713;</p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Palo Alto 网络](https://docs.paloaltonetworks.com/pan-os/9-0/pan-os-web-interface-help/monitor/monitor-logs/log-types.html)| <p align="center">&#x2713;</p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
> **注意：** 新的提供商将会不断加入 Microsoft Graph 安全生态系统。 要请求新的提供商或从现有提供商处获取更长时间的支持，请[在 Microsoft Graph 安全性 GitHub 存储库中提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new)。

## <a name="common-use-cases"></a>常见用例

下面是为使用 Microsoft Graph 安全性 API 而提出的最常见请求：

| **用例**   | **REST 资源** | **在 Graph 浏览器中试调用** |
|:---------------|:--------|:----------|
| 列出警报 | [List alerts](../api/alert-list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| 更新警报 | [更新警报](../api/alert-update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

可使用 Microsoft Graph [Webhook](/graph/webhooks) 订阅和接收与 Microsoft Graph 安全性实体更新相关的通知。

## <a name="resources"></a>资源

Microsoft Graph 安全性 API 示例的代码和贡献情况：

- [ASP.NET (C#) 示例](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python 示例](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript) 示例](https://github.com/microsoftgraph/nodejs-security-sample)

与社区互动：

- [加入技术社区](https://aka.ms/graphsecuritycommunity)
- [在 StackOverflow 上讨论](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a>后续步骤

Microsoft Graph 安全性 API 可以为你提供使用 Microsoft 和合作伙伴的不同安全解决方案的新方式。 请按照以下步骤开始操作：

- 深入了解[警报](alert.md)。
- 在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。 在“**示例查询**”中，选择“**显示更多示例**”并将“安全类别”设为“**开启**”。
- 请尝试[订阅和接收实体变更通知](/graph/webhooks)。

需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。

## <a name="see-also"></a>另请参阅

Microsoft Graph 安全性 API 示例的[代码和贡献情况](https://github.com/microsoftgraph/security-api-solutions/blob/master/CONTRIBUTING.md)：

- [ASP.NET (C#) 示例](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python 示例](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript) 示例](https://github.com/microsoftgraph/nodejs-security-sample)
- [PowerShell 示例](https://aka.ms/graphsecuritypowershellsample)
- [其他示例或贡献新的示例](https://aka.ms/graphsecurityapicode)

了解可与 Microsoft Graph 安全性 API 连接的其他选项：

- [适用于 Logic Apps、Flow 和 PowerApps 的 Microsoft Graph 安全性连接器](https://aka.ms/graphsecurityconnectors)
- [适用于 Power BI 的 Microsoft Graph 安全性连接器](https://aka.ms/graphsecuritypowerbiconnectordoc)
- [Jupyter Notebook 示例](https://aka.ms/graphsecurityjupyternotebooks)

与社区互动：

- [加入技术社区](https://aka.ms/graphsecuritycommunity)
- [在 StackOverflow 上讨论](https://stackoverflow.com/questions/tagged/microsoft-graph-security)