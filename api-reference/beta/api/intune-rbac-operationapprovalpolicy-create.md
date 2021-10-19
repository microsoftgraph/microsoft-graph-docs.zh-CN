---
title: 创建 operationApprovalPolicy
description: 创建新的 operationApprovalPolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 647ce2fff931c7400cf85cbd2254b6cc0c90120b
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60493178"
---
# <a name="create-operationapprovalpolicy"></a>创建 operationApprovalPolicy

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementRBAC.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/operationApprovalPolicies
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 operationApprovalPolicy 对象的 JSON 表示形式。

下表显示创建 operationApprovalPolicy 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|OperationApprovalPolicy 的 ID。 此属性是只读的。|
|displayName|String|此操作显示名称ApprovalPolicy|
|说明|String|此 OperationApprovalPolicy 的说明|
|lastModifiedDateTime|DateTimeOffset|此 OperationApprovalPolicy 的上次修改日期和时间。 此属性是只读的。|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|此 OperationApprovalPolicy 的策略类型。 可能的值是 `deviceActions` `deviceWipe` `deviceRetire` ：、、、、、、、、 `deviceRetireNonCompliant` `deviceDelete` `deviceLock` `deviceErase` `deviceDisableActivationLock` `windowsEnrollment` `compliancePolicies` `configurationPolicies` `appProtectionPolicies` `policySets` `filters` `endpointSecurity` `apps` `scripts` `roles` `unknownFutureValue` 。|
|policyPlatform|[operationApprovalPolicyPlatform](../resources/intune-rbac-operationapprovalpolicyplatform.md)|适用的平台 (OperationApprovalPolicy) 的一部分。 可取值为：`notApplicable`、`androidDeviceAdministrator`、`androidEnterprise`、`iOSiPadOS`、`macOS`、`windows10AndLater`、`windows81AndLater`、`windows10X`。|
|approverGroupIds|String 集合|此 OperationApprovalPolicy 的审批者组 ID|



## <a name="response"></a>响应
如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/operationApprovalPolicies
Content-type: application/json
Content-length: 289

{
  "@odata.type": "#microsoft.graph.operationApprovalPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "policyType": "deviceWipe",
  "policyPlatform": "androidDeviceAdministrator",
  "approverGroupIds": [
    "Approver Group Ids value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 402

{
  "@odata.type": "#microsoft.graph.operationApprovalPolicy",
  "id": "9d2caa5f-aa5f-9d2c-5faa-2c9d5faa2c9d",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "policyType": "deviceWipe",
  "policyPlatform": "androidDeviceAdministrator",
  "approverGroupIds": [
    "Approver Group Ids value"
  ]
}
```



