---
author: JeremyKelley
ms.date: 09/10/2017
title: 发送访问项目的邀请
ms.localizationpriority: medium
ms.prod: sharepoint
description: 发送 driveItem 的共享邀请。
doc_type: apiPageType
ms.openlocfilehash: 05a1502363244b0ee438a4a1afb05e967ad7890d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026645"
---
# <a name="send-a-sharing-invitation"></a>发送共享邀请

命名空间：microsoft.graph

发送 **driveItem 的共享邀请**。
共享邀请向收件人提供权限，并选择性地向其发送带[共享链接][]的电子邮件。

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

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

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

| 参数        | 类型                           | 说明
|:-----------------|:-------------------------------|:-------------------------
| recipients       | Collection([DriveRecipient][]) | 将获得访问权限和共享邀请的收件人的集合。
| message          | String                         | 共享邀请中包含的纯文本格式的邮件。最大长度为 2000 个字符。
| requireSignIn    | Boolean                        | 指定邀请的收件人是否需要登录才能查看共享项。
| sendInvitation   | Boolean                        | 如果为 true，则向收件人发送[共享链接][]。 否则，直接授予权限，而不发送通知。
| 角色            | 集合（字符串）             | 指定要授予共享邀请收件人的角色。
| expirationDateTime | DateTimeOffset                       | 指定权限过期的 DateTime。 可用于OneDrive for Business、SharePoint和高级个人OneDrive帐户。
| 密码           | String                         | 创建者邀请上设置的密码。 可选且OneDrive个人。

## <a name="example"></a>示例

本示例向电子邮件地址为“ryan@contoso.com”的用户发送共享邀请，其中包含关于协作文件的讯息。
此邀请授予 Ryan 对该文件的读写访问权限。

### <a name="http-request"></a>HTTP 请求

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [permission](../resources/permission.md) 集合对象。


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.com"
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面是一个响应示例。

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
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

## <a name="remarks"></a>备注

* **driveType** 为 `personal` 的 [Drives](../resources/drive.md)（OneDrive 个人版）无法创建或修改根 DriveItem 上的权限。
* 有关可用角色的列表，请参阅 [roles 属性值](../resources/permission.md#roles-property-values)。

## <a name="error-responses"></a>错误响应

请阅读 [错误响应][error-response] 主题，以了解有关如何返回错误的详细信息。


[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[共享链接]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
  ]
} -->

