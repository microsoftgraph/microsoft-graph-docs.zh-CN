---
title: userInsightsSettings 资源类型
description: 表示项目见解和会议时间见解的用户隐私设置。
ms.localizationpriority: medium
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 723f1ca8d0a56116039ae3f85eb0d534c3525972
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780889"
---
# <a name="userinsightssettings-resource-type"></a>userInsightsSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [itemInsights](iteminsights.md) 和会议时间见解 [的用户隐私设置](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) 。 使用此资源可禁用/启用计算和查看用户的项目见解和会议时间见解。 

- 项目见解：计算用户和项目（如文档中的文档或网站）Microsoft 365。  
- 会议时间见解：根据 Word、Excel、PowerPoint、电子邮件和 Outlook 日历中的活动计算Microsoft 365。

使用 [insightsSettings](insightssettings.md) 资源在组织级别禁用/启用项目见解、会议小时数见解或人员见解的计算和可见性。

## <a name="methods"></a>方法

| 方法                                                 | 返回类型                                                   | 说明                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [Get](../api/userinsightssettings-get.md)       | [userInsightsSettings](userinsightssettings.md) | 读取 **userinsightssettings 对象** 的属性。  |
| [更新](../api/userinsightssettings-update.md) | [userInsightsSettings](userinsightssettings.md) | 更新 **userinsightssettings 对象** 的属性。 |

## <a name="properties"></a>属性
| 属性                   | 类型                                                  | 说明                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| isEnabled     | Boolean  |  `true` 如果用户的 **itemInsights** 和会议时间见解已启用; `false` 如果禁用了 **用户的 itemInsights** 和会议小时数见解。 默认值为 `true`。 可选。|

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


