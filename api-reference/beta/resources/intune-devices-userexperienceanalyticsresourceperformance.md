---
title: userExperienceAnalyticsResourcePerformance 资源类型
description: 用户体验分析资源性能实体。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ca9f8fa6449871e5ead56976808267bb6cf2bfd9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046979"
---
# <a name="userexperienceanalyticsresourceperformance-resource-type"></a>userExperienceAnalyticsResourcePerformance 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析资源性能实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsResourcePerformances](../api/intune-devices-userexperienceanalyticsresourceperformance-list.md)|[userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 集合|列出 [userExperienceAnalyticsResourcePerformance 对象的属性和](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 关系。|
|[获取 userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-get.md)|[userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|读取 [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-create.md)|[userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|创建新的 [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 对象。|
|[删除 userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-delete.md)|无|删除 [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)。|
|[更新 userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-update.md)|[userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|更新 [userExperienceAnalyticsResourcePerformance 对象](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 的属性。|
|[summarizeDeviceResourcePerformance 函数](../api/intune-devices-userexperienceanalyticsresourceperformance-summarizedeviceresourceperformance.md)|[userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析资源性能实体的唯一标识符。|
|deviceId|String|设备的 ID。|
|deviceName|String|设备的名称。|
|model|String|用户体验分析设备模型。|
|deviceCount|Int64|用户体验分析汇总了设备计数。|
|manufacturer|String|用户体验分析设备制造商。|
|cpuSpikeTimePercentage|双精度|CPU 峰值时间百分比。 有效值为 0 至 100|
|ramSpikeTimePercentage|双精度|以百分比表示的 RAM 峰值时间。 有效值为 0 至 100|
|cpuSpikeTimeScore|Int32|用户体验分析设备 CPU 峰值时间分数。 有效值为 0 至 100|
|cpuSpikeTimePercentageThreshold|双精度|cpuSpikeTimeScore 的阈值。 有效值为 0 至 100|
|ramSpikeTimeScore|Int32|用户体验分析设备 RAM 峰值时间分数。 有效值为 0 至 100|
|ramSpikeTimePercentageThreshold|双精度|ramSpikeTimeScore 的阈值。 有效值为 0 至 100|
|deviceResourcePerformanceScore|Int32|特定设备的资源性能分数。 有效值为 0 至 100|
|averageSpikeTimeScore|Int32|设备或型号类型的 AverageSpikeTimeScore。 有效值为 0 至 100|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsResourcePerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceName": "String",
  "model": "String",
  "deviceCount": 1024,
  "manufacturer": "String",
  "cpuSpikeTimePercentage": "4.2",
  "ramSpikeTimePercentage": "4.2",
  "cpuSpikeTimeScore": 1024,
  "cpuSpikeTimePercentageThreshold": "4.2",
  "ramSpikeTimeScore": 1024,
  "ramSpikeTimePercentageThreshold": "4.2",
  "deviceResourcePerformanceScore": 1024,
  "averageSpikeTimeScore": 1024
}
```



