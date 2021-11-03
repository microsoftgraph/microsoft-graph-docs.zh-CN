---
title: userExperienceAnalyticsBatteryHealthModelPerformance 资源类型
description: 用户体验分析电池运行状况模型性能实体包含组织中所有唯一设备模型的电池相关信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae520e7123f14b48edbbb771d34a3bec0c9b76cd
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687830"
---
# <a name="userexperienceanalyticsbatteryhealthmodelperformance-resource-type"></a>userExperienceAnalyticsBatteryHealthModelPerformance 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析电池运行状况模型性能实体包含组织中所有唯一设备模型的电池相关信息。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsBatteryHealthModelPerformances](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-list.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) 集合|列出 [userExperienceAnalyticsBatteryHealthModelPerformance 对象的属性和](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) 关系。|
|[获取 userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-get.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|读取 [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-create.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|创建新的 [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) 对象。|
|[删除 userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-delete.md)|无|删除 [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)。|
|[更新 userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-update.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|更新 [userExperienceAnalyticsBatteryHealthModelPerformance 对象](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析电池运行状况模型性能对象的唯一标识符。|
|activeDevices|Int32|该型号的活动设备数。 有效值 -2147483648 2147483647|
|model|String|设备的型号名称。|
|manufacturer|String|设备制造商的名称。|
|averageMaxCapacityPercentage|Int32|给定型号的所有设备的最大容量的平均值。 最大容量用于测量设备电池的完全充电容量与设计容量。 有效值 -2147483648 2147483647|
|averageEstimatedRuntimeInMinutes|Int32|给定型号的所有设备的完全付费预计运行时的平均值。 单位（以分钟表示）。 有效值 -2147483648 2147483647|
|averageBatteryAgeInDays|Int32|租户中给定型号的所有设备的电池使用时间平均值。 单位（以天表示）。 有效值 -2147483648 2147483647|

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
  "averageBatteryAgeInDays": 1024
}
```



