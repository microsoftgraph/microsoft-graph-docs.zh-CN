---
title: embeddedSIMDeviceState 资源类型
description: 描述与设备相关的嵌入的 SIM 激活代码部署状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a79453c8d8bcb5682da64ce480f1a2f9f210a673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415570"
---
# <a name="embeddedsimdevicestate-resource-type"></a>embeddedSIMDeviceState 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述与设备相关的嵌入的 SIM 激活代码部署状态。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 embeddedSIMDeviceStates](../api/intune-esim-embeddedsimdevicestate-list.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)集合|列出属性和[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象之间的关系。|
|[获取 embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-get.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|读取属性和[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的关系。|
|[创建 embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-create.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|创建新的[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象。|
|[删除 embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-delete.md)|无|删除[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)。|
|[更新 embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-update.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|更新[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|嵌入 SIM 设备状态的唯一标识符。 系统生成时创建分配值。|
|createdDateTime|DateTimeOffset|创建嵌入的 SIM 设备状态的时间。 生成的服务方。|
|modifiedDateTime|DateTimeOffset|上次修改嵌入的 SIM 设备状态的时间。 更新服务端。|
|lastSyncDateTime|DateTimeOffset|嵌入的 SIM 设备上次签入的时间。 更新服务端。|
|universalIntegratedCircuitCardIdentifier|String|通用集成电路卡标识符 (UICCID) 标识到配置文件是要部署的硬件。|
|deviceName|String|订阅已的设备名称设置如桌面 JOE|
|userName|String|订阅已设置到例如 joe@contoso.com 用户名|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|应用于该设备配置文件操作的状态。 可取值为：`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser`。|
|stateDetails|String|字符串设置状态的说明。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "universalIntegratedCircuitCardIdentifier": "String",
  "deviceName": "String",
  "userName": "String",
  "state": "String",
  "stateDetails": "String"
}
```




