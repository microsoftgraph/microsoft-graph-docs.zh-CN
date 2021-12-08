---
title: userExperienceAnalyticsScoreHistory 资源类型
description: 用户体验分析设备启动分数历史记录。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 49e5390181c61c9817fa79f90073a7b355758e72
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348017"
---
# <a name="userexperienceanalyticsscorehistory-resource-type"></a>userExperienceAnalyticsScoreHistory 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析设备启动分数历史记录。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsScoreHistories](../api/intune-devices-userexperienceanalyticsscorehistory-list.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 集合|列出 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-get.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|读取 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-create.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|创建新的 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象。|
|[删除 userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-delete.md)|None|删除 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)。|
|[更新 userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-update.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|更新 [userExperienceAnalyticsScoreHistory 对象](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析设备启动过程的唯一标识符。|
|startupDateTime|DateTimeOffset|用户体验分析设备启动日期时间。|
|overallScore|Int32|用户体验分析总体分数。 分数范围为 0-100，100 是理想分数。 有效值为 0 至 100|
|startupScore|Int32|用户体验分析设备启动分数。 分数范围为 0-100，100 是理想分数。|
|coreBootScore|Int32|用户体验分析设备核心启动分数。 分数范围为 0-100，100 是理想分数。|
|coreSigninScore|Int32|用户体验分析设备核心登录分数。 分数范围为 0-100，100 是理想分数。|
|recommendedSoftwareScore|Int32|用户体验分析设备核心登录分数。 分数范围为 0-100，100 是理想分数。|
|appHealthOverallScore|Int32|用户体验分析应用运行状况总体分数。|
|batteryHealthScore|Int32|用户体验分析电池运行状况分数。|
|startupTotalDevices|Int32|用户体验分析类别启动性能的总设备计数。|
|recommendedSoftwareTotalDevices|Int32|用户体验分析类别推荐软件的总设备计数。|
|appHealthTotalDevices|Int32|用户体验分析类别应用运行状况的总设备计数。|
|batteryHealthTotalDevices|Int32|用户体验分析类别电池运行状况的总设备计数。|
|restartScore|Int32|重启分数。 分数将在 0-100 之间，100 是理想分数，0 表示重启过多。 有效值为 0 到 9999999|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsScoreHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "String (identifier)",
  "startupDateTime": "String (timestamp)",
  "overallScore": 1024,
  "startupScore": 1024,
  "coreBootScore": 1024,
  "coreSigninScore": 1024,
  "recommendedSoftwareScore": 1024,
  "appHealthOverallScore": 1024,
  "batteryHealthScore": 1024,
  "startupTotalDevices": 1024,
  "recommendedSoftwareTotalDevices": 1024,
  "appHealthTotalDevices": 1024,
  "batteryHealthTotalDevices": 1024,
  "restartScore": 1024
}
```




