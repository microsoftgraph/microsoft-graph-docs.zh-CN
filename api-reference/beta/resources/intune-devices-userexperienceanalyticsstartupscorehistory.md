---
title: userExperienceAnalyticsStartupScoreHistory 资源类型
description: User experience analytics 设备启动分数历史记录。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a89a1b1ea890f26ef49d0cc5362af866c1f4c4ff
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163785"
---
# <a name="userexperienceanalyticsstartupscorehistory-resource-type"></a>userExperienceAnalyticsStartupScoreHistory 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

User experience analytics 设备启动分数历史记录。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsStartupScoreHistories](../api/intune-devices-userexperienceanalyticsstartupscorehistory-list.md)|[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)集合|列出[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)对象的属性和关系。|
|[获取 userExperienceAnalyticsStartupScoreHistory](../api/intune-devices-userexperienceanalyticsstartupscorehistory-get.md)|[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)|读取[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)对象的属性和关系。|
|[创建 userExperienceAnalyticsStartupScoreHistory](../api/intune-devices-userexperienceanalyticsstartupscorehistory-create.md)|[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)|创建新的[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)对象。|
|[删除 userExperienceAnalyticsStartupScoreHistory](../api/intune-devices-userexperienceanalyticsstartupscorehistory-delete.md)|无|删除[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)。|
|[更新 userExperienceAnalyticsStartupScoreHistory](../api/intune-devices-userexperienceanalyticsstartupscorehistory-update.md)|[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)|更新[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|User experience analytics 设备启动过程的唯一标识符。|
|startupDateTime|DateTimeOffset|User experience analytics 设备启动日期时间。|
|startupScore|Int32|用户体验分析设备启动分数。|
|coreBootScore|Int32|用户体验分析设备核心启动分数。|
|coreSigninScore|Int32|用户体验分析设备核心登录分数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsStartupScoreHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "id": "String (identifier)",
  "startupDateTime": "String (timestamp)",
  "startupScore": 1024,
  "coreBootScore": 1024,
  "coreSigninScore": 1024
}
```



