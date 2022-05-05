---
title: 更新 delegatedAdminAccessAssignment
description: 更新 delegatedAdminAccessAssignment 对象的属性。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: 4cd761bee3a41033804e16840e27b60a3f4928aa
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202389"
---
# <a name="update-delegatedadminaccessassignment"></a>更新 delegatedAdminAccessAssignment
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) 对象的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| DelegatedAdminRelationship.ReadWrite.All |
|委派（个人 Microsoft 帐户）| 不支持。 |
|Application| 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}/accessAssignments/{delegatedAdminAccessAssignmentId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|If-Match|If-match：etag}。 要更新 **的 delegatedAdminAccessAssignment** 的最后一个已知 ETag 值。 必填。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|属性|类型|说明|
|:---|:---|:---|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|合作伙伴在客户租户中分配的管理角色的标识符|


## <a name="response"></a>响应

如果成功，此方法将返回一个 `200 OK` 或一个 `202 Accepted` 响应代码。

## <a name="response-headers"></a>响应标头
|名称|说明|
|:---|:---|
|Content-Type|application/json.|
|位置|长时间运行的操作的位置。|
|Retry-After|之后可以对位置 URL 进行后续 API 调用，以检查长时间运行的操作的状态。|

此方法通常返回一个 `202 Accepted` 响应代码，其中包含 **位置响应标** 头中长时间运行的操作的 URL，该操作可监视以完成。 如果调用中指定的值与现有对象中的值相同，则 API 将返回响应 `200 OK` 正文中原始 [delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) 对象的响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_delegatedadminaccessassignment",
  "@odata.type": "microsoft.graph.delegatedAdminAccessAssignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5e5594d3-6f82-458b-b567-77db4811f0cd-00000000-0000-0000-0000-000000001234/accessAssignments/da9d6cf90-083a-47dc-ace2-1da98be3f344
If-Match: W/"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw=="
Content-Type: application/json

{
  "accessDetails": {
    "unifiedRoles": [
      {
        "roleDefinitionId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
      },
      {
        "roleDefinitionId": "44367163-eba1-44c3-98af-f5787879f96a"
      },
      {
        "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8"
      }
    ]
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-delegatedadminaccessassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-delegatedadminaccessassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-delegatedadminaccessassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-delegatedadminaccessassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-delegatedadminaccessassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
下面是返回响应代码以及 **Location** 和 **Retry-After** 标头的示例响应`202 Accepted`。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.delegatedAdminAccessAssignment"
}
-->
``` http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5e5594d3-6f82-458b-b567-77db4811f0cd-00000000-0000-0000-0000-000000001234/operations/d8dbb27b-7fe7-4523-a3df-f766355fe0f2
Retry-After: 10
Content-Type: application/json

{
}
```
