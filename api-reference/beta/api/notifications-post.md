---
title: 创建和发送通知
description: 创建并发送针对用户通过 Microsoft Graph 的通知。
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 6062153c1eaff68a19cd5b27ac10efa9bacafb93
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937922"
---
# <a name="create-and-send-a-notification"></a>创建和发送通知
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建并发送针对用户通过 Microsoft Graph 的通知。 通知存储在 Microsoft Graph 通知源存储中，并发送到用户登录到的所有设备终结点上的所有应用程序客户端。  

## <a name="permissions"></a>Permissions
您的应用程序服务不需要任何额外的权限即可向目标用户发布通知。  

> [!IMPORTANT]
> 如果选择通过委派权限代表用户发布通知，则需要以下权限之一才能调用此 API。 建议您不要选择此选项来创建通知。 如果想要了解详细信息，包括如何选择权限，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Notifications.ReadWrite.CreatedByApp    |
|委派（个人 Microsoft 帐户） | Notifications.ReadWrite.CreatedByApp    |
|Application | 不支持。|



## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a>请求标头
|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|Authorization | string |授权标头用于传递呼叫方的凭据。 持有者 {令牌}。 必填。 |
|X-UNS-ID | string |Microsoft Graph 通知服务在创建订阅后返回的 UserNotificationSubscriptionId，并用于面向特定用户。 必需。 |
|Content-type | appliation/json。 必填。|

## <a name="request-body"></a>请求正文
在请求正文中，提供[通知](../resources/projectrome-notification.md)对象的 JSON 表示形式。

## <a name="response"></a>响应
如果成功，此方法将`201 Created`返回响应代码，指示已成功创建和存储通知。 随后，通知将通过有效订阅扇到所有指定的终结点。 

## <a name="example"></a>示例
### <a name="request"></a>请求
请求示例如下所示。

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2019-10-30T23:59:00.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
    "windows",
    "ios",
    "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "60"
}
```

### <a name="response"></a>响应
下面是对应响应的一个示例。

```http
HTTP/1.1 201
client-request-id: 71e62feb-8d72-4912-8b2c-4cee9d89e781
content-length: 356
content-type: application/json
location: https://graph.microsoft.com/beta/me/activities/119081f2-f19d-4fa8-817c-7e01092c0f7d
request-id: 71e62feb-8d72-4912-8b2c-4cee9d89e781

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('graphnotify%40contoso.com')/notifications/$entity",
    "displayTimeToLive": 59,
    "expirationDateTime": "2019-10-28T22:05:36.25Z",
    "groupName": "TestGroup",
    "id": "119081f2-f19d-4fa8-817c-7e01092c0f7d",
    "priority": "High",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```
