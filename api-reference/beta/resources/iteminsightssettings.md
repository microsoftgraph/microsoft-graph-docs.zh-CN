---
title: itemInsightsSettings 资源类型
description: 表示 itemInsights 的隐私设置。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c84b2397c938997a3285d16612d090ae22444580
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522725"
---
# <a name="iteminsightssettings-resource-type"></a>itemInsightsSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用于会议时间见解的 [itemInsights](iteminsights.md) 和隐私设置的隐私设置。 使用此 API 可以禁用/启用项目见解和会议时间见解的计算和可见性。 

- Item insights：计算用户和项目（如 Microsoft 365 中的文档或网站）之间的关系。  
- 会议时间见解：根据 Microsoft 365 中的 Word、Excel、PowerPoint、电子邮件和 Outlook 日历中的活动计算人员的日历会议时间。

> [!NOTE]
> 向从11月2020开始的客户推出会议时间见解。 

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [获取](../api/iteminsightssettings-get.md)| [itemInsightsSettings](iteminsightssettings.md) | 读取 **itemInsightsSettings** 对象的属性。 |
| [更新](../api/iteminsightssettings-update.md)| [itemInsightsSettings](iteminsightssettings.md) | 更新 **itemInsightsSettings** 对象。|


## <a name="properties"></a>属性
| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|isEnabledInOrganization|布尔值| `true` 如果启用了组织项目见解，则为 `false` 如果对不例外的所有用户禁用了组织项目见解。 默认值为 `true`。 可选。|
|disabledForGroup|String| Azure AD 组的 ID，其中成员的项目见解已禁用。 默认值为 `empty`。 可选。|

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


