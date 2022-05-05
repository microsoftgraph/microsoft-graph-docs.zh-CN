---
title: 列出 assignmentPolicies
description: 列出 accessPackageAssignmentPolicy 对象。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f5a6776ac699e35aa21419d1fa2f1baf018e2ced
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209684"
---
# <a name="list-assignmentpolicies"></a>列出 assignmentPolicies
命名空间：microsoft.graph

在[Azure AD权利管理](../resources/entitlementmanagement-overview.md)中，检索 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象的列表。 如果委派的用户处于目录角色中，则生成的列表包括调用方有权在所有目录和访问包中读取的所有分配策略。 如果委派的用户是访问包管理器或目录所有者，则应检索可以使用 [列表 accessPackage（](entitlementmanagement-list-accesspackages.md) 包括 `$expand=accessPackageAssignmentPolicies` 为查询参数）读取的访问包的策略。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |


## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/assignmentPolicies
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持某些 `$filter``$select`OData 查询参数，`$expand`以帮助自定义响应。 例如，若要检索具有指定显示名称的访问包分配策略，请包含 `$filter=displayName eq 'Employee sales support'` 在查询中。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accesspackageassignmentpolicy"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentPolicies
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accesspackageassignmentpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accesspackageassignmentpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-accesspackageassignmentpolicy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
      "displayName": "All Users",
      "description": "All users can request for access to the directory."
    }
  ]
}
```


