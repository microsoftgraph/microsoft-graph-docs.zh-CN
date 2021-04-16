---
title: userExperienceAnalyticsWorkFromAnywhereDevice 资源类型
description: 用户体验分析设备：从任何位置工作的报告
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b00e86422989575dd6b30a967861974469aa945c
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868490"
---
# <a name="userexperienceanalyticsworkfromanywheredevice-resource-type"></a>userExperienceAnalyticsWorkFromAnywhereDevice 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析设备：从任何位置工作的报告

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsWorkFromAnywhereDevices](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-list.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 集合|列出 [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-get.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|读取 [userExperienceAnalyticsWorkFromAnywhereDevice 对象的属性和](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 关系。|
|[创建 userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-create.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|创建新的 [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 对象。|
|[删除 userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-delete.md)|无|删除 [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)。|
|[更新 userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-update.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|更新 [userExperienceAnalyticsWorkFromAnywhereDevice 对象](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析的唯一标识符从任何设备工作。|
|deviceName|String|来自任何设备名称的工作。|
|serialNumber|String|用户体验随设备序列号随处工作。|
|manufacturer|String|用户体验从任何设备制造商处工作。|
|model|String|用户体验从任何设备型号开始工作。|
|ownership|String|用户体验从任何设备所有权开始工作。|
|managedBy|String|用户体验从设备的任何管理代理工作。|
|autoPilotRegistered|Boolean|用户体验从 intune 设备的 autopilotRegistered 的任何位置工作。|
|autoPilotProfileAssigned|Boolean|用户体验分析从 intune 设备的 autopilotProfileAssigned 的任何位置工作。|
|azureAdRegistered|Boolean|用户体验从任何设备的 azureAdRegistered 工作。|
|azureAdDeviceId|String|用户体验从 Azure Ad 设备 ID 的任何位置工作。|
|azureAdJoinType|String|用户体验从任何设备的 azure Ad joinType 工作。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "id": "String (identifier)",
  "deviceName": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "ownership": "String",
  "managedBy": "String",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "String",
  "azureAdJoinType": "String"
}
```




