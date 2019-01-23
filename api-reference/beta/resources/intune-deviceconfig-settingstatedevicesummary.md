---
title: settingStateDeviceSummary 资源类型
description: 设置状态的设备合规性策略和配置摘要
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fab849fa44c33996d31ddac15b44c23f8450988d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414835"
---
# <a name="settingstatedevicesummary-resource-type"></a>settingStateDeviceSummary 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设置状态的设备合规性策略和配置摘要

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 settingStateDeviceSummaries](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|列出 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。|
|[获取 settingStateDeviceSummary](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|读取 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。|
|[创建 settingStateDeviceSummary](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。|
|[删除 settingStateDeviceSummary](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|无|删除 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)。|
|[更新 settingStateDeviceSummary](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|settingName|String|设置的名称|
|instancePath|String|设置的 InstancePath 的名称|
|unknownDeviceCount|Int32|设置的设备未知计数|
|notApplicableDeviceCount|Int32|设置的设备不适用计数|
|compliantDeviceCount|Int32|设置的设备符合性计数|
|remediatedDeviceCount|Int32|设置的设备符合性计数|
|nonCompliantDeviceCount|Int32|设置的设备不符合计数|
|errorDeviceCount|Int32|设置的设备错误计数|
|conflictDeviceCount|Int32|设置的设备冲突错误计数|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.settingStateDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "instancePath": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```




