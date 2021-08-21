---
title: 获取 governanceRoleAssignmentRequest
description: '获取 governanceRoleAssignmentRequest。 '
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: 3a7fa06029344c3593433ae2ef95119251d60584
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453105"
---
# <a name="get-governanceroleassignmentrequest"></a>获取 governanceRoleAssignmentRequest

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。 

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。

### <a name="azure-resources"></a>Azure 资源

| 权限类型 | 权限 |
|:--------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureResources |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | PrivilegedAccess.Read.AzureResources |

### <a name="azure-ad"></a>Azure AD

| 权限类型 | 权限 |
|:--------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureAD |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | PrivilegedAccess.Read.AzureAD |

### <a name="groups"></a>组

|权限类型 | 权限 |
|:-------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureADGroup |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | PrivilegedAccess.Read.AzureADGroup |

除了权限范围之外，它还需要请求者 
*   至少对资源角色分配一个资源;或
*   是 [governanceRoleAssignmentRequest 的主题](../resources/governanceroleassignmentrequest.md)。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 对象。

## <a name="example"></a>示例
获取角色分配请求
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"e68ff888-4af5-4ccb-8b74-39156090344b",
  "resourceId":"ec3a00f7-81dc-43b3-bbe7-650d3a5f7d46",
  "roleDefinitionId":"be0767b9-2c31-4b0d-b820-726228e7ff5c",
  "subjectId":"a4c5a837-b546-4ec5-a7df-e61547a46a4b",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"2018-05-09T21:26:15.73-07:00",
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


