---
title: 使用 Microsoft Graph 安全性 API
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Priority
author: preetikr
ms.prod: security
ms.openlocfilehash: cd55b2d26d7460e7421b9da19658990b53dd7580
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571693"
---
# <a name="use-the-microsoft-graph-security-api"></a>使用 Microsoft Graph 安全性 API

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph 安全性 API 提供了统一的界面的架构，用于与 Microsoft 和生态系统合作伙伴的安全性解决方案集成。 这使客户能够简化安全性操作和更好地抵御日益增多的网络威胁。 Microsoft Graph 安全性 API 可用作联合安全聚合服务，向所有已启用的安全提供程序提交查询，以获得聚合响应。 使用 Microsoft Graph 安全性 API 构建应用程序，以：

- 合并和关联多个来源的安全警报
- 解锁上下文数据，以提供调查信息
- 自动执行安全性操作，以提高效率
- 提供安全性数据可见性，实现主动风险管理

Microsoft Graph 安全性 API 包括以下关键实体。

## <a name="alerts"></a>警报

警报表示 Microsoft 或合作伙伴安全解决方已标识客户组合内存在潜在的安全问题，用于提醒用户采取操作或通知用户。 利用 Microsoft Graph 安全性[警报](alert.md)实体，可以统一和简化所有集成解决方案中的安全问题。 此外，这还可以使应用程序关联警报和上下文，以提升威胁防护和响应。 这些警报可以缩短调查时间和解决事故的时间。 利用警报更新功能，你可以更新[警报](alert.md)实体，从而同步与 Microsoft Graph 安全性 API 集成的不同安全产品和服务中的特定警报状态。

Microsoft Graph 安全集成解决方案将收到来自以下安全提供程序的警报：

- [Azure 安全中心](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [Azure Active Directory Identity Protection](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [Microsoft Cloud App Security](https://docs.microsoft.com/cloud-app-security/monitor-alerts )
- [Windows Defender 高级威胁防护](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)
- [Azure 信息保护](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive)**（预览版）**
- Microsoft Intune **（个人预览版）**
- Office 365 **（即将推出）**
- Azure 高级威胁防护 **（即将推出）**
- 合作伙伴解决方案，例如 Palo Alto 网络应用程序框架

> **注释：** 新提供程序将会不断加入 Microsoft Graph 安全生态系统。

## <a name="secure-score-preview"></a>安全功能分数（预览版）

[Microsoft 安全功能分数](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358)是一款安全分析解决方案，可让你了解安全项目组合以及如何改进这些组合。 只需一个分数，你就可以更好地了解已采取了哪些措施来降低 Microsoft 解决方案中的风险。 此外，你还可以将你的分数与其他组织比较，以了解你的分数趋势。 Microsoft Graph 安全性 [secureScore](securescores.md) 和 [secureScoreControlProfile](securescorecontrolprofiles.md) 实体可以帮助你实现组织的安全性与生产力需求之间的平衡，同时支持相应的安全功能混合。 你也可以计划采取安全功能之后的分数。

## <a name="common-use-cases"></a>常见用例

以下是使用 Microsoft Graph 安全性 API 的一些热门的请求。

| **用例**   | **REST 资源** | **在 Graph 浏览器中试调用** |
|:---------------|:--------|:----------|
| 列出警报 | [List alerts](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| 更新警报 | [Update alert](../api/alert-update.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) |
|列出安全功能分数|[List secureScores](../api/securescores-list.md)（预览版）|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|列出安全功能控制配置文件|[List secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md)（预览版）|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|更新安全功能控制配置文件|[Update secureScoreControlProfiles](../api/securescorecontrolprofiles-update.md)（预览）|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|

可以使用 Microsoft Graph [webhooks](/graph/webhooks) 订阅和接收与 Microsoft Graph 安全性实体相关的通知。

## <a name="next-steps"></a>后续步骤

Microsoft Graph 安全性 API 可以为你提供使用 Microsoft 和合作伙伴的不同安全解决方案的新方式。 请按照以下步骤开始操作：

- 向下钻取到 [alerts](alert.md)、[secureScore](securescores.md)（预览版）和 [secureScoreControlProfile](securescorecontrolprofiles.md)（预览版）。
- 尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。 在“**示例查询**”中，选择“**显示更多示例**”并将“安全类别”设为“**开启**”。
- 请尝试[订阅和接收实体变更通知](/graph/webhooks)。

需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。

## <a name="see-also"></a>另请参阅

Microsoft Graph 安全性 API 示例代码及参与 API：

- [ASP.NET (C#) 示例](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python 示例](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript) 示例](https://github.com/microsoftgraph/nodejs-security-sample)

与社区互动：

- [加入技术社区](https://aka.ms/graphsecuritycommunity)
- [在 StackOverflow 上讨论](https://stackoverflow.com/questions/tagged/microsoft-graph-security)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/security-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
