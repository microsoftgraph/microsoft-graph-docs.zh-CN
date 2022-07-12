---
title: settingStateDeviceSummary 资源类型
description: 设置状态的设备合规性策略和配置摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31b751a53383bbc14ebd1dd1644b440df12957be
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734289"
---
# <a name="settingstatedevicesummary-resource-type"></a>settingStateDeviceSummary 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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
|id|字符串|实体的键。|
|settingName|String|设置的名称|
|instancePath|String|设置的 InstancePath 的名称|
|unknownDeviceCount|Int32|设置的设备未知计数|
|notApplicableDeviceCount|Int32|设置的设备不可用计数|
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





