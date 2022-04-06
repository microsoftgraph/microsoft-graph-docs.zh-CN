---
title: 创建 assignmentPolicies
description: 创建新的 accessPackageAssignmentPolicy 对象。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 848f259c6d40ae14fb45c9230ad4d0b524dbf17b
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608280"
---
# <a name="create-assignmentpolicies"></a>创建 assignmentPolicies
命名空间：microsoft.graph

在[Azure AD中](../resources/entitlementmanagement-overview.md)，创建新的 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象。  该请求将包括对将包含此策略的 [accessPackage](../resources/accesspackage.md) 的引用，该策略必须已经存在。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.ReadWrite.All  |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | EntitlementManagement.ReadWrite.All |


## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/assignmentPolicies
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象的 JSON 表示形式。

可以在创建 **accessPackageAssignmentPolicy 时指定以下属性**。

|属性|类型|说明|
|:---|:---|:---|
|说明|String|策略的说明。|
|displayName|String|策略显示名称。|
|allowedTargetScope|allowedTargetScope|Who允许通过此策略分配访问包。 可取值包括：`notSpecified`、`specificDirectoryUsers`、`specificConnectedOrganizationUsers`、`specificDirectoryServicePrincipals`、`allMemberUsers`、`allDirectoryUsers`、`allDirectoryServicePrincipals`、`allConfiguredConnectedOrganizationUsers`、`allExternalUsers`、`unknownFutureValue`。 可选。|
|expiration|[expirationPattern](../resources/expirationpattern.md)|在此策略中创建的工作分配的到期日期。|
|requestApprovalSettings|[accessPackageAssignmentApprovalSettings](../resources/accesspackageassignmentapprovalsettings.md)|指定通过此策略审批访问包分配请求的设置。 例如，如果新请求需要审批。|
|requestorSettings|[accessPackageAssignmentRequestorSettings](../resources/accesspackageassignmentrequestorsettings.md)|提供其他设置，以选择谁可以通过此策略创建访问包分配请求，以及可以在请求中包括的内容。|
|specificAllowedTargets|[subjectSet](../resources/subjectset.md) 集合|从此策略的访问包分配访问权限的目标。|
|accessPackage|[accessPackage](../resources/accesspackage.md)| 对将包含策略的访问包的引用，该访问包必须已存在。|

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentPolicies
Content-Type: application/json

{
  "displayName": "New Policy",
  "description": "policy for assignment",
  "allowedTargetScope": "notSpecified",
  "specificAllowedTargets": [],
  "expiration": {
      "endDateTime": null,
      "duration": null,
      "type": "noExpiration"
  },
  "requestorSettings": {
      "enableTargetsToSelfAddAccess": false,
      "enableTargetsToSelfUpdateAccess": false,
      "enableTargetsToSelfRemoveAccess": false,
      "allowCustomAssignmentSchedule": true,
      "enableOnBehalfRequestorsToAddAccess": false,
      "enableOnBehalfRequestorsToUpdateAccess": false,
      "enableOnBehalfRequestorsToRemoveAccess": false,
      "onBehalfRequestors": []
  },
  "requestApprovalSettings": {
      "isApprovalRequiredForAdd": false,
      "isApprovalRequiredForUpdate": false,
      "stages": []
  },
  "accessPackage": {
      "id": "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b"
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
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187",
  "displayName": "New policy",
  "description": "policy for assignment"
}
```


