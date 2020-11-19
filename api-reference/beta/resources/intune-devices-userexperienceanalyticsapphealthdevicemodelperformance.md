---
title: userExperienceAnalyticsAppHealthDeviceModelPerformance 资源类型
description: User experience analytics device model performance entity 包含设备模型性能详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4e0ee53570a5b92235737ac09db0d39e452c2156
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208547"
---
# <a name="userexperienceanalyticsapphealthdevicemodelperformance-resource-type"></a>userExperienceAnalyticsAppHealthDeviceModelPerformance 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

User experience analytics device model performance entity 包含设备模型性能详细信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsAppHealthDeviceModelPerformances](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-list.md)|[userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 集合|列出 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsAppHealthDeviceModelPerformance](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-get.md)|[userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|读取 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsAppHealthDeviceModelPerformance](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-create.md)|[userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|创建新的 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象。|
|[删除 userExperienceAnalyticsAppHealthDeviceModelPerformance](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-delete.md)|无|删除 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)。|
|[更新 userExperienceAnalyticsAppHealthDeviceModelPerformance](../api/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance-update.md)|[userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)|更新 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|User experience analytics 设备模型性能对象的唯一标识符。|
|deviceModel|String|设备的模型名称。|
|deviceManufacturer|String|设备的制造商名称。|
|activeDeviceCount|Int32|模型的活动设备数。 有效值-2147483648 到2147483647|
|meanTimeToFailureInMinutes|Int32|以分钟为单位的模型设备发生故障的平均时间。 有效值-2147483648 到2147483647|
|modelAppHealthScore|双精度|设备模型的应用运行状况得分。 有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308|
|modelAppHealthStatus|String|设备模型的整体应用运行状况状态。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
  "id": "String (identifier)",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "activeDeviceCount": 1024,
  "meanTimeToFailureInMinutes": 1024,
  "modelAppHealthScore": "4.2",
  "modelAppHealthStatus": "String"
}
```




