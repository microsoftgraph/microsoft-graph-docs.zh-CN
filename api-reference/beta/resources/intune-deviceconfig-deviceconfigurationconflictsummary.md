---
title: deviceConfigurationConflictSummary 资源类型
description: 一组设备配置策略的冲突摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8c020e38c030c8b9acfd427b047a9dbf0f37a9093cf3dc570c848499cf41ce72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54241953"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a>deviceConfigurationConflictSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一组设备配置策略的冲突摘要。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceConfigurationConflictSummaries](../api/intune-deviceconfig-deviceconfigurationconflictsummary-list.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) 集合|列出 [deviceConfigurationConflictSummary 对象的属性和](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) 关系。|
|[获取 deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-get.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|读取 [deviceConfigurationConflictSummary 对象的属性和](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) 关系。|
|[创建 deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-create.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|创建新的 [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) 对象。|
|[删除 deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-delete.md)|无|删除 [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)。|
|[更新 deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-update.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|更新 [deviceConfigurationConflictSummary 对象](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|conflictingDeviceConfigurations|[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合|与给定设置相冲突的策略集|
|id|String|这组冲突策略的 ID。 此 id 是 ConflictingDeviceConfigurations 中所有策略的 ID，按字典顺序使用下划线分隔。|
|contributingSettings|String collection|与给定策略相冲突的设置集|
|deviceCheckinsImpacted|Int32|受冲突策略和设置影响的签入计数|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationConflictSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String",
      "sourceType": "String"
    }
  ],
  "id": "String (identifier)",
  "contributingSettings": [
    "String"
  ],
  "deviceCheckinsImpacted": 1024
}
```




