---
title: accessPackage： getApplicablePolicyRequirements
description: 允许调用方查找请求特定 accessPackage 的分配的要求。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 525f0079f488d267ad8d16aac249b3f2a8140984
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242333"
---
# <a name="accesspackage-getapplicablepolicyrequirements"></a>accessPackage： getApplicablePolicyRequirements
命名空间：microsoft.graph


在[Azure AD](../resources/entitlementmanagement-root.md)中，此操作检索当前登录用户可以用于创建[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)的[accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md)对象列表。  每个要求对象对应于允许当前登录用户请求分配的访问包分配策略。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackages/{accessPackageId}/getApplicablePolicyRequirements
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md) 集合，对于用户是 **allowedRequestor** 的每个策略，返回一个对象。 如果存在没有要求的策略 **，accessPackageAssignmentRequestRequirements** 将具有 `false` 和 `null` 值。 如果没有用户为 **allowedRequestor** 的策略，将改为返回空集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "accesspackage_getapplicablepolicyrequirements"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackages/{accessPackageId}/getApplicablePolicyRequirements
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentRequestRequirements)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "microsoft.graph.accessPackageAssignmentRequestRequirements"
    }
  ]
}
```


