---
title: directoryObject：checkMemberGroups
description: 检查指定组列表中的成员身份，然后从该列表返回这些组
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 836dd80feccf585035f4f51c1ff3135a744b6e7d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022447"
---
# <a name="directoryobject-checkmembergroups"></a>directoryObject：checkMemberGroups

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检查指定组列表中的成员身份，然后从该列表返回指定的用户、组、服务主体或目录对象是其成员的组。 此函数是可传递的。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.ReadBasic.All、User.Read.All、Directory.Read.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | User.Read.All、Directory.Read.All |

下表列出了用于不同方案的权限类型。

| 方案 | 权限 |
|:-|:-|
| 获取已登录用户的组成员身份 | 使用以下权限集之一： <br/> <li> **User.Read** 和 **GroupMember.Read.All** <li>**User.Read** 和 **Group.Read.All** |
| 获取任何用户的组成员身份 | 使用以下权限集之一： <br/> <li> **User.ReadBasic.All** 和 **GroupMember.Read.All** <li>**User.Read.All** 和 **GroupMember.Read.All** <li>**User.ReadBasic.All** 和 **Group.Read.All** <li>**User.Read.All** 和 **Group.Read.All** |
| 获取组的组成员身份 | 使用 **GroupMember.Read.All 或** **Group.Read.All** 权限。 |
| 获取服务主体的组成员身份 | 使用以下权限集之一 <br/> <li>**Application.ReadWrite.All** 和 **GroupMember.Read.All** <li>**Application.ReadWrite.All** 和 **Group.Read.All** |
| 获取目录对象的组成员身份 | 使用 **Directory.Read.All** 权限。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servicePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a>请求标头

| 名称       |说明|
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。 |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|groupIds|String collection |包含检查成员身份的组中的对象 ID 的集合。可以指定多达 20 个组。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。

## <a name="example"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/directoryobject-checkmembergroups-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


