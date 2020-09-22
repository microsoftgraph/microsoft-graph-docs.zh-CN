---
title: itemInsightsSettings 资源类型
description: 表示 itemInsights 的隐私设置。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5d05a9fdf3a901fcddd55207bec373a3a0736afa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089327"
---
# <a name="iteminsightssettings-resource-type"></a>itemInsightsSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [itemInsights](iteminsights.md)的隐私设置，该设置配置从 microsoft Graph 派生的见解的可见性，在 microsoft 365 中的文档或网站) 的用户和其他项目 (。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [Get](../api/iteminsightssettings-get.md)| [itemInsightsSettings](iteminsightssettings.md) | 读取 **itemInsightsSettings** 对象的属性。 |
| [更新](../api/iteminsightssettings-update.md)| [itemInsightsSettings](iteminsightssettings.md) | 更新 **itemInsightsSettings** 对象。|


## <a name="properties"></a>属性
| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|isEnabledInOrganization|布尔| `true` 如果启用了组织项目见解，则为 `false` 如果对不例外的所有用户禁用了组织项目见解。 默认值为 `true`。 可选。|
|disabledForGroup|字符串| Azure AD 组的 ID，其中成员的项目见解已禁用。 默认值为 `empty`。 可选。|

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


