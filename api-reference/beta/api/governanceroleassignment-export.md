---
title: 导出 governanceRoleAssignmentRequests
description: 以格式`application/octet-stream`检索 governanceRoleAssignmentRequests 的集合, 可以在浏览器中将其解析为 .csv 文件。
localization_priority: Normal
ms.openlocfilehash: 454df89b014d3f8e0ed9a80d48b0ba7d97c29558
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422401"
---
# <a name="export-governanceroleassignmentrequests"></a>导出 governanceRoleAssignmentRequests

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

以格式`application/octet-stream`检索[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)的集合, 可以在浏览器中将其解析为 .csv 文件。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | PrivilegedAccess AzureResources  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |


## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
导出资源的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)集合
    
>**注意:** 除了权限范围之外, 此请求还要求请求者在资源上至少有一个角色分配。 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

导出地雷的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)集合
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
如果成功, 此方法将`200 OK`返回响应代码和类型`application/octet-stream`的内容。

## <a name="example"></a>示例
本示例将所有角色分配作为 .csv 文件保存在订阅 Wingtip 玩具-生产中。 

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
