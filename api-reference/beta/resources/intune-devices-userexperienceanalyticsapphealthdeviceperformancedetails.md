---
title: userExperienceAnalyticsAppHealthDevicePerformanceDetails 资源类型
description: User experience analytics device performance entity 包含设备性能详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 834d2e2871e8ddf7366ddc1ea0e77398eeae48f9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081989"
---
# <a name="userexperienceanalyticsapphealthdeviceperformancedetails-resource-type"></a>userExperienceAnalyticsAppHealthDevicePerformanceDetails 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

User experience analytics device performance entity 包含设备性能详细信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsAppHealthDevicePerformanceDetailses](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-list.md)|[userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) 集合|列出 [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsAppHealthDevicePerformanceDetails](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-get.md)|[userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|读取 [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsAppHealthDevicePerformanceDetails](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-create.md)|[userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|创建新的 [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) 对象。|
|[删除 userExperienceAnalyticsAppHealthDevicePerformanceDetails](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-delete.md)|无|删除 [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)。|
|[更新 userExperienceAnalyticsAppHealthDevicePerformanceDetails](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-update.md)|[userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|更新 [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|User experience analytics 设备性能对象的唯一标识符。|
|eventDateTime|DateTimeOffset|事件发生的时间。|
|eventType|字符串|事件的类型。|
|appDisplayName|String|发生事件的应用程序的友好名称。|
|deviceId|String|设备的 id。|
|deviceDisplayName|String|设备的名称。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "eventType": "String",
  "appDisplayName": "String",
  "deviceId": "String",
  "deviceDisplayName": "String"
}
```






