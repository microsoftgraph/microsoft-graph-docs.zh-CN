---
title: userExperienceAnalyticsDeviceScores 资源类型
description: 用户体验分析设备分数实体合并了各种终结点分析分数。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3ecd5fefcb24d9672bac4ee597453e5c151d20df
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868470"
---
# <a name="userexperienceanalyticsdevicescores-resource-type"></a>userExperienceAnalyticsDeviceScores 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析设备分数实体合并了各种终结点分析分数。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsDeviceScoreses](../api/intune-devices-userexperienceanalyticsdevicescores-list.md)|[userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) 集合|列出 [userExperienceAnalyticsDeviceScores 对象的属性和](../resources/intune-devices-userexperienceanalyticsdevicescores.md) 关系。|
|[获取 userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-get.md)|[userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|读取 [userExperienceAnalyticsDeviceScores 对象的属性和](../resources/intune-devices-userexperienceanalyticsdevicescores.md) 关系。|
|[创建 userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-create.md)|[userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|创建新的 [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) 对象。|
|[删除 userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-delete.md)|无|删除 [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)。|
|[更新 userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-update.md)|[userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|更新 [userExperienceAnalyticsDeviceScores 对象](../resources/intune-devices-userexperienceanalyticsdevicescores.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析设备评分设备的唯一标识符。|
|deviceName|String|用户体验分析设备名称。|
|model|String|用户体验分析设备模型。|
|manufacturer|String|用户体验分析设备制造商。|
|endpointAnalyticsScore|双精度|用户体验分析设备分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|startupPerformanceScore|双精度|用户体验分析设备启动性能分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|appReliabilityScore|双精度|用户体验分析设备应用可靠性分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceScores"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
  "id": "String (identifier)",
  "deviceName": "String",
  "model": "String",
  "manufacturer": "String",
  "endpointAnalyticsScore": "4.2",
  "startupPerformanceScore": "4.2",
  "appReliabilityScore": "4.2"
}
```




