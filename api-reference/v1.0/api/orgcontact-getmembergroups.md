---
title: orgContact： getMemberGroups
description: 返回组织联系人是成员的所有组。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7fc8f9a62656cace7a4dd3e02182a8a2bc454464
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761644"
---
# <a name="orgcontact-getmembergroups"></a>orgContact： getMemberGroups

命名空间：microsoft.graph

返回组织联系人 [是](../resources/orgcontact.md) 成员的所有组。 检查是可传递的，这和读取 **memberOf** 导航属性不同，后者仅返回用户是其直接成员的组。

此函数支持 Microsoft 365 和 Azure AD (Azure Active Directory 中预配) 。 每个请求可以返回的最大组数为 2046 组。 

>[!NOTE]
>Microsoft 365 组不能包含组。 Microsoft 365 组的成员身份始终是直接的。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | OrgContact.Read.All 和 Group.Read.All、Directory.Read.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | OrgContact.Read.All 和 Group.Read.All、Directory.Read.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:----------|
| Authorization  |  Bearer {token}。必需。 |
| Content-type   | application/json. Required. |

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
  "name": "orgcontact_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmembergroups-java-snippets.md)]
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
Content-length: 39

{
  "value": [
    "groupId-value1",
    "groupId-value2"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

