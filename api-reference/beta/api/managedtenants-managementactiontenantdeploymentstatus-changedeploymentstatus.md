---
title: managementActionTenantDeploymentStatus： changeDeploymentStatus
description: 更改管理操作租户级别的部署状态。 此信息用于提供对特定状态中的管理操作的见解。 例如，可能有一个计划对管理员应用需要多重身份验证，因此最好将状态更改为计划状态以反映相应的状态。
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 9be7954a2f1446477470fdf7a89f1e30dfa1e7c5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022051"
---
# <a name="managementactiontenantdeploymentstatus-changedeploymentstatus"></a>managementActionTenantDeploymentStatus： changeDeploymentStatus
命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更改管理操作租户级别的部署状态。 此信息用于提供对特定状态中的管理操作的见解。 例如，可能有一个计划对管理员应用需要多重身份验证，因此最好将状态更改为计划状态以反映相应的状态。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|ManagedTenants.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|:---|:---|:---|
|tenantGroupId|String|租户组的标识符。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。|
|managementActionId|String|管理操作 [的标识符](../resources/managedtenants-managementaction.md)。|
|managementTemplateId|String|管理模板 [的标识符](../resources/managedtenants-managementtemplate.md)。|
|status|String|管理操作租户 [部署的新](../resources/managedtenants-managementaction.md) 状态。|

## <a name="response"></a>响应

如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [managementActionDeploymentStatus。](../resources/managedtenants-managementactiondeploymentstatus.md)

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "managementactiontenantdeploymentstatus_changedeploymentstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
Content-Type: application/json

{
  "tenantGroupId": "String",
  "tenantId": "String",
  "managementActionId": "String",
  "managementTemplateId": "String",
  "status": "String"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/managementactiontenantdeploymentstatus-changedeploymentstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/managementactiontenantdeploymentstatus-changedeploymentstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/managementactiontenantdeploymentstatus-changedeploymentstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/managementactiontenantdeploymentstatus-changedeploymentstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/managementactiontenantdeploymentstatus-changedeploymentstatus-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.managedTenants.ManagementActionDeploymentStatus",
  "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
  "managementActionId": "e96a8cdb-0435-4808-9956-cf6b8ae77aa6",
  "status": "planned",
  "workloadActionDeploymentStatuses": []
}
```
