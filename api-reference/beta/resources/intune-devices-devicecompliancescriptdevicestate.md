---
title: deviceComplianceScriptDeviceState 资源类型
description: 包含设备合规性脚本的设备运行状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f5a24e00f5332231fb77439d82b7a7d57d1a749d4c838173faa1cef689640dc6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145332"
---
# <a name="devicecompliancescriptdevicestate-resource-type"></a>deviceComplianceScriptDeviceState 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含设备合规性脚本的设备运行状态的属性。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceComplianceScriptDeviceStates](../api/intune-devices-devicecompliancescriptdevicestate-list.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 集合|列出 [deviceComplianceScriptDeviceState 对象的属性和](../resources/intune-devices-devicecompliancescriptdevicestate.md) 关系。|
|[获取 deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-get.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|读取 [deviceComplianceScriptDeviceState 对象的属性和](../resources/intune-devices-devicecompliancescriptdevicestate.md) 关系。|
|[创建 deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-create.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|创建新的 [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 对象。|
|[删除 deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-delete.md)|无|删除 [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)。|
|[更新 deviceComplianceScriptDeviceState](../api/intune-devices-devicecompliancescriptdevicestate-update.md)|[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|更新 [deviceComplianceScriptDeviceState 对象](../resources/intune-devices-devicecompliancescriptdevicestate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备合规性脚本设备状态实体的键。 此属性是只读的。|
|detectionState|[runState](../resources/intune-shared-runstate.md)|最近一次执行设备合规性脚本的检测状态。 可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。|
|lastStateUpdateDateTime|DateTimeOffset|执行设备合规性脚本的最后时间戳|
|expectedStateUpdateDateTime|DateTimeOffset|下一次执行设备合规性脚本的时间戳|
|lastSyncDateTime|DateTimeOffset|Intune 管理扩展上次与 Intune 同步的时间|
|scriptOutput|字符串|检测脚本的输出|
|scriptError|String|检测脚本中的错误|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md)|执行设备合规性脚本的托管设备|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
  "id": "String (identifier)",
  "detectionState": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "expectedStateUpdateDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "scriptOutput": "String",
  "scriptError": "String"
}
```




