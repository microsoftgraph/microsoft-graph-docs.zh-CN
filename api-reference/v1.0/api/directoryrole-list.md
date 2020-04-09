---
title: 列出 directoryRoles
description: 列出租户中激活的目录角色。
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f4a8f8838d77c9a947c304ee18898832c1d5428
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181397"
---
# <a name="list-directoryroles"></a>列出 directoryRoles

命名空间：microsoft.graph

列出租户中激活的目录角色。

此操作仅返回已激活的角色。 当管理员使用[激活 directoryRole](directoryrole-post-directoryroles.md) API 激活角色时，角色即被激活。 最初并不激活所有内置角色。 

使用 Azure 门户分配角色时，将代表管理员隐式完成角色激活步骤。 若要获取 Azure AD 中可用角色的完整列表，请使用[List directoryroletemplate](directoryroletemplate-list.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法**不**支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。

## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:-----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和[directoryRole](../resources/directoryrole.md)对象集合。
## <a name="example"></a>示例
##### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
