---
title: 更新 accessPackageAssignmentPolicy
description: 更新 accessPackageAssignmentPolicy 对象的属性。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9721e20954105efde2c43be33ec47889884405e7
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608255"
---
# <a name="update-accesspackageassignmentpolicy"></a>更新 accessPackageAssignmentPolicy

命名空间：microsoft.graph


更新现有 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象以更改其一个或多个属性，例如显示名称或说明。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）     | EntitlementManagement.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /identityGovernance/entitlementManagement/assignmentPolicies/{accessPackageAssignmentPolicyId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|策略显示名称。|
|说明|String|策略的说明。|
|allowedTargetScope|allowedTargetScope|Who允许通过此策略请求访问包。 可取值包括：`notSpecified`、`specificDirectoryUsers`、`specificConnectedOrganizationUsers`、`specificDirectoryServicePrincipals`、`allMemberUsers`、`allDirectoryUsers`、`allDirectoryServicePrincipals`、`allConfiguredConnectedOrganizationUsers`、`allExternalUsers`、`unknownFutureValue`。|
|specificAllowedTargets|[subjectSet](../resources/subjectset.md) 集合|可以通过此策略从访问包分配访问权限的主体。|
|expiration|[expirationPattern](../resources/expirationpattern.md)|在此策略中创建的工作分配的到期日期。|
|requestorSettings|[accessPackageAssignmentRequestorSettings](../resources/accesspackageassignmentrequestorsettings.md)|提供其他设置，以选择谁可以通过此策略创建访问包分配请求，以及可以在请求中包括的内容。|
|requestApprovalSettings|[accessPackageAssignmentApprovalSettings](../resources/accesspackageassignmentapprovalsettings.md)|指定通过此策略审批访问包分配请求的设置。 例如，如果新请求需要审批。|
|reviewSettings|[accessPackageReviewSettings](../resources/accesspackageassignmentreviewsettings.md)|设置此策略访问分配评审。|

## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象。



## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignmentpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentPolicies/87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187
Content-Type: application/json

{
  "id":"87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187",
  "displayName": "All Users",
  "description": "All users can request for access to the directory.",
  "accessPackage": {
        "id": "49d2c59b-0a81-463d-a8ec-ddad3935d8a0"
  }
}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187",
  "displayName": "All Users",
  "description": "All users can request for access to the directory."
}
```

