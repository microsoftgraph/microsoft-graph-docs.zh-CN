---
title: hardwareConfigurationDeviceState 资源类型
description: 包含硬件配置的设备运行状态的属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4700f48823a54bba155841b492e5ff139f05e235
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345421"
---
# <a name="hardwareconfigurationdevicestate-resource-type"></a>hardwareConfigurationDeviceState 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含硬件配置的设备运行状态的属性

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 hardwareConfigurationDeviceStates](../api/intune-deviceconfig-hardwareconfigurationdevicestate-list.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) 集合|列出 [hardwareConfigurationDeviceState 对象的属性和](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) 关系。|
|[获取 hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-get.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|读取 [hardwareConfigurationDeviceState 对象的属性和](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) 关系。|
|[创建 hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-create.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|创建新的 [hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) 对象。|
|[删除 hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-delete.md)|None|删除 [hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)。|
|[更新 hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-update.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|更新 [hardwareConfigurationDeviceState 对象](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|硬件配置脚本设备状态实体的键。 此属性是只读的。|
|deviceName|String|设备名称|
|osVersion|String|设备的操作系统版本。|
|upn|String|用户主体名称 (UPN)。|
|internalVersion|Int32|策略内部版本|
|lastStateUpdateDateTime|DateTimeOffset|执行硬件配置的最后时间戳|
|configurationState|[runState](../resources/intune-shared-runstate.md)|上次执行硬件配置后的配置状态。 可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。|
|configurationOutput|String|硬件配置执行的输出|
|configurationError|String|硬件配置执行中的错误|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfigurationDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfigurationDeviceState",
  "id": "String (identifier)",
  "deviceName": "String",
  "osVersion": "String",
  "upn": "String",
  "internalVersion": 1024,
  "lastStateUpdateDateTime": "String (timestamp)",
  "configurationState": "String",
  "configurationOutput": "String",
  "configurationError": "String"
}
```




