---
title: userExperienceAnalyticsNotAutopilotReadyDevice 资源类型
description: 用户体验分析 设备未准备好 Windows autopilot。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c6104a142c76439bd3ad8ba9eaa2863bf2067b5e8096f278e5c1fad59367bf32
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54147964"
---
# <a name="userexperienceanalyticsnotautopilotreadydevice-resource-type"></a>userExperienceAnalyticsNotAutopilotReadyDevice 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析 设备未准备好 Windows autopilot。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsNotAutopilotReadyDevices](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-list.md)|[userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) 集合|列出 [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsNotAutopilotReadyDevice](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-get.md)|[userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|读取 [userExperienceAnalyticsNotAutopilotReadyDevice 对象的属性和](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) 关系。|
|[创建 userExperienceAnalyticsNotAutopilotReadyDevice](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-create.md)|[userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|创建新的 [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) 对象。|
|[删除 userExperienceAnalyticsNotAutopilotReadyDevice](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-delete.md)|无|删除 [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)。|
|[更新 userExperienceAnalyticsNotAutopilotReadyDevice](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-update.md)|[userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|更新 [userExperienceAnalyticsNotAutopilotReadyDevice 对象](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析 intune 设备的唯一标识符。|
|deviceName|String|intune 设备的名称。|
|serialNumber|String|intune 设备的序列号。|
|manufacturer|String|intune 设备的制造商。|
|model|String|intune 设备的型号。|
|managedBy|String|intune 设备的托管者。|
|autoPilotRegistered|布尔值|intune 设备的 autopilotRegistered。|
|autoPilotProfileAssigned|布尔值|intune 设备的 autopilotProfileAssigned。|
|azureAdRegistered|布尔值|intune 设备的 azureAdRegistered。|
|azureAdJoinType|字符串|intune 设备的 azure Ad joinType。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "id": "String (identifier)",
  "deviceName": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "managedBy": "String",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdJoinType": "String"
}
```




