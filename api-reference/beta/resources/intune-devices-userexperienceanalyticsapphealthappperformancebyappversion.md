---
title: userExperienceAnalyticsAppHealthAppPerformanceByAppVersion 资源类型
description: 用户体验分析应用程序性能实体包含应用程序版本的应用程序性能详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4c2c0ec5a532be1a9cb3090a4d2a1b6d69cb0fb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081994"
---
# <a name="userexperienceanalyticsapphealthappperformancebyappversion-resource-type"></a>userExperienceAnalyticsAppHealthAppPerformanceByAppVersion 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析应用程序性能实体包含应用程序版本的应用程序性能详细信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsAppHealthAppPerformanceByAppVersions](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-list.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 集合|列出 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-get.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)|读取 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-create.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)|创建新的 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象。|
|[删除 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-delete.md)|无|删除 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)。|
|[更新 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-update.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)|更新 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|User experience analytics 应用程序性能对象的唯一标识符。|
|appVersion|字符串|应用程序的版本。|
|appName|String|应用程序名。|
|appDisplayName|String|应用程序的友好名称。|
|appPublisher|字符串|应用程序的发布者。|
|appUsageDuration|Int32|应用程序的总使用时间，以分钟为单位。 有效值-2147483648 到2147483647|
|appCrashCount|Int32|应用程序的崩溃次数。 有效值-2147483648 到2147483647|
|meanTimeToFailureInMinutes|Int32|应用在几分钟内失败的平均时间。 有效值-2147483648 到2147483647|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersion",
  "id": "String (identifier)",
  "appVersion": "String",
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appUsageDuration": 1024,
  "appCrashCount": 1024,
  "meanTimeToFailureInMinutes": 1024
}
```






