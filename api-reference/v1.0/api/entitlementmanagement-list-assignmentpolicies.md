---
title: 列出 assignmentPolicies
description: 列出 accessPackageAssignmentPolicy 对象。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 82de66f4eac1095374177eff848ea4e6b67d1540
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608253"
---
# <a name="list-assignmentpolicies"></a>列出 assignmentPolicies
命名空间：microsoft.graph

在[Azure AD中](../resources/entitlementmanagement-overview.md)，检索 [accessPackageAssignmentPolicy 对象](../resources/accesspackageassignmentpolicy.md)的列表。 如果委派用户位于目录角色中，则结果列表包括调用方有权访问的所有目录和访问包中读取的所有分配策略。 如果委派的用户是访问包管理器或目录所有者，他们应改为检索他们可以通过列表 [accessPackages](entitlementmanagement-list-accesspackages.md) 读取的访问包的策略，方法为包括 `$expand=accessPackageAssignmentPolicies` 作为查询参数。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |


## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/assignmentPolicies
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 `$filter`、 和 `$select``$expand` OData 查询参数来帮助自定义响应。 例如，若要检索具有指定权限的访问包分配显示名称，请包括在 `$filter=displayName eq 'Employee sales support'` 查询中。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_accesspackageassignmentpolicy"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentPolicies
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
      "displayName": "All Users",
      "description": "All users can request for access to the directory."
    }
  ]
}
```


