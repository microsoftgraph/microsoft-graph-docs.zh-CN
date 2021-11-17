---
title: orgContact： getMemberObjects
description: 返回此组织联系人是成员的所有组。 检查是可传递的。
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a48b9a0a24f7cb0eb130853fdeaa012e5d7e9dc7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992814"
---
# <a name="orgcontact-getmemberobjects"></a>orgContact： getMemberObjects

命名空间：microsoft.graph

返回此组织联系人 [是](../resources/orgcontact.md) 成员的所有组。 检查是可传递的。 组织联系人不能是目录角色的成员。 不会返回任何目录角色。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | OrgContact.Read.All 和 Group.Read.All、Directory.Read.All  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | OrgContact.Read.All 和 Group.Read.All、Directory.Read.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Content-type   | application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|securityEnabledOnly|Boolean|设置为 `false` 。 只支持对用户仅返回启用安全机制的组。|

## <a name="response"></a>响应

如果成功，该运营商将返回 `200 OK` 响应代码和响应正文中的字符串集合对象。

## <a name="example"></a>示例

##### <a name="request"></a>请求
下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/orgcontact-getmemberobjects-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
下面展示了示例响应。
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
    "groupID-value1"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

