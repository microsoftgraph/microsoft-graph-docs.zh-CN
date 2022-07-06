---
title: 更新 profilePhoto
description: 更新已登录用户、指定组或联系人的照片。
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fb3ccef7898305dbd76f891ff85019da853187dc
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645483"
---
# <a name="update-profilephoto"></a>更新 profilePhoto

命名空间：microsoft.graph

更新已登录 **用户**、指定 **组** 或 **联系人** 的照片。

由于每个 REST 请求的总大小当前限制为 4 MB，可以添加的照片大小也限制为 4 MB。 以下是Exchange Online上 HD 照片支持的维度：`48x48`、、`64x64`、`96x96`、`240x240``120x120`、`360x360`、`432x432``504x504`和 `648x648`。

可以在版本 1.0 中使用 PATCH 或 PUT 执行此操作。

> **注意：** 此操作仅支持用户的工作或学校邮箱，而不支持个人邮箱。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="to-update-the-profile-photo-of-the-signed-in-user"></a>要更新已登录用户的个人资料照片

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）      |   User.ReadWrite、User.ReadWrite.All           |
|委派（个人 Microsoft 帐户）      |   不支持。            |
|应用程序      |    User.ReadWrite.All           |

### <a name="to-update-the-profile-photo-of-a-group"></a>要更新组的个人资料照片

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）      |   Group.ReadWrite.All           |
|委派（个人 Microsoft 帐户）      |   不支持。            |
|应用程序      |    Group.ReadWrite.All           |

### <a name="to-update-the-profile-photo-of-a-contact"></a>要更新联系人的个人资料照片

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）      |   Contacts.ReadWrite           |
|委派（个人 Microsoft 帐户）      |   不支持。            |
|应用程序      |    Contacts.ReadWrite           |

> [!NOTE]
> 1. 若要更新组织中任何用户的照片，应用必须具有 *User.ReadWrite.All* 应用程序权限，并以自己的标识（而不是代表用户）调用此 API。 若要了解详细信息，请参阅[在没有已登录用户的情况下进行访问](/graph/auth-v2-service)。 更新已登录用户的照片仅需要 *User.ReadWrite 权* 限。
> 2. 当前在使用应用权限访问组照片方面存在一个 [已知问题](/graph/known-issues#groups)。
> 3. Azure AD B2C 租户目前不支持使用 Microsoft 图形 API 更新用户的照片。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/photo/$value
PATCH /users/{id | userPrincipalName}/photo/$value
PATCH /groups/{id}/photo/$value
PATCH /me/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PATCH /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value

PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | image/jpeg。必需。  |

## <a name="request-body"></a>请求正文
在请求正文中，包括请求正文中照片的二进制数据。

## <a name="response"></a>响应

如果成功，此方法返回 `200 OK` 响应代码。
## <a name="example"></a>示例
### <a name="request"></a>请求
请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-profilephoto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应
下面展示了示例响应。 
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

