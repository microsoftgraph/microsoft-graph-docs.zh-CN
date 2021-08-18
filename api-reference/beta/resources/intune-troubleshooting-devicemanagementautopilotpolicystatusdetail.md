---
title: deviceManagementAutopilotPolicyStatusDetail 资源类型
description: Autopilot 事件包含的策略状态详细信息项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3cacc18dae925f6c95333693b2bf928b1f466f28
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264351"
---
# <a name="devicemanagementautopilotpolicystatusdetail-resource-type"></a>deviceManagementAutopilotPolicyStatusDetail 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Autopilot 事件包含的策略状态详细信息项。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementAutopilotPolicyStatusDetails](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-list.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) 集合|列出 [deviceManagementAutopilotPolicyStatusDetail 对象的属性和](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) 关系。|
|[获取 deviceManagementAutopilotPolicyStatusDetail](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-get.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|读取 [deviceManagementAutopilotPolicyStatusDetail 对象的属性和](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) 关系。|
|[创建 deviceManagementAutopilotPolicyStatusDetail](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-create.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|创建新的 [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) 对象。|
|[删除 deviceManagementAutopilotPolicyStatusDetail](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-delete.md)|无|删除 [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)。|
|[更新 deviceManagementAutopilotPolicyStatusDetail](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-update.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|更新 [deviceManagementAutopilotPolicyStatusDetail 对象](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID|
|displayName|字符串|策略的友好名称。|
|policyType|[deviceManagementAutopilotPolicyType](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|策略的类型。 可取值为：`unknown`、`application`、`appModel`、`configurationPolicy`。|
|complianceStatus|[deviceManagementAutopilotPolicyComplianceStatus](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|策略合规性状态。 可取值为：`unknown`、`compliant`、`installed`、`notCompliant`、`notInstalled`、`error`。|
|trackedOnEnrollmentStatus|布尔值|指示此许可证是否作为 autopilot 启动注册同步会话的一部分进行跟踪|
|lastReportedDateTime|DateTimeOffset|报告的策略状态的时间戳|
|errorCode|Int32|与策略的合规性或强制状态相关联的错误模式。 强制状态的错误代码如果存在，则优先。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementAutopilotPolicyStatusDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "id": "String (identifier)",
  "displayName": "String",
  "policyType": "String",
  "complianceStatus": "String",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "String (timestamp)",
  "errorCode": 1024
}
```




