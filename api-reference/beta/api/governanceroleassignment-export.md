---
title: 导出 governanceRoleAssignmentRequests
description: 检索格式为 的 governanceRoleAssignmentRequests 集合，该集合可在浏览器中.csv `application/octet-stream` 文件的形式进行分析。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8faff2bbd4b41eda693467b55641204cb6bbaef3
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350843"
---
# <a name="export-governanceroleassignmentrequests"></a>导出 governanceRoleAssignmentRequests

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索格式为 [的 governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) 集合，该集合可在浏览器中.csv `application/octet-stream` 文件的形式进行分析。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。

### <a name="azure-resources"></a>Azure 资源

| 权限类型 | 权限 |
|:--------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureResources |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application | PrivilegedAccess.Read.AzureResources |

### <a name="azure-ad"></a>Azure AD

| 权限类型 | 权限 |
|:--------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureAD |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application | PrivilegedAccess.Read.AzureAD |

### <a name="groups"></a>组

|权限类型 | 权限 |
|:-------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureADGroup |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application | PrivilegedAccess.Read.AzureADGroup |


## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
导出资源上的 [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) 集合
    
>**注意：** 除了权限范围之外，此请求要求请求者至少具有一角色分配资源访问权限。 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

导出 mine 的 [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) 集合
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法返回 响应 `200 OK` 代码和类型 的内容 `application/octet-stream` 。

## <a name="example"></a>示例
本示例将订阅 Wingtip Toys - Prod .csv所有角色分配另存为一个角色分配文件。 

##### <a name="request"></a>请求
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a>响应
下面是一个响应示例。 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


