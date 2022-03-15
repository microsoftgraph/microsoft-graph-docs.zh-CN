---
title: insightsSettings 资源类型
description: 表示见解的隐私设置。
ms.localizationpriority: medium
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 61625b4d9309ca203d1d523f1fcdb4f0fe6c583f
ms.sourcegitcommit: 0fa7148e0b776663eaca3e79e72b85046d4b8b1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/15/2022
ms.locfileid: "63500887"
---
# <a name="insightssettings-resource-type"></a>insightsSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

_表示_ 用于计算和管理组织中特定类型见解的显示或编程返回的设置。 见解可以是项目见解、会议时间见解或人员见解。 

项目见解和[会议时间见解](https://support.microsoft.com/office/suggested-meeting-hours-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)表示用户与项目（如文档、网站和其他内容类型）之间Microsoft 365。 以编程方式，它们由 [itemInsights 资源](iteminsights.md) 表示。 您可以获取与用户[共享](../api/insights-list-shared.md)的文档、[用户趋势或](../api/insights-list-trending.md)[用户使用](../api/insights-list-used.md)的文档。 可以使用 **insightsSettings** 自定义用于计算、显示或返回组织中 [项目见解的隐私设置](/graph/insights-customize-item-insights-privacy)。

人员见解表示基于其业务关系彼此相关或彼此合作的人脉。 以编程方式，个人人员由 [person](person.md) 资源表示。 可以使用 [人员 API 获取人员见解](/graph/people-example)。 可以使用 **insightsSettings** [自定义用于显示或](/graph/insights-customize-people-insights-privacy)返回人员见解的隐私设置。

相比之下，对于项目见解和会议时间[](https://support.microsoft.com/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)见解，您还可以使用 [userInsightsSettings](userinsightssettings.md) 资源在用户级别管理其计算和可见性。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [List itemInsights](../api/organizationsettings-list-iteminsights.md) | [insightsSettings](insightssettings.md) | 获取 [insightsSettings](insightssettings.md) 对象中的设置，用于显示组织中项目见解。 |
| [列出 peopleInsights](../api/organizationsettings-list-peopleinsights.md) | [insightsSettings](insightssettings.md) | 获取 [insightsSettings](insightssettings.md) 对象中的设置，用于显示组织中人员见解。 |
| [更新 insightsSettings](../api/insightssettings-update.md) | [insightsSettings](insightssettings.md) | 更新 **insightsSettings** 资源的属性，以管理指定类型见解（可以是项目见解或人员见解）的显示或返回。 |


## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Boolean| `true` 如果为组织启用了指定类型的见解; `false` 如果为所有用户禁用了指定类型的见解，则无例外。 默认值为“`true`”。 可选。|
|disabledForGroup|字符串| 已禁用Azure Active Directory组（其指定类型的见解）的 ID。 默认值为“`empty`”。 可选。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.insightsSettings"
}-->

```json
{
  "disabledForGroup": "String",
  "isEnabledInOrganization": "Boolean"
}
```





