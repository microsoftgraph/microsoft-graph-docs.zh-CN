---
title: userExperienceAnalyticsBatteryHealthDeviceAppImpact 资源类型
description: 用户体验分析电池运行状况设备应用影响实体包含给定设备的应用级别的电池使用情况相关信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6e1e9dafdc831528ff9d05115f86a68b1df328d4
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348066"
---
# <a name="userexperienceanalyticsbatteryhealthdeviceappimpact-resource-type"></a>userExperienceAnalyticsBatteryHealthDeviceAppImpact 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析电池运行状况设备应用影响实体包含给定设备的应用级别的电池使用情况相关信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsBatteryHealthDeviceAppImpacts](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-list.md)|[userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md) 集合|列出 [userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsBatteryHealthDeviceAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-get.md)|[userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|读取 [userExperienceAnalyticsBatteryHealthDeviceAppImpact 对象的属性和](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md) 关系。|
|[创建 userExperienceAnalyticsBatteryHealthDeviceAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-create.md)|[userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|创建新的 [userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md) 对象。|
|[删除 userExperienceAnalyticsBatteryHealthDeviceAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-delete.md)|None|删除用户 [ExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)。|
|[更新 userExperienceAnalyticsBatteryHealthDeviceAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-update.md)|[userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|更新 [userExperienceAnalyticsBatteryHealthDeviceAppImpact 对象](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析电池设备应用影响对象的唯一标识符。|
|deviceId|String|设备的唯一标识符，Intune DeviceID 或 SCCM 设备 ID。|
|appName|String|应用名称。 例如：oltk.exe|
|appDisplayName|String|适用于显示名称用户友好应用程序。 例如：Outlook|
|appPublisher|String|应用发布者。 例如：Microsoft Corporation|
|isForegroundApp|布尔|如果用户与应用有活动交互，则其为 true。|
|batteryUsagePercentage|双精度|在 14 天内，当设备未接通交流电源时，此应用程序使用的电池总电量的百分比。 百分比单位。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceAppImpact"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceAppImpact",
  "id": "String (identifier)",
  "deviceId": "String",
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "isForegroundApp": true,
  "batteryUsagePercentage": "4.2"
}
```




