---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 发送邀请以访问项目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b324c92f58090159643aeecd4a6e2d1e24fb2f44
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861142"
---
# <a name="send-a-sharing-invitation"></a>发送共享邀请

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

发送 **DriveItem** 的共享邀请。共享邀请为收件人提供权限，也可以选择向收件人发送电子邮件以通知他们项目已共享。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.ReadWrite、Files.ReadWrite.All    |
|应用程序 | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite" } -->

```json
{
  "requireSignIn": false,
  "sendInvitation": false,
  "roles": [ "read | write"],
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" },
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "message": "string"
}
```

| 参数        | 类型                                            | 说明                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| recipients       | Collection([DriveRecipient](../resources/driverecipient.md)) | 将获得访问权限和共享邀请的收件人的集合。                                            |
| message          | String                                          | 共享邀请中包含的纯文本格式的邮件。最大长度为 2000 个字符。 |
| requireSignIn    | Boolean                                         | 指定邀请的收件人要查看共享项目的登录位置。            |
| sendInvitation   | Boolean                                         | 指定是否生成电子邮件或帖子 (false)，或是否仅创建权限 (true)。            |
| roles            | 集合（字符串）                              | 指定授予共享邀请收件人的角色。                         |
| expirationDateTime | DateTimeOffset                       | 指定权限将在其后过期的日期时间。 在 OneDrive for business、SharePoint 和 premium 个人 OneDrive 帐户上可用。
| 密码           | String                         | 由创建者在邀请上设置的密码。 可选和 OneDrive 仅个人版

## <a name="example"></a>示例

本示例向电子邮件地址为“ryan@contoso.org”的用户发送共享邀请，其中包含关于协作文件的讯息。
此邀请授予 Ryan 对该文件的读写访问权限。

### <a name="http-request"></a>HTTP 请求

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [permission](../resources/permission.md) 集合对象。


# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ],
  "password": "password123",
  "expirationDateTime": "2018-07-15T14:00:00.000Z"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面是一个响应示例。

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "hasPassword": true,
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="partial-success-response"></a>部分成功响应

当邀请多个收件人时, 通知可能会成功, 其他人也会失败。
在这种情况下, 服务将返回 HTTP 状态代码为207的部分成功响应。
当返回部分成功时, 每个失败的收件人的响应将包含`error`一个对象, 其中包含有关出错的信息以及如何修复。

下面的示例展示了部分响应。  

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 207 Multi-Status
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "John Adams",
          "id": "5D8CA5D0-FFF8-4A97-B0A6-8F5AEA339681"
        }
      },
      "id": "1EFG7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "adams@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "error": {
        "code":"notAllowed",
        "message":"Account verification needed to unblock sending emails.",
        "localizedMessage": "Kontobestätigung erforderlich, um das Senden von E-Mails zu entsperren.",
        "fixItUrl":"http://g.live.com/8SESkydrive/VerifyAccount",
        "innererror":{  
          "code":"accountVerificationRequired" 
        }
      }
    },
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="sendnotification-errors"></a>SendNotification 错误
以下是在发送通知失败时, 应用可能会在嵌套`innererror`的对象中遇到的一些其他错误。 应用程序不需要处理这些。

| 代码                           | 说明
|:-------------------------------|:--------------------------------------------------------------------------------------
| accountVerificationRequired    | 若要取消阻止发送通知, 需要进行帐户验证。
| hipCheckRequired               | 需要解决 HIP (主机入侵防护) 检查以取消阻止发送通知。
| exchangeInvalidUser            | 找不到当前用户的邮箱。
| exchangeOutOfMailboxQuota      | 配额不足。
| exchangeMaxRecipients          | 超过了可以同时发送通知的收件人的最大数量。

>**注意:** 服务可随时添加新的错误代码或停止返回旧的错误代码。

## <a name="remarks"></a>注解

* 具有 `personal` **driveType**（OneDrive 个人版）的[驱动器](../resources/drive.md)无法创建或修改根 DriveItem 上的权限。
* 如需可用角色的列表，请参阅[角色枚举](../resources/permission.md#roles-enumeration-values)。

## <a name="error-responses"></a>错误响应

请参阅[错误响应][error-response]主题，详细了解错误返回方式。


[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
  ]
}
-->
