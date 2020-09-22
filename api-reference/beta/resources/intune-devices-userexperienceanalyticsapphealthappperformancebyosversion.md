---
title: userExperienceAnalyticsAppHealthAppPerformanceByOSVersion 资源类型
description: User experience analytics application performance entity 包含 OS 版本的应用程序性能详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 673833ebcdccb90f5d691a7dad9d560da774add3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081993"
---
# <a name="userexperienceanalyticsapphealthappperformancebyosversion-resource-type"></a>userExperienceAnalyticsAppHealthAppPerformanceByOSVersion 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

User experience analytics application performance entity 包含 OS 版本的应用程序性能详细信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsAppHealthAppPerformanceByOSVersions](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-list.md)|[userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) 集合|列出 [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-get.md)|[userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|读取 [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-create.md)|[userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|创建新的 [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) 对象。|
|[删除 userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-delete.md)|无|删除 [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)。|
|[更新 userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-update.md)|[userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|更新 [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|User experience analytics 应用程序版本性能对象的唯一标识符。|
|osVersion|String|应用程序的操作系统版本。|
|osBuildNumber|字符串|应用程序的操作系统内部版本号。|
|activeDeviceCount|Int32|应用程序处于活动状态的设备的数量。 有效值-2147483648 到2147483647|
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
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByOSVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByOSVersion",
  "id": "String (identifier)",
  "osVersion": "String",
  "osBuildNumber": "String",
  "activeDeviceCount": 1024,
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appUsageDuration": 1024,
  "appCrashCount": 1024,
  "meanTimeToFailureInMinutes": 1024
}
```






