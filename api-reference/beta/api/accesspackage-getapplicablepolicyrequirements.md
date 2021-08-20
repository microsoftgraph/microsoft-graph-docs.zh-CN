---
title: accessPackage： getApplicablePolicyRequirements
description: 允许调用方查找请求特定 accessPackage 的分配的要求。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2572239463e9ab1142c2b5e475f25e7ce1914b39
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259271"
---
# <a name="accesspackage-getapplicablepolicyrequirements"></a>accessPackage： getApplicablePolicyRequirements
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD 权利](../resources/entitlementmanagement-root.md)管理中，此操作检索当前登录用户可以用于创建[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)的[accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md)对象列表。  每个要求对象对应于允许当前登录用户请求分配的访问包分配策略。

## <a name="permissions"></a>权限
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
POST /identityGovernance/entitlementManagement/accessPackages/{id}/getApplicablePolicyRequirements
```

## <a name="function-parameters"></a>函数参数

无。

## <a name="request-headers"></a>请求头
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
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/fb449cf8-3a59-4d86-bdfd-a1b7299681de/getApplicablePolicyRequirements
```

### <a name="response"></a>响应
> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentRequestRequirements)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "policyId": "449feb20-7040-499a-ba91-bdfb93ede34b", 
            "policyDisplayName": "Initial Policy", 
            "policyDescription": "Initial Policy", 
            "isApprovalRequired": false, 
            "isApprovalRequiredForExtension": false, 
            "isRequestorJustificationRequired": false, 
            "questions": [], 
            "existingAnswers": [],
            "schedule": []
        }
    ]
}
``` 
