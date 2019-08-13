---
title: deviceManagementScriptDeviceState 资源类型
description: 包含设备管理脚本的设备运行状态的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 86f3dcfefb80765ff13bb8742d88fdd869072f66
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370044"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a>deviceManagementScriptDeviceState 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含设备管理脚本的设备运行状态的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementScriptDeviceStates](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合|列出[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性和关系。|
|[获取 deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|读取[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性和关系。|
|[创建 deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|创建新的[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。|
|[删除 deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|无|删除[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)。|
|[更新 deviceManagementScriptDeviceState](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|更新[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备管理脚本设备状态实体的密钥。|
|runState|[runState](../resources/intune-shared-runstate.md)|设备管理脚本最新运行的状态。 可取值为：`unknown`、`success`、`fail`、`error`、`pending`。|
|resultMessage|String|执行输出的详细信息。|
|lastStateUpdateDateTime|DateTimeOffset|最近执行设备管理脚本的时间。|
|errorCode|Int32|与设备管理脚本的错误执行相对应的错误代码。|
|errorDescription|String|与设备管理脚本的错误执行相对应的错误说明。|
|lastSyncDateTime|DateTimeOffset|Intune 管理扩展将同步到 Intune 的最新时间。|
|preRemediationDetectionScriptOutput|String|修复前的检测脚本输出。|
|remediationScriptError|String|修正脚本的错误输出。|
|postRemediationDetectionScriptOutput|String|修正后的检测脚本输出。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md)|执行设备管理脚本的托管设备。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "String (identifier)",
  "runState": "String",
  "resultMessage": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "errorCode": 1024,
  "errorDescription": "String",
  "lastSyncDateTime": "String (timestamp)",
  "preRemediationDetectionScriptOutput": "String",
  "remediationScriptError": "String",
  "postRemediationDetectionScriptOutput": "String"
}
```



