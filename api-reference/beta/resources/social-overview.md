---
title: 使用 Microsoft Graph API 在应用程序中集成社交智能
description: Microsoft Graph 支持用户社交环境中的社交手势，并提供对有用人员和社交数据的访问权限。
localization_priority: Priority
author: simonhult
ms.prod: insights
ms.openlocfilehash: b5a89f46c8480fb90cd019e5b4fb370e0a6592bf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509593"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a>使用 Microsoft Graph API 在应用程序中集成社交智能

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph 支持用户社交环境中的社交手势，并提供对有用人员和社交数据的访问权限。

## <a name="aggregate-and-extract-specific-information-about-people"></a>聚合并提取有关人员的特定信息

你可以使用 [person](../resources/person.md) 资源和 People API 从邮件、联系人和社交网络中聚合某个人员的相关信息。 根据多种通信、协作和业务关系按相关性对结果进行排序。 通过此 API 可以基于自己的条件对人员进行浏览、排序、选择、筛选或搜索。

- [列出人员](../api/user-list-people.md)

## <a name="manage--mentions"></a>管理 @提及

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

## <a name="access-social-data-around-and-about-a-user"></a>访问有关用户的社交数据

Office Graph 封装了 Office 365 中的不同实体之间的关系。 使用 Office Graph 获取 Office 365 中的各个用户的社交见解。

- 列出用户[常用的项目](../api/insights-list-trending.md)
- 列出与某个用户[合作](../api/user-list-people.md)的用户
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/social-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
