---
title: userExperienceAnalyticsDeviceStartupHistory 资源类型
description: 用户体验分析设备启动历史记录实体包含设备启动性能历史记录详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d3b435caf5cd8bb3c514eeb602f2397a6e93322754bb4313536ffb33ace5f727
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244713"
---
# <a name="userexperienceanalyticsdevicestartuphistory-resource-type"></a>userExperienceAnalyticsDeviceStartupHistory 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析设备启动历史记录实体包含设备启动性能历史记录详细信息。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsDeviceStartupHistories](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-list.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 集合|列出 [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-get.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|读取 [userExperienceAnalyticsDeviceStartupHistory 对象的属性和](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 关系。|
|[创建 userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-create.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|创建新的 [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 对象。|
|[删除 userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-delete.md)|无|删除 [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)。|
|[更新 userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-update.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|更新 [userExperienceAnalyticsDeviceStartupHistory 对象](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析设备启动历史记录的唯一标识符。|
|deviceId|String|用户体验分析设备 ID。|
|startTime|DateTimeOffset|用户体验分析设备启动开始时间。|
|coreBootTimeInMs|Int32|用户体验分析设备核心启动时间（以毫秒为单位）。|
|groupPolicyBootTimeInMs|Int32|用户体验分析 设备组策略启动时间（以毫秒为单位）。|
|featureUpdateBootTimeInMs|Int32|用户体验分析设备功能更新时间（以毫秒为单位）。|
|totalBootTimeInMs|Int32|用户体验分析设备总启动时间（以毫秒为单位）。|
|groupPolicyLoginTimeInMs|Int32|用户体验分析 设备组策略登录时间（以毫秒为单位）。|
|coreLoginTimeInMs|Int32|用户体验分析设备核心登录时间（以毫秒为单位）。|
|responsiveDesktopTimeInMs|Int32|用户体验分析响应式桌面时间（以毫秒为单位）。|
|totalLoginTimeInMs|Int32|用户体验分析设备登录总时间（以毫秒为单位）。|
|isFirstLogin|布尔值|用户体验分析设备第一次登录。|
|isFeatureUpdate|布尔值|用户体验分析设备启动记录是一项功能更新。|
|operatingSystemVersion|String|用户体验分析设备启动记录的操作系统版本。|
|restartCategory|[userExperienceAnalyticsOperatingSystemRestartCategory](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|操作系统重启类别。 可取值为：`unknown`、`restartWithUpdate`、`restartWithoutUpdate`、`blueScreen`、`shutdownWithUpdate`、`shutdownWithoutUpdate`、`longPowerButtonPress`、`bootError`、`update`。|
|restartStopCode|String|操作系统重新启动停止代码。 这将显示可用于查找蓝屏原因的错误检查代码。|
|restartFaultBucket|字符串|操作系统重新启动故障存储桶。 故障存储桶用于查找有关系统崩溃的其他信息。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceStartupHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "id": "String (identifier)",
  "deviceId": "String",
  "startTime": "String (timestamp)",
  "coreBootTimeInMs": 1024,
  "groupPolicyBootTimeInMs": 1024,
  "featureUpdateBootTimeInMs": 1024,
  "totalBootTimeInMs": 1024,
  "groupPolicyLoginTimeInMs": 1024,
  "coreLoginTimeInMs": 1024,
  "responsiveDesktopTimeInMs": 1024,
  "totalLoginTimeInMs": 1024,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "String",
  "restartCategory": "String",
  "restartStopCode": "String",
  "restartFaultBucket": "String"
}
```




