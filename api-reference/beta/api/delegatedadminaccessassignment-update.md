---
title: 更新 delegatedAdminAccessAssignment
description: 更新 delegatedAdminAccessAssignment 对象的属性。
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 52bee21df148af0bd02bb6a72d52d7c24db3c75f
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589622"
---
# <a name="update-delegatedadminaccessassignment"></a>更新 delegatedAdminAccessAssignment
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [delegatedAdminAccessAssignment 对象](../resources/delegatedadminaccessassignment.md) 的属性。

## <a name="permissions"></a>Permissions
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
|If-Match|If-match：etag}。 要更新的 **delegatedAdminAccessAssignment 的** 上次已知 ETag 值。 必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|属性|类型|说明|
|:---|:---|:---|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|合作伙伴在客户租户中分配的管理角色的标识符|


## <a name="response"></a>响应

如果成功，此方法返回 或 `200 OK` 响应 `202 Accepted` 代码。

## <a name="response-headers"></a>响应标头
|名称|说明|
|:---|:---|
|Content-Type|application/json.|
|位置|长时间运行的操作的位置。|
|Retry-After|之后对位置 URL 进行后续 API 调用以检查长时间运行的操作的状态的时间。|

此方法通常返回响应 `202 Accepted` 代码，该响应代码的 URL 指向 **Location** 响应标头中长时间运行的操作，该响应标头可监视其完成情况。 如果在调用中指定的值与现有对象中的值相同，API `200 OK` 将返回响应代码，响应正文中具有原始 [delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
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

### <a name="response"></a>响应
下面是返回 响应代码以及 `202 Accepted` **Location** 和 **Retry-After** 标头的示例响应。
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