---
title: 列出 accessPackageAssignments
description: 检索 accesspackageassignment 对象的列表。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f0fe67076195ea044e2dd8bca822192c31664f69
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100975"
---
# <a name="list-assignments"></a>列出作业

命名空间：microsoft.graph

在[Azure AD中](../resources/entitlementmanagement-overview.md)，检索[accessPackageAssignment 对象](../resources/accesspackageassignment.md)的列表。

对于目录范围的管理员，结果列表包括调用方有权访问的所有目录和访问包的所有分配（当前分配和过期分配）。  如果调用方代表仅分配给特定于目录的委派管理角色的委派用户，则请求必须提供筛选器来指示特定访问包，例如 `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` ：。


## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/assignments
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 `$select` 、 `$filter` 和 `$expand` OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

### <a name="example-scenarios-for-using-query-parameters"></a>使用查询参数的示例方案

- 如果调用方代表仅分配给特定于目录的委派管理角色的委派用户，则请求必须提供筛选器来指示特定访问包，例如 `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` ：。
- 若要返回目标主题和访问包，请包含 `$expand=target,accessPackage` 。
- 若要仅检索已传递的工作分配，可以包括查询 `$filter=assignmentState eq 'Delivered'` 。
- 若要仅检索特定用户的工作分配，可以包含一个包含针对该用户的对象 ID 的工作分配的查询 `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` ：。
- 若要仅检索特定用户和特定访问包的工作分配，可以包含包含针对该访问包的工作分配和该用户的对象 ID 的查询 `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` ：。


## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageAssignment](../resources/accesspackageassignment.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accesspackageassignment"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignments
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accesspackageassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accesspackageassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accesspackageassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accesspackageassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accesspackageassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-accesspackageassignment-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "2a353749-3749-2a35-4937-352a4937352a",
      "state": "delivered",
      "status": "Delivered",
      "expiredDateTime": "2019-04-25T23:45:40.42Z",
      "schedule": {
        "@odata.type": "microsoft.graph.entitlementManagementSchedule"
      }
    }
  ]
}
```



