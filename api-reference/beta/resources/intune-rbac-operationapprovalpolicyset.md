---
title: operationApprovalPolicySet 资源类型
description: 包含 OperationApprovalPolicyType 和 OperationApprovalPolicyPlatform 对，用于确定用户适用的 OperationApprovalPolicies 集
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d314a9ca5d8f842b7e898ba0ff358241bf996e2f
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340170"
---
# <a name="operationapprovalpolicyset-resource-type"></a>operationApprovalPolicySet 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 OperationApprovalPolicyType 和 OperationApprovalPolicyPlatform 对，用于确定用户适用的 OperationApprovalPolicies 集

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|此 OperationApprovalPolicy 的策略类型。 此属性是只读的。 可能的值是 `deviceActions` `deviceWipe` `deviceRetire` ：、、、、、、、、。 `deviceRetireNonCompliant` `deviceDelete` `deviceLock` `deviceErase` `deviceDisableActivationLock` `windowsEnrollment` `compliancePolicies` `configurationPolicies` `appProtectionPolicies` `policySets` `filters` `endpointSecurity` `apps` `scripts` `roles` `deviceResetPasscode` `unknownFutureValue`|
|policyPlatform|[operationApprovalPolicyPlatform](../resources/intune-rbac-operationapprovalpolicyplatform.md)|适用于此 OperationApprovalPolicy () 一个应用平台。 此属性是只读的。 可取值为：`notApplicable`、`androidDeviceAdministrator`、`androidEnterprise`、`iOSiPadOS`、`macOS`、`windows10AndLater`、`windows81AndLater`、`windows10X`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationApprovalPolicySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operationApprovalPolicySet",
  "policyType": "String",
  "policyPlatform": "String"
}
```




