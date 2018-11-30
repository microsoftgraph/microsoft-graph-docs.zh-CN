---
title: 获取订阅
description: 检索订阅的属性和关系。
ms.openlocfilehash: 5694015fe7e8cbf87b5d62f7ae4af35d1773532b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044662"
---
# <a name="get-subscription"></a>获取订阅

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

检索订阅的属性和关系。

## <a name="permissions"></a>权限

下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 资源类型/项        | 权限          |
|-----------------------------|---------------------|
| 联系人                    | Contacts.Read       |
| Conversations               | Group.Read.All      |
| Events                      | Calendars.Read      |
| Messages                    | Mail.Read           |
| Groups                      | Group.Read.All      |
| Users                       | User.Read.All       |
| Drive（用户的 OneDrive）    | Files.ReadWrite     |
| 驱动器 （共享的 SharePoint 内容和驱动器） | Files.ReadWrite.All |
| 安全警报              | SecurityEvents.ReadWrite.All |

***注意：***/Beta 终结点允许资源最多的应用程序权限。 应用程序权限不支持对话组和 OneDrive 驱动器根项目。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:-----------|:-----|:-----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。

## <a name="example"></a>示例

##### <a name="request"></a>请求

下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a>响应

下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
