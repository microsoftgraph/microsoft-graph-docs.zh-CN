---
title: 列出目录角色的 scopedMembers
description: 检索目录角色的 scopedRoleMembership 对象列表。
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d5f915debcdecba1effdf96bae6ae36da0331783
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207697"
---
# <a name="list-scopedmembers-for-a-directory-role"></a>列出目录角色的 scopedMembers

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索目录角色 [的 scopedRoleMembership](../resources/scopedrolemembership.md) 对象列表。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /directoryroles/{role-id}/scopedMembers
GET /directoryroles/roleTemplateId={roleTemplateId}/scopedMembers
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [scopedRoleMembership](../resources/scopedrolemembership.md) 对象集合。
## <a name="examples"></a>示例

### <a name="example-1--get-the-scoped-members-of-a-directory-role-using-role-id"></a>示例 1：使用角色 ID 获取目录角色的作用域成员

#### <a name="request"></a>请求
下面是一个请求目录角色 **ID 的示例** `41d12a2f-caa8-4e3e-ba14-05e5102ce085` 。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/41d12a2f-caa8-4e3e-ba14-05e5102ce085/scopedMembers
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedmembers-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedmembers-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedmembers-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedmembers-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应
以下示例显示了相应的响应。 
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships",
    "value": [
        {
            "id": "LyrRQajKPk66FAXlECzghXFuYtw3SOtAvkq8KdiKEXiTwZeOU-r8RIHrq2vQ4F1wU",
            "roleId": "41d12a2f-caa8-4e3e-ba14-05e5102ce085",
            "administrativeUnitId": "dc626e71-4837-40eb-be4a-bc29d88a1178",
            "roleMemberInfo": {
                "id": "8e97c193-ea53-44fc-81eb-ab6bd0e05d70",
                "displayName": "Adele Vance"
            }
        }
    ]
}
```

### <a name="example-2--get-the-scoped-members-of-a-directory-role-using-roletemplateid"></a>示例 2：使用 roleTemplateId 获取目录角色的作用域成员

#### <a name="request"></a>请求
以下是对 **roleTemplateId** 为 的目录角色的请求示例 `fdd7a751-b60b-444a-984c-02652fe8fa1c` 。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=fdd7a751-b60b-444a-984c-02652fe8fa1c/scopedMembers
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedmembers-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedmembers-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedmembers-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedmembers-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
以下示例显示了相应的响应。 
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships",
    "value": [
        {
            "id": "LyrRQajKPk66FAXlECzghXFuYtw3SOtAvkq8KdiKEXiTwZeOU-r8RIHrq2vQ4F1wU",
            "roleId": "41d12a2f-caa8-4e3e-ba14-05e5102ce085",
            "administrativeUnitId": "dc626e71-4837-40eb-be4a-bc29d88a1178",
            "roleMemberInfo": {
                "id": "8e97c193-ea53-44fc-81eb-ab6bd0e05d70",
                "displayName": "Adele Vance"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedmembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
