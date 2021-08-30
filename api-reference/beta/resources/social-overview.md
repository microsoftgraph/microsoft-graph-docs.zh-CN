---
title: 使用 Microsoft Graph API 在应用中集成人员和工作区智能
description: Microsoft Graph 允许访问相关人员的有用数据、其个人资料、与之交互的文档和工作模式，并支持用户社交环境中的手势。
ms.localizationpriority: high
author: simonhult
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 17b0c03659e53685ff0644100f31dc7bd20df4d4
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695250"
---
# <a name="use-the-microsoft-graph-api-to-integrate-people-and-workplace-intelligence-in-an-app"></a>使用 Microsoft Graph API 在应用中集成人员和工作区智能

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph 允许访问相关人员的有用数据、其个人资料、与之交互的文档和工作模式，并支持用户社交环境中的手势。

## <a name="aggregate-and-extract-specific-information-about-people"></a>聚合并提取有关人员的特定信息

功能：人员

你可以使用 [person](../resources/person.md) 资源和 People API 从邮件、联系人和社交网络中聚合某个人员的相关信息。 根据多种通信、协作和业务关系按相关性对结果进行排序。 通过此 API 可以基于自己的条件对人员进行浏览、排序、选择、筛选或搜索。

- [列出人员](../api/user-list-people.md)

## <a name="help-users-contextualize-others-in-their-organization"></a>帮助用户将组织内的其他用户置于上下文中考虑

功能：个人资料（预览版）

若要将组织内的其他人员置于上下文中考虑，通常会查看人员的个人资料或个人资料卡片。

[profile](../resources/profile.md) 资源是关于租户内人员的信息的丰富源，提供了用于存储和检索人员信息的轻型机制。

## <a name="personalize-people-experiences-within-your-organization"></a>在组织内部提供个性化的人员体验

功能：个人资料卡片自定义（预览版）

使管理员能够自定义在组织内的 Microsoft 365 中使用的个人资料卡片上显示的信息。

[profileCardProperty](../resources/profileCardProperty.md) 资源表示 Microsoft 365 个人资料卡片上的用户的属性，便于组织打造共享的人员体验。

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a>帮助用户获得最相关的工作文档

功能：文档见解

使用见解 API 为用户标识最相关的文档：

- 列出用户[常用的](../api/insights-list-trending.md)文档
- 列出用户[使用的](../api/insights-list-used.md)文档
- 列出[与用户共享或由用户共享的](../api/insights-list-shared.md)文档
- 探索在组织内[为项目见解自定义隐私设置](/graph/insights-customize-item-insights-privacy.md)的方式。

## <a name="manage--mentions"></a>管理 @提及

功能：@-提及（预览版）

标注要通知的收件人并在邮件中引起该收件人的注意是一种常见的社交手势。
[mention](../resources/mention.md) 资源和 Mentions API 提供了一种轻型机制，可以在[邮件](../resources/message.md)中标注收件人，获取使用 @提及功能向用户发出通知的所有邮件，或者获取邮件中的每个提及。

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- 在新邮件中创建提及

  - [将提及作为新邮件的一部分进行创建并发送](../api/user-sendmail.md#request-2)
  - [将提及作为邮件草稿的一部分进行创建](../api/user-post-messages.md#request-2)

- 获取有关邮件中的提及的信息

  - [获取已登录用户的邮箱中提及该用户的所有邮件](../api/user-list-messages.md#request-2)
  - [获取邮件中的每个提及的详细信息](../api/message-get.md#request-2)

- [删除邮件中的提及](../api/message-delete.md#request-2)


## <a name="help-users-gain-insights-into-their-work-patterns"></a>帮助用户深入了解其工作模式

功能：分析（预览版）

使用分析 API 获取用户的活动统计信息及相关设置：

- [设置](../resources/settings.md)：要让分析 API 为用户返回结果，当前用户分析设置必须显示有效的 MyAnalytics 许可证、选择使用 MyAnalytics，并具有启用了图形的云托管邮箱。
- [activityStatistics](../resources/activitystatistics.md)：获取整个上周用户花时间参与的 Microsoft 365 活动的相关数据，包括工作时间内及工作之余在[通话](callactivitystatistics.md)、[聊天（即时消息）](chatactivitystatistics.md)、[电子邮件](emailactivitystatistics.md)和[会议](meetingactivitystatistics.md)上花费的小时数，以及可用于[专注工作](focusactivitystatistics.md)的小时数。

## <a name="whats-new"></a>新增功能
了解这些 API 集的[最新功能和更新](/graph/whats-new-overview)。


