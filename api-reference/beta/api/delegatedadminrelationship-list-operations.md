---
title: 列举操作
description: 获取 delegatedAdminRelationshipOperation 对象及其属性的列表。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: 782d4cec7ebf4268330c5b23ca1e2b30f1c66a42
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704380"
---
# <a name="list-operations"></a>列举操作
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [delegatedAdminRelationshipOperation](../resources/delegatedadminrelationshipoperation.md) 对象及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| DelegatedAdminRelationship.Read.All、DelegatedAdminRelationship.ReadWrite.All |
|委派（个人 Microsoft 帐户）| 不支持。 |
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}/operations
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$expand`[OData](/graph/query-parameters) `$select``$top``$filter`查询参数，`$count``$skipToken`以帮助自定义响应。  

`$top` 最多支持 300 个对象。

## <a name="request-headers"></a>请求头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [delegatedAdminRelationshipOperation](../resources/delegatedadminrelationshipoperation.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_delegatedadminrelationshipoperation"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836/operations
```

### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.delegatedAdminRelationshipOperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#operations",
  "value": [
    {
      "@odata.type": "#microsoft.graph.delegatedAdminRelationshipOperation",
      "@odata.etag": "W/\"JyIwMzAwZTM0ZS0wMDAwLTAyMDAtMDAwMC02MTRjZjI1YzAwMDAiJw==\"",
      "id": "e7de9158-df46-478e-820c-d6eff099d27b",
      "operationType": "delegatedAdminAccessAssignmentUpdate",
      "data": "{\"id\":\"a97a9b4c-f43e-4c47-bbd6-50d8d3c88d94\",\"accessContainer\":{\"accessContainerId\":\"11cc3849-c298-455f-9a11-b7be350ef352\",\"accessContainerType\":\"securityGroup\"},\"accessDetails\":{\"unifiedRoles\":[{\"roleDefinitionId\":\"f2ef992c-3afb-46b9-b7cf-a126ee74c451\"},{\"roleDefinitionId\":\"62e90394-69f5-4237-9190-012177145e10\"}]},\"status\":\"active\"}",
      "status": "complete",
      "createdDateTime": "2022-02-09T22:17:43.9821847Z",
      "lastModifiedDateTime": "2022-02-09T22:17:43.9821847Z"
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminRelationshipOperation",
      "@odata.etag": "W/\"JyIwMzAwZTM0ZS0wMKMh5TAyMDAtMDAwMC02MTRjZjI1YzAwMDAiJw==\"",
      "id": "f7a7dad4-8cc4-40d7-be44-dd3501b1f4e0",
      "operationType": "delegatedAdminAccessAssignmentUpdate",
      "data": "{\"id\":\"a97a9b4c-f43e-4c47-bbd6-50d8d3c88d94\",\"accessContainer\":{\"accessContainerId\":\"8d56bce3-440f-4b4f-b5c2-cc0bcbd0199c\",\"accessContainerType\":\"securityGroup\"},\"accessDetails\":{\"unifiedRoles\":[{\"roleDefinitionId\":\"29232cdf-9323-42fd-ade2-1d097af3e4de\"},{\"roleDefinitionId\":\"88d8e3e3-8f55-4a1e-953a-9b9898b8876b\"}]},\"status\":\"active\"}",
      "status": "complete",
      "createdDateTime": "2022-02-11T20:32:05.4659288Z",
      "lastModifiedDateTime": "2022-02-11T20:34:42.9202474Z"
    }
  ]
}
```

