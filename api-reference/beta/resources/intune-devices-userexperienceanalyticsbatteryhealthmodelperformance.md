---
title: userExperienceAnalyticsBatteryHealthModelPerformance 资源类型
description: 用户体验分析电池运行状况模型性能实体包含其组织中所有唯一设备模型的电池相关信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 010b4498a8b725519636a727e0fada648c3a2b69
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857426"
---
# <a name="userexperienceanalyticsbatteryhealthmodelperformance-resource-type"></a>userExperienceAnalyticsBatteryHealthModelPerformance 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析电池运行状况模型性能实体包含其组织中所有唯一设备模型的电池相关信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsBatteryHealthModelPerformances](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-list.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) 集合|列出 [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-get.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|读取 [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-create.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|创建新的 [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) 对象。|
|[删除 userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-delete.md)|None|删除 [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)。|
|[更新 userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-update.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|更新 [userExperienceAnalyticsBatteryHealthModelPerformance 对象的](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析电池运行状况模型性能对象的唯一标识符。|
|activeDevices|Int32|该模型的活动设备数。 有效值 -2147483648 2147483647|
|model|String|设备的模型名称。|
|manufacturer|String|设备制造商的名称。|
|averageMaxCapacityPercentage|Int32|给定模型的所有设备的最大容量的平均值。 最大容量度量设备电池的全费与设计容量。 有效值 -2147483648 2147483647|
|averageEstimatedRuntimeInMinutes|Int32|给定模型的所有设备的全费估计运行时的平均值。 以分钟为单位。 有效值 -2147483648 2147483647|
|averageBatteryAgeInDays|Int32|租户中给定模型的所有设备的电池使用时间平均值。 单位（以天为单位）。 有效值 -2147483648 2147483647|
|modelBatteryHealthScore|Int32|模型最大容量分数和运行时估计分数的加权平均值。 值范围为 0-100。 有效值 -2147483648 2147483647|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthModelPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthModelPerformance",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "model": "String",
  "manufacturer": "String",
  "averageMaxCapacityPercentage": 1024,
  "averageEstimatedRuntimeInMinutes": 1024,
  "averageBatteryAgeInDays": 1024,
  "modelBatteryHealthScore": 1024
}
```




