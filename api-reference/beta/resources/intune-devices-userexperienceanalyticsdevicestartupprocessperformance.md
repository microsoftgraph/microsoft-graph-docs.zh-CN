---
title: userExperienceAnalyticsDeviceStartupProcessPerformance 资源类型
description: User experience analytics 设备启动过程性能。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 11f8f7b6dc4d217235778de0cb36661361be6e10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080906"
---
# <a name="userexperienceanalyticsdevicestartupprocessperformance-resource-type"></a>userExperienceAnalyticsDeviceStartupProcessPerformance 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

User experience analytics 设备启动过程性能。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsDeviceStartupProcessPerformances](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-list.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) 集合|列出 [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-get.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|读取 [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-create.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|创建新的 [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) 对象。|
|[删除 userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-delete.md)|无|删除 [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)。|
|[更新 userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-devices-userexperienceanalyticsdevicestartupprocessperformance-update.md)|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|更新 [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|User experience analytics 设备启动过程性能的唯一标识符。|
|processName|字符串|User experience analytics 设备启动过程名称。|
|productName|String|User experience analytics 设备启动过程产品名称。|
|发布者|String|User experience analytics 设备启动过程发布者。|
|deviceCount|Int64|User experience analytics 设备启动过程汇总计数。|
|medianImpactInMs|Int32|User experience analytics 设备启动过程的中间影响（以毫秒为单位）。|
|totalImpactInMs|Int32|User experience analytics 设备启动过程以毫秒为单位的总影响。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "id": "String (identifier)",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "deviceCount": 1024,
  "medianImpactInMs": 1024,
  "totalImpactInMs": 1024
}
```






