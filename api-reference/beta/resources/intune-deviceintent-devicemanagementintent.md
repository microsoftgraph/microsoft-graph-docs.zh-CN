---
title: deviceManagementIntent 资源类型
description: 表示将设置应用到设备的意图的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0e3750a6bfaec140231d680560ad63c89f2f1de759378a5d3748571a701edcd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54219869"
---
# <a name="devicemanagementintent-resource-type"></a>deviceManagementIntent 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示将设置应用到设备的意图的实体

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementIntents](../api/intune-deviceintent-devicemanagementintent-list.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) 集合|列出 [deviceManagementIntent 对象的属性和](../resources/intune-deviceintent-devicemanagementintent.md) 关系。|
|[获取 deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-get.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|读取 [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) 对象的属性和关系。|
|[创建 deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-create.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|创建新的 [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) 对象。|
|[删除 deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-delete.md)|无|删除 [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)。|
|[更新 deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-update.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|更新 [deviceManagementIntent 对象](../resources/intune-deviceintent-devicemanagementintent.md) 的属性。|
|[updateSettings 操作](../api/intune-deviceintent-devicemanagementintent-updatesettings.md)|无|尚未记录|
|[migrateToTemplate 操作](../api/intune-deviceintent-devicemanagementintent-migratetotemplate.md)|无|尚未记录|
|[createCopy 操作](../api/intune-deviceintent-devicemanagementintent-createcopy.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|尚未记录|
|[分配操作](../api/intune-deviceintent-devicemanagementintent-assign.md)|无|尚未记录|
|[compare 函数](../api/intune-deviceintent-devicemanagementintent-compare.md)|[deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|意图 ID|
|displayName|String|给定用户显示名称|
|description|String|用户给定的说明|
|isAssigned|Boolean|表示是否将意图分配给用户|
|lastModifiedDateTime|DateTimeOffset|上次修改意图时|
|templateId|字符串|此意图的模板 ID 是 (（如果有) |
|roleScopeTagIds|String collection|此实体实例的范围标记列表。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|设置|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) 集合|要应用的所有设置的集合|
|categories|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) 集合|意图中的设置类别集合|
|assignments|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) 集合|工作分配集合|
|deviceSettingStateSummaries|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) 集合|属于意图中所有设置的相应状态的设备集合及其状态和计数|
|deviceStates|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) 集合|意图应用于的所有设备状态的集合|
|userStates|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) 集合|意图应用于的所有用户状态的集合|
|deviceStateSummary|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|属于适用意图的所有设备的对应状态的设备状态和计数的摘要|
|userStateSummary|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|用户状态摘要和用户计数，这些用户属于将意图应用于的所有用户的相应状态|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isAssigned": true,
  "lastModifiedDateTime": "String (timestamp)",
  "templateId": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```




