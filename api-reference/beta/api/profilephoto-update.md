---
title: 更新 profilephoto
description: 更新租户中任意用户的照片，其中包括已登录用户或指定的组或联系人。
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: people
author: kevinbellinger
ms.openlocfilehash: 31d3ace676a00af96a21cf0d666012dfba4df6ae
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861363"
---
# <a name="update-profilephoto"></a>更新 profilephoto

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新租户中任何用户的照片，包括已登录用户或指定的组或联系人。 由于目前每个 REST 请求的总大小限制为 8MB，因此可以添加的照片大小限制为 8 MB 以下。

仅对此操作使用 PUT。

> **注意**：更新用户 **照片时**，此操作首先尝试更新用户Microsoft 365。 如果由于 (邮箱而失败，) API 将尝试更新Azure Active Directory。

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
> 1. 若要更新组织中任何用户的照片，你的应用必须具有 *User.ReadWrite.All* 应用程序权限，并且以其自己的身份（而不是代表用户）调用此 API。 若要了解详细信息，请参阅[在没有已登录用户的情况下进行访问](/graph/auth-v2-service)。 更新已登录用户的照片仅需要 *User.ReadWrite* 权限。
> 2. 当前在使用应用权限访问组照片方面存在一个 [已知问题](/graph/known-issues#groups)。
> 3. 目前，B2C 租户不支持使用 Microsoft Graph API 更新Azure AD的照片。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```

若要更新团队的照片，请进行以下操作：

<!-- { "blockType": "ignored" } -->
```http
PUT /groups/{teamId}/photo/$value
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
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
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
<!--
{
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


