---
title: embeddedSIMDeviceState 资源类型
description: 描述与设备相关的嵌入的 SIM 激活代码部署状态。
author: tfitzmac
ms.openlocfilehash: ef7611e96b1b6f3bba0a3c59dead85ede41b2eda
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308454"
---
# <a name="embeddedsimdevicestate-resource-type"></a>embeddedSIMDeviceState 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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
|id|字符串|嵌入 SIM 设备状态的唯一标识符。 系统生成时创建分配值。|
|createdDateTime|DateTimeOffset|创建嵌入的 SIM 设备状态的时间。 生成的服务方。|
|modifiedDateTime|DateTimeOffset|上次修改嵌入的 SIM 设备状态的时间。 更新服务端。|
|lastSyncDateTime|DateTimeOffset|嵌入的 SIM 设备上次签入的时间。 更新服务端。|
|universalIntegratedCircuitCardIdentifier|字符串|通用集成电路卡标识符 (UICCID) 标识到配置文件是要部署的硬件。|
|deviceName|String|订阅已的设备名称设置如桌面 JOE|
|userName|String|订阅已设置到例如 joe@contoso.com 用户名|
|状态|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|应用于该设备配置文件操作的状态。 可取值为：`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser`。|
|stateDetails|字符串|字符串设置状态的说明。|

## <a name="relationships"></a>Relationships
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





