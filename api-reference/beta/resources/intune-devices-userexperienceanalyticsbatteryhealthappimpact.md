---
title: userExperienceAnalyticsBatteryHealthAppImpact 资源类型
description: 用户体验分析电池运行状况应用影响实体包含租户的应用级别的电池使用情况相关信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c0ecc24b6cb9069091fe9cbb51694c12f5a12b95
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697169"
---
# <a name="userexperienceanalyticsbatteryhealthappimpact-resource-type"></a>userExperienceAnalyticsBatteryHealthAppImpact 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析电池运行状况应用影响实体包含租户的应用级别的电池使用情况相关信息。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsBatteryHealthAppImpacts](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-list.md)|[userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md) 集合|列出 [userExperienceAnalyticsBatteryHealthAppImpact 对象的属性和](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md) 关系。|
|[获取 userExperienceAnalyticsBatteryHealthAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-get.md)|[userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|读取 [userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsBatteryHealthAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-create.md)|[userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|创建新的 [userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md) 对象。|
|[删除 userExperienceAnalyticsBatteryHealthAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-delete.md)|无|删除 [userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)。|
|[更新 userExperienceAnalyticsBatteryHealthAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-update.md)|[userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|更新 [userExperienceAnalyticsBatteryHealthAppImpact 对象](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析电池应用影响对象的唯一标识符。|
|activeDevices|Int32|14 天期间使用该应用的活动设备数。 有效值 -2147483648 to 2147483647|
|appName|String|应用名称。 例如：oltk.exe|
|appDisplayName|String|适用于显示名称用户友好应用程序。 例如：Outlook|
|appPublisher|String|应用发布者。 例如：Microsoft Corporation|
|isForegroundApp|布尔值|如果用户与应用有活动交互，则其为 true。|
|batteryUsagePercentage|双精度|当设备未接通交流电源时，此应用程序在 14 天内在租户中所有设备上计算出的总电池电源百分比。 百分比单位。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthAppImpact"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthAppImpact",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "isForegroundApp": true,
  "batteryUsagePercentage": "4.2"
}
```



