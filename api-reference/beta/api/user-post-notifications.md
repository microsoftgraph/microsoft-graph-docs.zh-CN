---
title: '创建并发送已 (的通知) '
description: 通过 Microsoft Graph 创建并发送面向用户Graph。
ms.localizationpriority: medium
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 33346ef8a625b08652c3b11d8ac9e4e3b17e6060
ms.sourcegitcommit: 7a0f9f1a535795c6f77c80e02fd97581c36f1273
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/27/2021
ms.locfileid: "61608911"
---
# <a name="create-and-send-a-notification-deprecated"></a>创建并发送已 (的通知) 

命名空间：microsoft.graph

> [!IMPORTANT]
> Microsoft Graph通知 API 已弃用，将在 2022 年 1 月底停止返回数据。 有关其他通知体验，请参阅Microsoft Azure[中心"，](/azure/notification-hubs)[并查看此博客](https://devblogs.microsoft.com/microsoft365dev/retiring-microsoft-graph-notifications/)文章了解详细信息。

通过 Microsoft Graph 创建并发送面向用户Graph。 通知存储在 Microsoft Graph源存储中，并发送到用户登录的所有设备终结点上的所有应用客户端。  

## <a name="permissions"></a>权限
您的应用程序服务不需要任何其他权限来向目标用户发布通知。  

> [!IMPORTANT]
> 如果选择改为通过委派权限代表用户发布通知，则调用此 API 需要以下权限之一。 建议不要使用此选项来创建通知。 若要了解更多信息，包括如何选择权限，请参阅 [权限](/graph/permissions-reference)。

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
|Authorization | 授权标头用于传递调用方凭据。 Bearer {token}。 必需。 |
|X-UNS-ID | 创建订阅后由 Microsoft Graph UserNotificationSubscriptionId，用于定位特定用户。 必需。 |
|Content-type | application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供通知对象的 JSON [表示](../resources/projectrome-notification.md) 形式。

## <a name="response"></a>响应
如果成功，此方法返回 `201 Created` 响应代码，指示已成功创建和存储通知。 通知随后会扇出到具有有效订阅的所有指定终结点。 

下表列出了可能的错误和可返回的响应代码。

|错误代码             | Descrition                              |
|:-----------------------------------|:----------------------------------------------------------|
|HttpStatusCode.BadRequest           | 正文是一个 (，不支持多个) 。|
|HttpStatusCode.BadRequest           | 正文与 API 的协定不匹配。               |
|HttpStatusCode.Forbidden            | 呼叫者位于阻止列表中。                          |
|HttpStatusCode.MethodNotAllowed     | 使用的 HTTP 方法不受支持。                     |
|HttpStatusCode.BadRequest           | 请求中出现不受支持的标题。 不支持两个标头：<br/><br/>If-Modified-Since<br/>If-Range |                    
|HttpStatusCode.UnsupportedMediaType | 标头 Content-Encoding 存在，并且具有除 或 外的其他 `Deflate` 压缩算法值 `Gzip` 。  |
|HttpStatusCode.BadRequest           | 有效负载无效。                                           |
|HttpStatusCode.Forbidden            | 呼叫者无权代表用户或向用户发送通知。                         |
|HttpStatusCode.Unauthorized         |    请求正文包含无效的活动数据类型。        |
|HttpStatusCode.OK                   |     已成功创建活动。                            |
|HttpStatusCode.NotAcceptable        |    请求已受到限制或服务器繁忙。    |


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
下面是相应响应的示例。

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


