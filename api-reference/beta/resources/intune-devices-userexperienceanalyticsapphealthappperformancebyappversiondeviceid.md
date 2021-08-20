---
title: userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId 资源类型
description: 用户体验分析应用程序性能实体包含按应用版本设备 ID 的应用性能。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: efaaa1c2ac380fc3802426fc771f4bdfed7c6b99
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259218"
---
# <a name="userexperienceanalyticsapphealthappperformancebyappversiondeviceid-resource-type"></a>userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析应用程序性能实体包含按应用版本设备 ID 的应用性能。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceIds](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-list.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md) 集合|列出 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId 对象的属性和](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md) 关系。|
|[获取 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-get.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|读取 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId 对象的属性和](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md) 关系。|
|[创建 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-create.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|创建新的 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md) 对象。|
|[删除 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-delete.md)|无|删除 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)。|
|[更新 userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-update.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|更新 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId 对象](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析应用性能对象的唯一标识符。|
|deviceId|String|设备的 ID。|
|deviceDisplayName|String|设备的名称。|
|processedDateTime|DateTimeOffset|上次计算统计信息的日期和时间。|
|appName|String|应用程序名。|
|appDisplayName|String|应用程序的友好名称。|
|appPublisher|String|应用程序的发布者。|
|appVersion|String|应用程序的版本。|
|appCrashCount|Int32|应用的崩溃数。 有效值 -2147483648 2147483647|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceDisplayName": "String",
  "processedDateTime": "String (timestamp)",
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appVersion": "String",
  "appCrashCount": 1024
}
```




