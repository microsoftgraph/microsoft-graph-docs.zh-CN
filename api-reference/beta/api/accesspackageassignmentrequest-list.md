---
title: 列出 accessPackageAssignmentRequests
description: 检索 accessPackageAssignmentRequest 对象的列表。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c6a111f65195b109bc786719de1f8946d59c6674
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983456"
---
# <a name="list-accesspackageassignmentrequests"></a>列出 accessPackageAssignmentRequests

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD中](../resources/entitlementmanagement-root.md)，检索[accessPackageAssignmentRequest 对象](../resources/accesspackageassignmentrequest.md)的列表。  生成的列表包括调用方有权访问的所有目录和访问包中当前和过期的所有分配请求。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 `$expand` 和 `$filter` OData 查询参数来帮助自定义响应。 例如，若要检索每个请求的访问包，请包括在 `$expand=accessPackage` 查询中。  若要仅检索特定访问包的请求，在查询中包括筛选器（如 `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'` ）。  若要检索结果分配，请包括在 `$expand=accessPackageAssignment` 查询中。  若要获取有关请求程序的详细信息，请包含 `$expand=requestor` 到查询中。
若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。 请求 URI 包括仅返回特定状态的请求，以及返回请求者 `$filter` `$expand` 及其已连接组织的详细信息。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests?$expand=requestor($expand=connectedOrganization)&$filter=(requestState eq 'PendingApproval')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-accesspackageassignmentrequests-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "433dafca-5047-4614-95f7-a03510b1ded3",
      "requestType": "UserAdd",
      "requestState": "PendingApproval",
      "createdDateTime": "2019-10-25T22:55:11.623Z",
      "justification": "Need access",
      "answers": [],
      "requestor": {
        "connectedOrganizationId": "c3c2adbc-a863-437f-9383-ee578665317d",
        "id": "ba7ef0fb-e16f-474b-87aa-02815d061e67",
        "displayName": "displayname",
        "email": "displayname@example.com",
        "type": "User",
        "connectedOrganization": {
          "id": "c3c2adbc-a863-437f-9383-ee578665317d",
          "displayName": "example"
        }
      }
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

