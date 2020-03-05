---
title: 创建和发送通知
description: 创建并发送针对用户通过 Microsoft Graph 的通知。
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: b66544406372c2eaa7be6f8f4261c75cbd7c6c5e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451663"
---
# <a name="create-and-send-a-notification"></a>创建和发送通知

命名空间： microsoft. graph[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建并发送针对用户通过 Microsoft Graph 的通知。 通知存储在 Microsoft Graph 通知源存储中，并发送到用户登录到的所有设备终结点上的所有应用程序客户端。  

## <a name="permissions"></a>权限
您的应用程序服务不需要任何额外的权限即可向目标用户发布通知。  

> [!IMPORTANT]
> 如果选择通过委派权限代表用户发布通知，则需要以下权限之一才能调用此 API。 建议您不要选择此选项来创建通知。 如果想要了解详细信息，包括如何选择权限，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Notifications.ReadWrite.CreatedByApp    |
|委派（个人 Microsoft 帐户） | Notifications.ReadWrite.CreatedByApp    |
|应用程序 | 不支持。|



## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a>请求标头
|名称 | 说明|
|:----|:-----------|
|Authorization | 授权标头用于传递呼叫方的凭据。 持有者 {令牌}。 必填。 |
|X-UNS-ID | Microsoft Graph 通知服务在创建订阅后返回的 UserNotificationSubscriptionId，并用于面向特定用户。 必需。 |
|Content-type | application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供[通知](../resources/projectrome-notification.md)对象的 JSON 表示形式。

## <a name="response"></a>响应
如果成功，此方法将`201 Created`返回响应代码，指示已成功创建和存储通知。 随后，通知将通过有效订阅扇到所有指定的终结点。 

下表列出了可能返回的错误和响应代码。

|错误代码             | Descrition                             |
|:-----------------------------------|:----------------------------------------------------------|
|HttpStatusCode。 BadRequest           | Body 为数组（不支持多个通知）。|
|HttpStatusCode。 BadRequest           | 正文与 API 的协定不匹配。               |
|HttpStatusCode            | 呼叫者位于阻止列表中。                          |
|HttpStatusCode。 MethodNotAllowed     | 不支持使用的 HTTP 方法。                     |
|HttpStatusCode。 BadRequest           | 请求中存在不受支持的标头。 不支持两个标头：<br/><br/>修改时间-自<br/>If-Range |                    
|HttpStatusCode。 UnsupportedMediaType | 标头内容编码存在，并且具有除`Deflate`或`Gzip`之外的压缩算法值。  |
|HttpStatusCode。 BadRequest           | 有效负载无效。                                           |
|HttpStatusCode            | 呼叫者无权代表用户执行操作或向用户发送通知。                         |
|HttpStatusCode 未经授权         |  请求正文包含无效的活动数据类型。        |
|HttpStatusCode                   |  已成功创建活动。                            |
|HttpStatusCode。 NotAcceptable        |  请求已被阻止或服务器正忙。    |


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
