---
title: 获取 accessPackageAssignmentRequest
description: 检索 accessPackageAssignmentRequest 对象的属性和关系。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4955330fe99df4613cc4d24fb5175db84146cf90
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242373"
---
# <a name="get-accesspackageassignmentrequest"></a>获取 accessPackageAssignmentRequest

命名空间：microsoft.graph


在[Azure AD中](../resources/entitlementmanagement-root.md)，检索[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象的属性和关系。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All  |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/assignmentRequests/{accessPackageAssignmentRequestId}
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 `$expand` OData 查询参数扩展关系，以检索 和 `accessPackage` `requestor` `acccessPackageAssignment` 。  例如，若要检索访问包分配的目标，请包括在 `$expand=accessPackageAssignment($expand=target)` 查询中。  若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentRequests/{accessPackageAssignmentRequestId}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "7999249e-249e-7999-9e24-99799e249979",
  "requestType": "adminAdd",
  "state": "delivered",
  "status": "Delivered",
  "createdDateTime": "2019-10-25T22:55:11.623Z",
  "completedDate": "2019-10-26T22:55:11.623Z",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```


