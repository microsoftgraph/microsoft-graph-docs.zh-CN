---
title: userExperienceAnalyticsAppHealthApplicationPerformance 资源类型
description: User experience analytics application performance entity 包含应用程序性能详细信息。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e5c6e2c9292d11cc1a7384d0213a0adbd85921c3
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793238"
---
# <a name="userexperienceanalyticsapphealthapplicationperformance-resource-type"></a>userExperienceAnalyticsAppHealthApplicationPerformance 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

User experience analytics application performance entity 包含应用程序性能详细信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsAppHealthApplicationPerformances](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-list.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 集合|列出 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-get.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|读取 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-create.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|创建新的 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 对象。|
|[删除 userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-delete.md)|无|删除 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)。|
|[更新 userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-update.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|更新 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|User experience analytics 应用程序性能对象的唯一标识符。|
|appName|String|应用程序名。|
|appFriendlyName|String|应用程序的友好名称。|
|appPublisher|String|应用程序的发布者。|
|activeDevices|Int32|应用程序处于活动状态的设备的数量。 有效值-2147483648 到2147483647|
|totalAppUsageDuration|Int32|应用程序的总使用时间，以分钟为单位。 有效值-2147483648 到2147483647|
|totalAppCrashes|Int32|应用程序的崩溃次数。 有效值-2147483648 到2147483647|
|totalAppHangs|Int32|应用程序的挂起次数。 有效值-2147483648 到2147483647|
|meanTimeToFailure|Int32|应用在几分钟内失败的平均时间。 有效值-2147483648 到2147483647|
|appHealthScore|双精度|应用程序的运行状况分数。 有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308|
|appHealthStatus|String|应用程序的整体运行状况状态。|
|allOrgsHealthScore|双精度|应用程序在所有组织中的中间运行状况分数。 有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308|
|allOrgsMeanTimeToFailure|Int32|在整个应用程序的所有 emc 中失败的中间平均时间（分钟）。 有效值-2147483648 到2147483647|
|tenantId|String|与此应用程序对象关联的租户的 id。|
|memaTimeGenerated|String|在 MEMA 中执行聚合时的时间。|

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
  "appName": "String",
  "appFriendlyName": "String",
  "appPublisher": "String",
  "activeDevices": 1024,
  "totalAppUsageDuration": 1024,
  "totalAppCrashes": 1024,
  "totalAppHangs": 1024,
  "meanTimeToFailure": 1024,
  "appHealthScore": "4.2",
  "appHealthStatus": "String",
  "allOrgsHealthScore": "4.2",
  "allOrgsMeanTimeToFailure": 1024,
  "tenantId": "String",
  "memaTimeGenerated": "String"
}
```



