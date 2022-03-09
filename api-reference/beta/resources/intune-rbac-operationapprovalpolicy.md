---
title: operationApprovalPolicy 资源类型
description: 操作审批策略
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8bcee20030f654ff17f0ebba28ba199dbbe1a7c
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367901"
---
# <a name="operationapprovalpolicy-resource-type"></a>operationApprovalPolicy 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

操作审批策略

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[List operationApprovalPolicies](../api/intune-rbac-operationapprovalpolicy-list.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) 集合|列出 [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) 对象的属性和关系。|
|[获取 operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-get.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|读取 [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) 对象的属性和关系。|
|[创建 operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-create.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|创建新的 [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) 对象。|
|[删除 operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-delete.md)|无|删除 [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)。|
|[Update operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-update.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|更新 [operationApprovalPolicy 对象](../resources/intune-rbac-operationapprovalpolicy.md) 的属性。|
|[getOperationsAllowedApproval 函数](../api/intune-rbac-operationapprovalpolicy-getoperationsallowedapproval.md)|[operationApprovalPolicySet](../resources/intune-rbac-operationapprovalpolicyset.md) 集合|尚未记录|
|[getOperationsRequiringApproval 函数](../api/intune-rbac-operationapprovalpolicy-getoperationsrequiringapproval.md)|[operationApprovalPolicySet](../resources/intune-rbac-operationapprovalpolicyset.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|OperationApprovalPolicy 的 ID。 此属性是只读的。|
|displayName|String|OperationApprovalPolicy 显示名称|
|说明|String|此 OperationApprovalPolicy 的说明|
|lastModifiedDateTime|DateTimeOffset|此 OperationApprovalPolicy 的上次修改日期和时间。 此属性是只读的。|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|此 OperationApprovalPolicy 的策略类型。 可能的值是：、`deviceActions`、`deviceRetire``deviceWipe`、`deviceRetireNonCompliant`、、`deviceDelete`、`deviceLock`、、`windowsEnrollment``deviceResetPasscode``scripts``unknownFutureValue``roles``apps``endpointSecurity``filters``appProtectionPolicies``compliancePolicies``policySets``deviceErase``deviceDisableActivationLock``configurationPolicies`。|
|approverGroupIds|字符串集合|此 OperationApprovalPolicy 的审批者组 ID|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.operationApprovalPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operationApprovalPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "policyType": "String",
  "approverGroupIds": [
    "String"
  ]
}
```




