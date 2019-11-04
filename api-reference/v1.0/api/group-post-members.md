---
title: 添加成员
description: 通过 **members** 导航属性将成员添加到 Office 365 组、安全组或启用邮件的安全组中。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 76213aa84377de6c4d469a61d8287a58d7f76a20
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37934856"
---
# <a name="add-member"></a>添加成员
通过 **members** 导航属性将成员添加到 Office 365 组或安全组中。

可以添加用户、组织联系人或其他组。 

> [!IMPORTANT]
> 仅能将用户添加到 Office 365 组。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.ReadWrite.All 和 Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Content-type   | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md)、[group](../resources/group.md) 或 [organizational contact](../resources/orgcontact.md) 对象的 JSON 表示形式。

## <a name="response"></a>响应
如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例
#### <a name="request"></a>请求
下面展示了示例请求。

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_member_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
