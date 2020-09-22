---
title: userExperienceAnalyticsScoreHistory 资源类型
description: User experience analytics 设备启动分数历史记录。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d5b4ef00ccdab5ba6f1fab8087027e24a87e6f8c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080766"
---
# <a name="userexperienceanalyticsscorehistory-resource-type"></a>userExperienceAnalyticsScoreHistory 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

User experience analytics 设备启动分数历史记录。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsScoreHistories](../api/intune-devices-userexperienceanalyticsscorehistory-list.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 集合|列出 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-get.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|读取 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-create.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|创建新的 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象。|
|[删除 userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-delete.md)|无|删除 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)。|
|[更新 userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-update.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|更新 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|User experience analytics 设备启动过程的唯一标识符。|
|startupDateTime|DateTimeOffset|User experience analytics 设备启动日期时间。|
|startupScore|Int32|用户体验分析设备启动分数。 分数将在范围0-100，100是理想的分数。|
|coreBootScore|Int32|用户体验分析设备核心启动分数。 分数将在范围0-100，100是理想的分数。|
|coreSigninScore|Int32|用户体验分析设备核心登录分数。 分数将在范围0-100，100是理想的分数。|
|recommendedSoftwareScore|Int32|用户体验分析设备核心登录分数。 分数将在范围0-100，100是理想的分数。|
|restartScore|Int32|重启分数。 分数将在范围0-100，100为理想分数，0表示重新启动过多。 有效值为0至9999999|

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
  "startupScore": 1024,
  "coreBootScore": 1024,
  "coreSigninScore": 1024,
  "recommendedSoftwareScore": 1024,
  "restartScore": 1024
}
```






