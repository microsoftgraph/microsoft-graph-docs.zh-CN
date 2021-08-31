---
title: userExperienceAnalyticsAppHealthApplicationPerformance 资源类型
description: 用户体验分析应用程序性能实体包含应用性能详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c81eef2fbab97c2ba2ed6a6a290fcfd790a7eb65
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788463"
---
# <a name="userexperienceanalyticsapphealthapplicationperformance-resource-type"></a>userExperienceAnalyticsAppHealthApplicationPerformance 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析应用程序性能实体包含应用性能详细信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsAppHealthApplicationPerformances](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-list.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 集合|列出 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-get.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|读取 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-create.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|创建新的 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 对象。|
|[删除 userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-delete.md)|无|删除 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)。|
|[更新 userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-update.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|更新 [userExperienceAnalyticsAppHealthApplicationPerformance 对象](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析应用性能对象的唯一标识符。|
|appHangCount|Int32|应用的挂起数。 有效值 -2147483648 2147483647|
|appHealthScore|双精度|应用的运行状况分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|appHealthStatus|String|应用的整体运行状况状态。|
|allOrgsHealthScore|双精度|所有组织的应用程序的中值运行状况分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|activeDeviceCount|Int32|应用处于活动状态的设备数。 有效值 -2147483648 2147483647|
|appName|String|应用程序名。|
|appDisplayName|String|应用程序的友好名称。|
|appPublisher|String|应用程序的发布者。|
|appUsageDuration|Int32|应用程序的总使用时间（分钟）。 有效值 -2147483648 2147483647|
|appCrashCount|Int32|应用的崩溃数。 有效值 -2147483648 2147483647|
|meanTimeToFailureInMinutes|Int32|应用失败平均时间（分钟）。 有效值 -2147483648 2147483647|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "id": "String (identifier)",
  "appHangCount": 1024,
  "appHealthScore": "4.2",
  "appHealthStatus": "String",
  "allOrgsHealthScore": "4.2",
  "activeDeviceCount": 1024,
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appUsageDuration": 1024,
  "appCrashCount": 1024,
  "meanTimeToFailureInMinutes": 1024
}
```



