---
title: userExperienceAnalyticsDeviceStartupHistory 资源类型
description: User experience analytics 设备启动历史记录实体包含设备启动性能历史记录详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1e907b162082f8622c50bc7b7c9b4610dfab7867
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080927"
---
# <a name="userexperienceanalyticsdevicestartuphistory-resource-type"></a>userExperienceAnalyticsDeviceStartupHistory 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

User experience analytics 设备启动历史记录实体包含设备启动性能历史记录详细信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsDeviceStartupHistories](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-list.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 集合|列出 [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-get.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|读取 [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-create.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|创建新的 [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 对象。|
|[删除 userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-delete.md)|无|删除 [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)。|
|[更新 userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-update.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|更新 [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|User experience analytics 设备启动历史记录的唯一标识符。|
|deviceId|String|User experience analytics 设备 id。|
|startTime|DateTimeOffset|用户体验分析设备启动开始时间。|
|coreBootTimeInMs|Int32|User experience analytics device core boot time （以毫秒为单位）。|
|groupPolicyBootTimeInMs|Int32|User experience analytics Device group policy boot time （以毫秒为单位）。|
|featureUpdateBootTimeInMs|Int32|User experience analytics 设备功能更新时间（以毫秒为单位）。|
|totalBootTimeInMs|Int32|User experience analytics 设备总启动时间（以毫秒为单位）。|
|groupPolicyLoginTimeInMs|Int32|User experience analytics 设备组策略登录时间（以毫秒为单位）。|
|coreLoginTimeInMs|Int32|User experience analytics device core login time （以毫秒为单位）。|
|responsiveDesktopTimeInMs|Int32|用户体验分析响应桌面时间（以毫秒为单位）。|
|totalLoginTimeInMs|Int32|User experience analytics 设备总登录时间（以毫秒为单位）。|
|isFirstLogin|布尔|User experience analytics 设备第一次登录。|
|isFeatureUpdate|布尔|User experience analytics 设备启动记录是一项功能更新。|
|operatingSystemVersion|String|User experience analytics 设备启动记录的操作系统版本。|
|restartCategory|[userExperienceAnalyticsOperatingSystemRestartCategory](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|OS 重新启动类别。 可取值为：`unknown`、`restartWithUpdate`、`restartWithoutUpdate`、`blueScreen`、`shutdownWithUpdate`、`shutdownWithoutUpdate`、`longPowerButtonPress`、`bootError`。|
|restartStopCode|字符串|操作系统重新启动停止代码。 这将显示可用于查找蓝屏原因的 bug 检查代码。|
|restartFaultBucket|字符串|OS 重新启动故障存储桶。 故障存储桶用于查找有关系统崩溃的其他信息。|

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






