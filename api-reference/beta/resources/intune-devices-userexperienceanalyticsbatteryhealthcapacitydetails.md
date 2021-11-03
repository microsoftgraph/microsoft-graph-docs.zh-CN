---
title: userExperienceAnalyticsBatteryHealthCapacityDetails 资源类型
description: 用户体验分析电池运行状况容量实体包含分为 3 个类别的设备计数 - 容量为 > 80% 的设备、容量为 50-80% 的设备以及容量为 < 50% 的设备。此 API 提供这 3 个类别中的设备计数。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b03710f31470a7b1c43b15933b24e6cd90a14731
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689242"
---
# <a name="userexperienceanalyticsbatteryhealthcapacitydetails-resource-type"></a>userExperienceAnalyticsBatteryHealthCapacityDetails 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析电池运行状况容量实体包含分为 3 个类别的设备计数 - 容量为 > 80% 的设备、容量为 50-80% 的设备以及容量为 < 50% 的设备。此 API 提供这 3 个类别中的设备计数。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 userExperienceAnalyticsBatteryHealthCapacityDetails](../api/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails-get.md)|[userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md)|读取 [userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md) 对象的属性和关系。|
|[更新 userExperienceAnalyticsBatteryHealthCapacityDetails](../api/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails-update.md)|[userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md)|更新 [userExperienceAnalyticsBatteryHealthCapacityDetails 对象](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析电池运行状况容量对象的唯一标识符。|
|activeDevices|Int32|租户中的活动设备数。 有效值 -2147483648 to 2147483647|
|batteryCapacityGood|Int32|电池最大容量大于 80% 的设备数量。 有效值 -2147483648 to 2147483647|
|batteryCapacityFair|Int32|电池最大容量大于 50%但小于 80% 的设备数量。 有效值 -2147483648 to 2147483647|
|batteryCapacityPoor|Int32|电池最大容量小于 50% 的设备数量。 有效值 -2147483648 to 2147483647|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthCapacityDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthCapacityDetails",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "batteryCapacityGood": 1024,
  "batteryCapacityFair": 1024,
  "batteryCapacityPoor": 1024
}
```



