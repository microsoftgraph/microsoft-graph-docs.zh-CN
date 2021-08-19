---
title: deviceHealthScriptDeviceState 资源类型
description: 包含设备运行状况脚本的设备运行状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e80f47a2daa68bffb8d90c536bf066ad0b1a303d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58256078"
---
# <a name="devicehealthscriptdevicestate-resource-type"></a>deviceHealthScriptDeviceState 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含设备运行状况脚本的设备运行状态的属性。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceHealthScriptDeviceStates](../api/intune-devices-devicehealthscriptdevicestate-list.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 集合|列出 [deviceHealthScriptDeviceState 对象的属性和](../resources/intune-devices-devicehealthscriptdevicestate.md) 关系。|
|[获取 deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-get.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|读取 [deviceHealthScriptDeviceState 对象的属性和](../resources/intune-devices-devicehealthscriptdevicestate.md) 关系。|
|[创建 deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-create.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|创建新的 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 对象。|
|[删除 deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-delete.md)|无|删除 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)。|
|[更新 deviceHealthScriptDeviceState](../api/intune-devices-devicehealthscriptdevicestate-update.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|更新 [deviceHealthScriptDeviceState 对象](../resources/intune-devices-devicehealthscriptdevicestate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备运行状况脚本设备状态实体的键。 此属性是只读的。|
|detectionState|[runState](../resources/intune-devices-runstate.md)|最近一次执行设备运行状况脚本的检测状态。 可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。|
|lastStateUpdateDateTime|DateTimeOffset|执行设备运行状况脚本的最后时间戳|
|expectedStateUpdateDateTime|DateTimeOffset|预计执行设备运行状况脚本的下一个时间戳|
|lastSyncDateTime|DateTimeOffset|Intune 管理扩展上次与 Intune 同步的时间|
|preRemediationDetectionScriptOutput|字符串|修正前检测脚本的输出|
|preRemediationDetectionScriptError|字符串|修正前检测脚本的错误|
|remediationScriptError|String|修正脚本的错误输出|
|postRemediationDetectionScriptOutput|String|修正后检测脚本输出|
|postRemediationDetectionScriptError|String|修正后检测脚本中的错误|
|remediationState|[remediationState](../resources/intune-devices-remediationstate.md)|自上次设备运行状况脚本执行以来的修正状态。 可取值为：`unknown`、`skipped`、`success`、`remediationFailed`、`scriptError`。|
|assignmentFilterIds|String collection|用于运行状况脚本适用性评估的分配筛选器 ID 的列表|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md)|执行设备运行状况脚本的托管设备|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "id": "String (identifier)",
  "detectionState": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "expectedStateUpdateDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "preRemediationDetectionScriptOutput": "String",
  "preRemediationDetectionScriptError": "String",
  "remediationScriptError": "String",
  "postRemediationDetectionScriptOutput": "String",
  "postRemediationDetectionScriptError": "String",
  "remediationState": "String",
  "assignmentFilterIds": [
    "String"
  ]
}
```




