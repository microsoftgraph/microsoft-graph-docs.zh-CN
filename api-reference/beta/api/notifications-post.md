---
title: 创建和发送通知
description: '创建并发送针对用户通过 Microsoft Graph 的通知。 通知存储在 Microsoft Graph 通知源存储中, 并发送到用户登录到的所有设备终结点上的所有应用程序客户端。  '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 86e67d040dcae3a013d8848c638ffadca41e4f5f
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063451"
---
# <a name="create-and-send-a-notification"></a>创建和发送通知
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建并发送针对用户通过 Microsoft Graph 的通知。 通知存储在 Microsoft Graph 通知源存储中, 并发送到用户登录到的所有设备终结点上的所有应用程序客户端。  
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Notifications.ReadWrite.CreatedByApp    |
|委派（个人 Microsoft 帐户） | Notifications.ReadWrite.CreatedByApp    |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a>请求标头
|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|Authorization | string |授权标头用于传递呼叫方的凭据。 持有者 {令牌}。 必需。 |
## <a name="request-body"></a>请求正文
在请求正文中, 提供[通知](../resources/projectrome-notification.md)对象的 JSON 表示形式。

## <a name="response"></a>响应
如果成功, 此方法将`201 Created`返回指示已成功创建和存储通知的响应代码。 
## <a name="example"></a>示例
#### <a name="request"></a>请求
下面展示了示例请求。

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2018-08-29T23:51:33.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
        "windows",
        "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "23"
}
```

#### <a name="response"></a>响应
下面展示了示例响应。

```http
HTTP/1.1 201
Content-Type: application/json
location: https://graph.microsoft.com/beta/me/notifications/518c4fb1-c565-4d67-95c4-bcc3eb8eda1b

{
    "@odata.context": "https://graph.microsoft.com/test872018/$metadata#users('graphNotificationsUser%40contoso.com')/notifications/$entity",
    "appNotificationId": "testDirectToastNotification",
    "displayTimeToLive": 23,
    "expirationDateTime": "2018-08-24T12:31:53.858Z",
    "groupName": "TestGroup",
    "id": "cd5c5e6a-99ce-470a-9982-c47635e73620",
    "priority": "1",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```


