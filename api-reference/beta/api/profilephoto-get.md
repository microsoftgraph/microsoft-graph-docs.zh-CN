---
title: 获取照片
description: 获取指定的 profilePhoto 或其元数据（**profilePhoto** 属性）。
ms.localizationpriority: high
doc_type: apiPageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: 690720e1c2de153a7b56aab30a1212f4b530a468
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695411"
---
# <a name="get-photo"></a>获取照片

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 Microsoft 365 中指定的 [profilePhoto](../resources/profilephoto.md) 或其元数据（**profilePhoto** 属性）。

> **注意**：尝试获取 **用户** 照片时，此操作将首先尝试从 Microsoft 365 检索指定的照片。 如果 Microsoft 365 中没有此照片，则 API 将尝试从 Azure Active Directory 检索该照片。

Microsoft 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。 如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。

可以获取最大可用照片的元数据，或者指定一个大小来获取该照片大小的元数据。如果请求的大小不可用，则仍然可以获取用户已上载且可供使用的较小大小。例如，如果用户上传 504x504 像素的照片，则除大小为 648x648 的照片之外所有照片都可供下载。如果在用户邮箱或 Azure Active Directory 中未找到可用的指定大小，则会返回 1x1 的大小和剩余的元数据。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

> **注意：** beta 版中的获取照片方法支持用户的工作、学校或个人帐户。 但是获取照片元数据方法仅支持用户的工作或学校帐户，不支持个人帐户。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 对于 **user** 资源：<br/>User.Read、User.ReadBasic.All、User.Read.All、User.ReadWrite、User.ReadWrite.All<br /><br />对于 **group** 资源：<br />Group.Read.All、Group.ReadWrite.All<br /><br />对于 **contact** 资源：<br />Contacts.Read、Contacts.ReadWrite |
|委派（个人 Microsoft 帐户）  <br /> **注意**：不支持元数据操作。 | 对于 **user** 资源：<br/>User.Read、User.ReadWrite<br /><br />对于 **contact** 资源：<br />Contacts.Read、Contacts.ReadWrite |
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

|**参数**|**类型**|**说明**|
|:-----|:-----|:-----|
|size  |String  | 照片尺寸。 Microsoft 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。 如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。 |

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求头
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

### <a name="example-1-get-the-photo-of-the-signed-in-user-in-the-largest-available-size"></a>示例 1：为已登录用户获取最大可用大小的照片

##### <a name="request"></a>请求

<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response"></a>响应
包含所请求照片的二进制数据。HTTP 响应代码为 200。

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-user"></a>示例 2：获取已登录用户的 48x48 照片

##### <a name="request"></a>请求
<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a>响应
包含所请求的 48x48 照片的二进制数据。HTTP 响应代码为 200。

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a>示例 3：获取已登录用户的用户照片的元数据

##### <a name="request"></a>请求

<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/beta/me/photo
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```

## <a name="using-the-binary-data-of-the-requested-photo"></a>使用所请求照片的二进制数据

使用 `/photo/$value` 终结点来获取个人资料照片的二进制数据时，需要将数据转换为 Base64 字符串，以便将其添加为电子邮件附件。 以下 JavaScript 示例介绍如何创建一个数组，并将其作为 [Outlook 邮件](user-post-messages.md)的 `Attachments` 参数值传递。

```javascript
const attachments = [{
  '@odata.type': '#microsoft.graph.fileAttachment',
  ContentBytes: file.toString('base64'),
  Name: 'mypic.jpg'
}];
```

有关此示例的实现，请参阅[用于 Node.js 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample)。

如果想要在网页上显示图像，可以通过图像创建内存中对象，然后使该对象成为图像元素源。下面是此操作的 JavaScript 示例。

```javascript
const url = window.URL || window.webkitURL;
const blobUrl = url.createObjectURL(image.data);
document.getElementById(imageElement).setAttribute("src", blobUrl);
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


