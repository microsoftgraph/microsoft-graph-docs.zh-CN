---
title: deviceManagementIntent 资源类型
description: 表示将设置应用于设备的意图的实体
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2de7d4e8c177317aa220d6aafbba4bda8b7fe299
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541855"
---
# <a name="devicemanagementintent-resource-type"></a>deviceManagementIntent 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示将设置应用于设备的意图的实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementIntents](../api/intune-deviceintent-devicemanagementintent-list.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)集合|列出[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象的属性和关系。|
|[获取 deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-get.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|读取[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象的属性和关系。|
|[创建 deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-create.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|创建新的[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象。|
|[删除 deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-delete.md)|无|删除[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)。|
|[更新 deviceManagementIntent](../api/intune-deviceintent-devicemanagementintent-update.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|更新[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象的属性。|
|[updateSettings 操作](../api/intune-deviceintent-devicemanagementintent-updatesettings.md)|无|尚未记录|
|[分配操作](../api/intune-deviceintent-devicemanagementintent-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|意向 ID|
|displayName|String|用户给定的显示名称|
|description|String|用户提供的说明|
|isAssigned|Boolean|指示是否将意向分配给用户|
|lastModifiedDateTime|DateTimeOffset|上次修改意向的时间|
|templateId|String|创建此目的的模板的 ID (如果有)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|settings|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合|要应用的所有设置的集合|
|categories|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)集合|在意向中设置类别的集合|
|assignments|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)集合|工作分配集合|
|deviceSettingStateSummaries|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)集合|设置及其状态和这些设备的计数, 这些设备属于意向中所有设置的对应状态|
|deviceStates|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)集合|将应用该意向的所有设备的状态的集合|
|userStates|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)集合|将应用此意向的所有用户的状态的集合|
|deviceStateSummary|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|属于应用此目的的所有设备的对应状态的设备状态和设备计数的摘要|
|userStateSummary|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|用户状态和用户计数的摘要, 这些用户属于应用该意向的所有用户的相应状态|

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
  "templateId": "String"
}
```





