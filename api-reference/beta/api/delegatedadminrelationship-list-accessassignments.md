---
title: 列出 accessAssignments
description: 获取 delegatedAdminAccessAssignment 对象及其属性的列表。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: 32b79e4a42cb7b781ad3bc698222c2202e09d6db
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211960"
---
# <a name="list-accessassignments"></a>列出 accessAssignments
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) 对象及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| DelegatedAdminRelationship.Read.All、DelegatedAdminRelationship.ReadWrite.All |
|委派（个人 Microsoft 帐户）| 不支持。 |
|Application| 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}/accessAssignments
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select`[OData](/graph/query-parameters) `$filter``$orderBy``$top`查询参数，`$count``$skipToken`以帮助自定义响应。  

`$top` 最多支持 300 个对象。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) 对象的集合。

每个 **delegatedAdminAccessAssignment** 对象都包含根据 RFC2616 的 **@odata.etag** 属性。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_delegatedadminaccessassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/72a7ae7e-4887-4e34-9755-2e1e9b26b943-63f017cb-9e0d-4f14-94bd-4871902b3409/accessAssignments
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-delegatedadminaccessassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-delegatedadminaccessassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-delegatedadminaccessassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-delegatedadminaccessassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-delegatedadminaccessassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.delegatedAdminAccessAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#accessAssignments",
  "value": [
    {
      "@odata.type": "#microsoft.graph.delegatedAdminAccessAssignment",
      "@odata.etag": "W/\"JyIwMDAwMDI5OC0wMDAwLTAyMDAtMDAwMC02MjJiZTA0YjAwMDAiJw==\"",
      "id": "84c586df-0943-416e-b95f-7289cb8d3bd5",
      "status": "active",
      "createdDateTime": "2022-03-07T22:55:18.6780449Z",
      "lastModifiedDateTime": "2022-03-11T23:50:35.8970153Z",
      "accessContainer": {
          "accessContainerId": "227a2f44-2682-4831-a021-f8d69a34bcba",
          "accessContainerType": "securityGroup"
      },
      "accessDetails": {
          "unifiedRoles": [
              {
                   "roleDefinitionId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
              },
              {
                  "roleDefinitionId": "44367163-eba1-44c3-98af-f5787879f96a"
              },
              {
                  "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de"
              },
              {
                  "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
              }
          ]
      }
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminAccessAssignment",
      "@odata.etag": "W/\"JyIwMDAwMjAwOC0wMDAwLTAyMDAtMDAwMC02MjJhYWQzYjAwMDAiJw==\"",
      "id": "8d56bce3-440f-4b4f-b5c2-cc0bcbd0199c",
      "status": "active",
      "createdDateTime": "2022-03-10T23:50:35.8970153Z",
      "lastModifiedDateTime": "2022-03-11T02:00:27.7912161Z",
      "accessContainer": {
          "accessContainerId": "869713c9-0b28-4d08-8949-ae07ae1bf528",
          "accessContainerType": "securityGroup"
      },
      "accessDetails": {
          "unifiedRoles": [
              {
                  "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de"
              },
              {
                  "roleDefinitionId": "f2ef992c-3afb-46b9-b7cf-a126ee74c451"
              },
              {
                  "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8"
              },
              {
                  "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5"
              }
          ]
      }
    }
  ]
}
```

