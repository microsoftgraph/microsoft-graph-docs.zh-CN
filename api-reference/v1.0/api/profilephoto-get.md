---
title: 获取照片
description: 获取指定的 profilePhoto 或其元数据（profilePhoto 属性）。
localization_priority: Priority
author: kevinbellinger
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c3bd5a0d69ab392fc55ac1f44bfbe3dc6d74ad08
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790613"
---
# <a name="get-photo"></a>获取照片

命名空间：microsoft.graph

获取指定的 [profilePhoto](../resources/profilephoto.md) 或其元数据（profilePhoto 属性）。

> **注意**：在版本 1.0 中，此操作仅支持用户的工作或学校邮箱，不支持个人邮箱。

Microsoft 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。 如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。

可以获取最大照片的元数据，也可以指定尺寸来获取相应照片尺寸的元数据。
如果请求的大小不可用，则仍然可以获取用户已上载且可供使用的较小大小。
例如，如果用户上传像素为 504x504 的照片，除 648x648 外的所有尺寸的照片都可供下载。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 对于 **user** 资源：<br/>User.Read、User.ReadBasic.All、User.Read.All、User.ReadWrite、User.ReadWrite.All<br /><br />对于 **group** 资源：<br />Group.Read.All、Group.ReadWrite.All<br /><br />对于 **contact** 资源：<br />Contacts.Read、Contacts.ReadWrite |
|委派（个人 Microsoft 帐户） | 不支持 |
|应用程序                        | 对于 **user** 资源：<br/>User.Read.All、User.ReadWrite.All<br /><br />对于 **group** 资源：<br />Group.Read.All、Group.ReadWrite.All<br /><br />对于 **contact** 资源：<br />Contacts.Read、Contacts.ReadWrite |

> **注意：** 当前有一个 [已知问题](/graph/known-issues#groups)，即使用应用程序权限访问组照片。

## <a name="http-request"></a>HTTP 请求

### <a name="get-the-photo"></a>获取照片
<!-- { "blockType": "ignored" } -->

```http
GET /me/photo/$value
GET /users/{id | userPrincipalName}/photo/$value
GET /groups/{id}/photo/$value
GET /me/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contacts/{id}/photo/$value
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```

### <a name="get-the-metadata-of-the-photo"></a>获取照片的元数据
<!-- { "blockType": "ignored" } -->

```http
GET /me/photo
GET /me/photos
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

### <a name="get-the-metadata-for-a-specific-photo-size"></a>获取指定照片尺寸的元数据
<!-- { "blockType": "ignored" } -->

```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
```

## <a name="path-parameters"></a>路径参数

|参数|类型|说明|
|:-----|:-----|:-----|
|size  |String  | 照片尺寸。 Microsoft 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。 如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。 |

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
### <a name="response-for-getting-the-photo"></a>获取照片的响应
如果成功，此方法返回 `200 OK` 响应代码和所请求照片的二进制数据。如果照片不存在，此操作返回 `404 Not Found`。
### <a name="response-for-getting-the-metadata-of-the-photo"></a>获取照片元数据的响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象。
## <a name="examples"></a>示例

### <a name="example-1-get-the-photo-for-the-signed-in-user-in-the-largest-available-size"></a>示例 1：为已登录用户获取最大可用大小的照片
##### <a name="request"></a>请求
<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response"></a>响应
包含所请求照片的二进制数据。 HTTP 响应代码为 200。

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-user"></a>示例 2：获取已登录用户的 48x48 照片
##### <a name="request"></a>请求
<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a>响应
包含所请求的 48x48 照片的二进制数据。 HTTP 响应代码为 200。

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a>示例 3：获取已登录用户的用户照片的元数据
##### <a name="request"></a>请求
<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response"></a>响应

以下响应数据显示照片的元数据。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "ignored"
}-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

以下响应数据显示还没有为用户上传照片时的响应内容。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "ignored"
}-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```

## <a name="using-the-binary-data-of-the-requested-photo"></a>使用所请求照片的二进制数据

使用 `/photo/$value` 终结点来获取个人资料照片的二进制数据时，需要将数据转换为 Base64 字符串，以便将其添加为电子邮件附件。 以下是 JavaScript 中的一个示例，介绍如何创建一个数组，并将其作为 [Outlook 邮件](user-post-messages.md)的 `Attachments` 参数值传递。

```java
const attachments = [{
  '@odata.type': '#microsoft.graph.fileAttachment',
  ContentBytes: file.toString('base64'),
  Name: 'mypic.jpg'
}];
```

有关此示例的实现，请参阅[用于 Node.js 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample)。

如果想要在网页上显示图像，可以通过图像创建内存中对象，然后使该对象成为图像元素源。 以下示例演示了如何在 JavaScript 中执行此操作。

```javascript
const url = window.URL || window.webkitURL;
const blobUrl = url.createObjectURL(image.data);
document.getElementById(imageElement).setAttribute("src", blobUrl);
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

