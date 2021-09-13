---
title: embeddedSIMDeviceState 资源类型
description: 描述与设备相关的嵌入式 SIM 卡激活代码部署状态。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0f5b98cbf3d70514b09a18ccd6d9eab7033c862c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039859"
---
# <a name="embeddedsimdevicestate-resource-type"></a>embeddedSIMDeviceState 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述与设备相关的嵌入式 SIM 卡激活代码部署状态。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 embeddedSIMDeviceStates](../api/intune-esim-embeddedsimdevicestate-list.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) 集合|列出 [embeddedSIMDeviceState 对象的属性和](../resources/intune-esim-embeddedsimdevicestate.md) 关系。|
|[获取 embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-get.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|读取 [embeddedSIMDeviceState 对象的属性和](../resources/intune-esim-embeddedsimdevicestate.md) 关系。|
|[创建 embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-create.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|创建新的 [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) 对象。|
|[删除 embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-delete.md)|无|删除嵌入 [的SIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)。|
|[更新 embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-update.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|更新嵌入 [SIMDeviceState 对象](../resources/intune-esim-embeddedsimdevicestate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|嵌入式 SIM 卡设备状态的唯一标识符。 创建时分配的系统生成值。|
|createdDateTime|DateTimeOffset|嵌入式 SIM 卡设备状态的创建时间。 生成的服务器端。|
|modifiedDateTime|DateTimeOffset|上次修改嵌入式 SIM 卡设备状态的时间。 更新的服务器端。|
|lastSyncDateTime|DateTimeOffset|嵌入式 SIM 卡设备上次签入的时间。 更新的服务器端。|
|universalIntegratedCircuitCardIdentifier|String|通用集成电路卡标识符 (UI进行) 标识要部署配置文件的硬件。|
|deviceName|String|预配订阅的设备名称，例如 DESKTOP-JOE|
|userName|String|订阅预配到的用户名，例如 joe@contoso.com|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|应用于设备的配置文件操作的状态。 可取值为：`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser`。|
|stateDetails|String|设置状态字符串说明。|

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



