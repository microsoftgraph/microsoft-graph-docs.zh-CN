---
title: 导出 governanceRoleAssignmentRequests
description: 检索的格式 governanceRoleAssignmentRequests 集合`application/octet-stream`，其中可以解析为浏览器中的.csv 文件。
ms.openlocfilehash: 8b9e64faeb8134f5b0bb964d296b1bab309021d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043312"
---
# <a name="export-governanceroleassignmentrequests"></a>导出 governanceRoleAssignmentRequests

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

检索的格式[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)集合`application/octet-stream`，其中可以解析为浏览器中的.csv 文件。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureResources  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | PrivilegedAccess.ReadWrite.AzureResources |


## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->导出[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)对资源的集合
    
>**注意：** 除了权限范围，该请求需要具有至少一个角色分配对资源的请求程序。 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

导出的我的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)集合
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应代码和内容类型的`application/octet-stream`。

## <a name="example"></a>示例
本示例保存为.csv 文件订阅 Wingtip Toys-prod 移中的所有角色分配。 

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
<!-- {
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
