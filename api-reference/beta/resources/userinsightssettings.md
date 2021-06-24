---
title: userInsightsSettings 资源类型
description: 表示项目见解和会议时间见解的用户隐私设置。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5ecc9277d0bd98df99387a5dd222998074c6eb1b
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109090"
---
# <a name="userinsightssettings-resource-type"></a>userInsightsSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [itemInsights](iteminsights.md) 和会议时间见解 [的用户隐私设置](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) 。 使用此资源可禁用/启用计算和查看用户的项目见解和会议时间见解。 

- 项目见解：计算用户与项目（如文档中的文档或网站）Microsoft 365。  
- 会议时间见解：根据 Word、Excel、PowerPoint、电子邮件和 Microsoft 365 日历中的活动计算Outlook会议Microsoft 365。

使用 [itemInsightsSettings](iteminsightssettings.md) 资源在组织级别禁用/启用项目见解和会议小时数见解的计算和可见性。

## <a name="methods"></a>方法

| 方法                                                 | 返回类型                                                   | 说明                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [获取](../api/userinsightssettings-get.md)       | [userInsightsSettings](userinsightssettings.md) | 读取 **userinsightssettings 对象** 的属性。  |
| [更新](../api/userinsightssettings-update.md) | [userInsightsSettings](userinsightssettings.md) | 更新 **userinsightssettings 对象** 的属性。 |

## <a name="properties"></a>属性
| 属性                   | 类型                                                  | 说明                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| isEnabled     | Boolean  |  `true` 如果用户的 **itemInsights** 和会议时间见解已启用; `false` 如果禁用了 **用户的 itemInsights** 和会议小时数见解。 默认值为“`true`”。 可选。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.userInsightsSettings"
}-->

```json
{
  "isEnabled": "Boolean"
}
```


