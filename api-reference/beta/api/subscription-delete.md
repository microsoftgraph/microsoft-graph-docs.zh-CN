---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9fa5a60bbb00bb7d15ae14a0b76235a5629f2c42
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140451"
---
# <a name="delete-subscription"></a>删除订阅

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除订阅。

## <a name="permissions"></a>权限

根据所请求的资源和权限类型 (委派或应用程序), 下表中指定的权限是调用此 API 所需的最低特权。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 支持的资源 | 委派（工作或学校帐户） | 委派（个人 Microsoft 帐户） | 应用程序 |
|:-----|:-----|:-----|:-----|
|[联系人](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md)(用户的个人 OneDrive) | 不支持 | Files.ReadWrite | 不支持 |
|[driveItem](../resources/driveitem.md)(OneDrive for business) | Files.ReadWrite.All | 不支持 | Files.ReadWrite.All |
|[event](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[group](../resources/group.md) | Group.Read.All | 不支持 | Group.Read.All |
|[组对话](../resources/conversation.md) | Group.Read.All | 不支持 | 不支持 |
|[message](../resources/message.md) | Mail.Read | Mail.Read | Mail.Read |
|[安全警报](../resources/alert.md) | SecurityEvents.ReadWrite.All | 不支持 | SecurityEvents.ReadWrite.All |
|[user](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **注意:** 对 OneDrive 和 Outlook 项目的订阅有其他限制。 这些限制适用于创建和管理订阅 (获取、更新和删除订阅)。

- 在个人 OneDrive 上, 您可以订阅该驱动器中的根文件夹或任何子文件夹。 在 OneDrive for business 中, 只能订阅根文件夹。 将为订阅的文件夹中的所请求类型的更改发送通知, 或在其层次结构中的任何文件、文件夹或其他 driveItem 对象上发送通知。 您无法订阅不是文件夹的**驱动器**或**driveItem**实例, 例如单个文件。

- 在 Outlook 中, 委派权限仅支持订阅登录用户的邮箱中的文件夹中的项目。 这意味着, 您不能使用委派的权限日历。读取它可订阅其他用户的邮箱中的事件。
- 若要订阅_共享或委托_文件夹中的 Outlook 联系人、事件或邮件的更改通知, 请执行以下操作:

  - 使用相应的应用程序权限订阅租户中_任何_用户的文件夹或邮箱中的项目更改。
  - 请勿使用 Outlook 共享权限 ("联系人"、"共享"、"日历"、"共享"、"邮件"、"已读/写" 等), 因为它们**不**支持对共享或委派文件夹中的项目的更改通知进行订阅。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

##### <a name="request"></a>请求

下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a>响应

下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
