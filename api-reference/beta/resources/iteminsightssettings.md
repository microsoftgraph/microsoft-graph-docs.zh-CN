---
title: itemInsightsSettings 资源类型
description: 表示 itemInsights 的隐私设置。
ms.localizationpriority: medium
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 764e47071d0f7554e3bcdd2c5ce4350304bdd6fe
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891222"
---
# <a name="iteminsightssettings-resource-type"></a>itemInsightsSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用于会议时间 [见解的 itemInsights](iteminsights.md) 的隐私 [设置和隐私设置](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) 。 使用此 API 禁用/启用项目见解和会议时间见解的计算和可见性。 

- 项目见解：计算用户与项目（如文档中的文档或网站）Microsoft 365。  
- 会议小时数见解：根据 Word、Excel、PowerPoint、电子邮件和 Microsoft 365 中的活动计算Outlook会议Microsoft 365。

使用 [userInsightsSettings](userinsightssettings.md) 资源可禁用/启用计算和查看用户的项目见解和会议时间见解。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [Get](../api/iteminsightssettings-get.md)| [itemInsightsSettings](iteminsightssettings.md) | 读取 **itemInsightsSettings 对象** 的属性。 |
| [更新](../api/iteminsightssettings-update.md)| [itemInsightsSettings](iteminsightssettings.md) | 更新 **itemInsightsSettings** 对象。|


## <a name="properties"></a>属性
| 属性   | 类型|描述|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Boolean| `true` 如果已启用组织项目见解; `false` 如果为所有用户禁用组织项目见解，则无例外。 默认值为 `true`。 可选。|
|disabledForGroup|String| 已禁用Azure AD项见解的组 ID。 默认值为 `empty`。 可选。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.itemInsightsSettings"
}-->

```json
{
  "isEnabledInOrganization": "Boolean",
  "disabledForGroup": "String"
}
```


