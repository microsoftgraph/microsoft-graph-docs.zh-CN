---
title: userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails 资源类型
description: 用户体验分析应用程序性能实体包含应用版本详细信息的应用性能。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d47b63e775eb19419b696f921482001d08574046
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58263385"
---
# <a name="userexperienceanalyticsapphealthappperformancebyappversiondetails-resource-type"></a>userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析应用程序性能实体包含应用版本详细信息的应用性能。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetailses](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-list.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md) 集合|列出 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails 对象的属性和](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md) 关系。|
|[获取 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-get.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|读取 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails 对象的属性和](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md) 关系。|
|[创建 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-create.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|创建新的 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md) 对象。|
|[删除 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-delete.md)|无|删除 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)。|
|[更新 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails-update.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)|更新 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails 对象](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析应用性能对象的唯一标识符。|
|deviceCountWithCrashes|Int32|已报告此应用程序和版本的一个或多个应用程序崩溃的设备总数。 有效值 -2147483648 to 2147483647|
|isMostUsedVersion|布尔值|应用程序版本是该应用程序最常用的版本。|
|isLatestUsedVersion|布尔值|应用程序的版本是该应用使用的最新版本。|
|appName|String|应用程序名。|
|appDisplayName|String|应用程序的友好名称。|
|appPublisher|String|应用程序的发布者。|
|appVersion|字符串|应用程序的版本。|
|appCrashCount|Int32|应用的崩溃数。 有效值 -2147483648 to 2147483647|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails",
  "id": "String (identifier)",
  "deviceCountWithCrashes": 1024,
  "isMostUsedVersion": true,
  "isLatestUsedVersion": true,
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appVersion": "String",
  "appCrashCount": 1024
}
```




