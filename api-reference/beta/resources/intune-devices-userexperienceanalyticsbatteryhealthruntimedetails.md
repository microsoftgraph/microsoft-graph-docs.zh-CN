---
title: userExperienceAnalyticsBatteryHealthRuntimeDetails 资源类型
description: 用户体验分析电池运行状况运行时实体包含分为 3 类的设备计数：运行时为 > 5 小时的设备、运行时为 3-5 小时的设备以及运行时为 < 3 小时的设备。此 API 提供这 3 个类别中的设备计数。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4328abe87c73c10d0b5e16a2b9869b539d168a62
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292065"
---
# <a name="userexperienceanalyticsbatteryhealthruntimedetails-resource-type"></a>userExperienceAnalyticsBatteryHealthRuntimeDetails 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析电池运行状况运行时实体包含分为 3 类的设备计数：运行时为 > 5 小时的设备、运行时为 3-5 小时的设备以及运行时为 < 3 小时的设备。此 API 提供这 3 个类别中的设备计数。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 userExperienceAnalyticsBatteryHealthRuntimeDetails](../api/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails-get.md)|[userExperienceAnalyticsBatteryHealthRuntimeDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md)|读取 [userExperienceAnalyticsBatteryHealthRuntimeDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md) 对象的属性和关系。|
|[更新 userExperienceAnalyticsBatteryHealthRuntimeDetails](../api/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails-update.md)|[userExperienceAnalyticsBatteryHealthRuntimeDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md)|更新 [userExperienceAnalyticsBatteryHealthRuntimeDetails 对象](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析电池运行状况运行时对象的唯一标识符。|
|activeDevices|Int32|租户中的活动设备数。 有效值 -2147483648 2147483647|
|batteryRuntimeGood|Int32|活动运行时大于 5 小时的设备数量。 有效值 -2147483648 2147483647|
|batteryRuntimeFair|Int32|活动运行时大于 3 小时但小于 5 小时的设备数量。 有效值 -2147483648 2147483647|
|batteryRuntimePoor|Int32|活动运行时小于 3 小时的设备数量。 有效值 -2147483648 2147483647|
|lastRefreshedDateTime|DateTimeOffset|此运行时详细信息实例的记录日期时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthRuntimeDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthRuntimeDetails",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "batteryRuntimeGood": 1024,
  "batteryRuntimeFair": 1024,
  "batteryRuntimePoor": 1024,
  "lastRefreshedDateTime": "String (timestamp)"
}
```




