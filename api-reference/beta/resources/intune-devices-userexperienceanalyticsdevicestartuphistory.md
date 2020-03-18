---
title: userExperienceAnalyticsDeviceStartupHistory 资源类型
description: User experience analytics 设备启动历史记录实体包含设备启动性能历史记录详细信息。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d4275053cda78e26093879b64a521870eec21089
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783821"
---
# <a name="userexperienceanalyticsdevicestartuphistory-resource-type"></a>userExperienceAnalyticsDeviceStartupHistory 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

User experience analytics 设备启动历史记录实体包含设备启动性能历史记录详细信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsDeviceStartupHistories](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-list.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)集合|列出[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象的属性和关系。|
|[获取 userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-get.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|读取[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象的属性和关系。|
|[创建 userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-create.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|创建新的[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象。|
|[删除 userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-delete.md)|None|删除[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)。|
|[更新 userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-update.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|更新[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|User experience analytics 设备启动历史记录的唯一标识符。|
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
|isFirstLogin|布尔值|User experience analytics 设备第一次登录。|
|isFeatureUpdate|布尔值|User experience analytics 设备启动记录是一项功能更新。|
|operatingSystemVersion|String|User experience analytics 设备启动记录的操作系统版本。|

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
  "operatingSystemVersion": "String"
}
```



