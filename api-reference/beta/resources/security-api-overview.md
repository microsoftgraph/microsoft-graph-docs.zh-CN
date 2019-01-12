---
title: 使用 Microsoft Graph 安全性 API
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Priority
author: preetikr
ms.prod: security
ms.openlocfilehash: bc5a307b17a37f5523e3dbc8b145c248b0226471
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944766"
---
# <a name="use-the-microsoft-graph-security-api"></a>使用 Microsoft Graph 安全性 API

 > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

Microsoft Graph 安全 API 提供统一的接口和集成使用经 Microsoft 和生态系统的合作伙伴的安全解决方案的架构。 这使客户能够简化安全性操作和更好地防御增加网络威胁。 Microsoft Graph 安全 API 可以作为联盟的安全聚合服务，用于向所有 onboarded 安全提供程序获取聚合的响应提交查询。 使用 Microsoft Graph 安全 API 来构建应用程序的：

- 合并和关联多个来源的安全警告
- 解除锁定上下文数据来告知调查
- 自动化安全操作以提高效率
- 提供的可见性安全数据，以启用主动风险管理

Microsoft Graph 安全 API 包括以下主要实体。

## <a name="alerts"></a>警报

通知是潜在客户的租户的 Microsoft 或合作伙伴的安全解决方案已经确定并标记的操作或通知中的安全问题。 与 Microsoft Graph 安全[警报](alert.md)实体，您可以统一并简化跨所有集成的解决方案的安全问题。 这还允许应用程序关联的通知和上下文改进威胁保护和响应。 通过减少调查时间和时间的事件的分辨率，这些解锁安全运营效率。 使用通知更新功能中，可以跨不同安全产品和服务与 Microsoft Graph 安全 API 通过更新[通知](alert.md)实体集成同步特定警报的状态。

Microsoft Graph 安全集成解决方案将收到来自下列安全提供程序的通知：

- [Azure 安全中心](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [Azure Active Directory 标识保护](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [Microsoft 云应用程序安全性](https://docs.microsoft.com/cloud-app-security/monitor-alerts )
- [Windows Defender 高级威胁保护](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)
- [Azure 信息保护](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive)**（预览）**
- Microsoft Intune **（专用预览）**
- Office 365 **（即将推出）**
- Azure 高级威胁保护 **（即将推出）**
- 合作伙伴解决方案，如帕洛阿尔托市网络应用程序框架

> **注意：** 新的提供程序持续是加入到 Microsoft Graph Security 生态系统。

## <a name="secure-score-preview"></a>安全分数 （预览）

[Microsoft 安全 Score](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358)是使您了解您安全的项目组合和如何提高其安全分析解决方案。 单个分数，您可以更好地了解以降低风险 Microsoft 解决方案中的已完成。 您还可以比较您与其他组织的分数，并查看随着时间的推移您分数趋势已如何。 Microsoft Graph Security [secureScore](securescores.md)和[secureScoreControlProfiles](securescorecontrolprofiles.md)实体可帮助您平衡贵组织的安全性和工作效率需要同时启用适当的安全功能的组合。 您也可以计划您分数采用采用安全功能之后。

## <a name="common-use-cases"></a>常见用例

下面是一些有关使用 Microsoft Graph 安全 API 最常用的请求。

| **用例**   | **REST 资源** | **尝试在图资源管理器** |
|:---------------|:--------|:----------|
| 列出警报 | [列出警报](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| 更新通知 | [更新警报](../api/alert-update.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) |
|列表安全分数|[列表 secureScores](../api/securescores-list.md)（预览）|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|列表安全分数控件配置文件|[列表 secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md)（预览）|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|更新安全分数控件配置文件|[更新 secureScoreControlProfiles](../api/securescorecontrolprofiles-update.md)（预览）|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|

您可以使用 Microsoft Graph [webhooks](/graph/webhooks)订阅和接收有关 Microsoft Graph Security 实体更新通知。

## <a name="next-steps"></a>后续步骤

您可以使用不同的安全解决方案来自 Microsoft 和合作伙伴进行新的方法可以打开 Microsoft Graph 安全 API。 按照以下步骤开始：

- 向下钻取到[通知](alert.md)， [secureScore](securescores.md) （预览） 和[secureScoreControlProfiles](securescorecontrolprofiles.md) (Preview)。
- 尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。 下**的示例查询**，选择**显示更多示例**，并设置为**上**的安全类别。
- 尝试在实体更改[订阅和接收通知](/graph/webhooks)。

需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。

## <a name="see-also"></a>另请参阅

代码并参与到这些 Microsoft Graph 安全 API 示例：

- [ASP.NET (C#) 示例](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python 示例](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript) 示例](https://github.com/microsoftgraph/nodejs-security-sample)

社区的使用：

- [加入技术社区](https://aka.ms/graphsecuritycommunity)
- [讨论在 StackOverflow 上](https://stackoverflow.com/questions/tagged/microsoft-graph-security)
