---
title: 创建和发送通知
description: 创建并发送针对用户通过 Microsoft Graph 的通知。
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 8eb35ea0ade2e7d471674d8d064ba0ac38b361cc
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996262"
---
# <a name="create-and-send-a-notification"></a>创建和发送通知
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建并发送针对用户通过 Microsoft Graph 的通知。 通知存储在 Microsoft Graph 通知源存储中，并发送到用户登录到的所有设备终结点上的所有应用程序客户端。  

## <a name="permissions"></a>权限
您的应用程序服务不需要任何额外的权限即可向目标用户发布通知。  

> [!IMPORTANT]
> 如果选择通过委派权限代表用户发布通知，则需要以下权限之一才能调用此 API。 建议不要在发布通知时选择此选项，但如果您想了解详细信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Notifications.ReadWrite.CreatedByApp    |
|委派（个人 Microsoft 帐户） | Notifications.ReadWrite.CreatedByApp    |
| 应用程序                           | 不支持。 |


## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a>请求标头
|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|Authorization | string |授权标头用于传递呼叫方的凭据。 持有者 {令牌}。 必填。 |
|X-UNS-ID | string |Microsoft Graph 通知服务在客户端上创建订阅后返回的 UserNotificationSubscriptionId，用于面向特定用户。 必需。 |
|Content-type| application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供[通知](../resources/projectrome-notification.md)对象的 JSON 表示形式。

## <a name="response"></a>响应
如果成功，此方法将`201 Created`返回响应代码，指示已成功创建和存储通知。 随后，通知将通过有效订阅扇到所有指定的终结点。 

## <a name="example"></a>示例
### <a name="request"></a>请求
请求示例如下所示。


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_notification_from_user"
}-->

```http
POST https://graph.microsoft.com/beta/me/notifications
Content-type: application/json

{
  "notification": {
    "targetHostName": "targetHostName-value",
    "appNotificationId": "appNotificationID-value",
    "expirationDateTime": "datetime-value",
    "targetPolicy": {
      "platformTypes": [
        "platformTypes-value"
        ]
      }, 
    "payload": {
      "rawContent": "rawContent-value",
      "visualContent": {
        "title": "title-value",
        "body": "body-value"
      }
    },
    "displayTimeToLive": 99,
    "priority": "priority-value",
    "groupName": "groupName-value"
  }
}
```
# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-notification-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notification"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "notification": {
    "targetHostName": "targetHostName-value",
    "expirationDateTime": "datetime-value",
    "payload": {
      "rawContent": "rawContent-value",
      "visualContent": {
        "title": "title-value",
        "body": "body-value"
      }
    },
    "displayTimeToLive": 99,
    "priority": "priority-value",
    "groupName": "groupName-value"
  }
}
```
