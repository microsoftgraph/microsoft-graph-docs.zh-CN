---
title: 更新 profilephoto
description: 更新租户中任意用户的照片，其中包括已登录用户或指定的组或联系人。 自此处起
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: 67ec3e6400e007e5c0638bea92097e9e4945e85e
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515707"
---
# <a name="update-profilephoto"></a>更新 profilephoto

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新租户中任何用户的照片，包括登录用户或指定的组或联系人。 由于目前每个 REST 请求的总大小限制为 8MB，因此可以添加的照片大小限制为 8MB 以下。

仅对此操作使用 PUT。

> **注意**：更新用户照片 **时** ，此操作首先尝试在 Microsoft 365 中更新照片。 如果由于 (邮箱帐户而失败) ，此 API 将尝试在 Azure Active Directory 中更新照片。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | 已登录用户的个人资料 **照片**：<br/>User.ReadWrite、User.ReadWrite.All<br /><br />对于 **group** 资源：<br />Group.ReadWrite.All<br /><br />对于 **contact** 资源：<br />Contacts.ReadWrite |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application                            | 对于 **user** 资源：<br/>User.ReadWrite.All<br /><br />对于 **group** 资源：<br />Group.ReadWrite.All<br /><br />对于 **contact** 资源：<br />Contacts.ReadWrite |

> **注意** 若要更新组织中任何用户的照片，应用必须具有 User.ReadWrite.All 应用程序权限，并以其自己的身份而不是代表用户来调用此 API。 若要了解详细信息，请参阅[在没有已登录用户的情况下进行访问](/graph/auth-v2-service)。 更新已登录用户的照片仅需要 User.ReadWrite 权限。

> **注意：** 当前有一个 [已知问题](/graph/known-issues#groups)，即使用应用程序权限访问组照片。

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

若要更新团队的照片，请：

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
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
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


