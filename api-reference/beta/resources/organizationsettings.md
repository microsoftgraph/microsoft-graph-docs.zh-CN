---
title: organizationSettings 资源类型
description: 包含适用于组织或其内的用户对象的设置。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e95bae902b444735b87fa7b29e061bf9bf2629ba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998472"
---
# <a name="organizationsettings-resource-type"></a>organizationSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含适用于 [组织](organization.md) 或应应用于组织中的 [用户](user.md) 对象的设置。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取组织设置](../api/organizationsettings-get.md) | [organizationSettings](organizationsettings.md) | 读取组织设置对象。 |
| [创建 profileCardProperty](../api/organizationsettings-post-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | 通过发布到**profileCardProperty**对象集合创建新的**profileCardProperty** 。 |
| [列出 profileCardProperties](../api/organizationsettings-list-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) 集合 | 获取 **profileCardProperty** 对象集合。 |
| [获取 itemInsightsSettings](../api/iteminsightssettings-get.md) | [itemInsightsSettings](iteminsightssettings.md) | 获取 **itemInsightsSettings** 对象的属性。 |
| [更新 itemInsightsSettings](../api/iteminsightssettings-update.md) | [itemInsightsSettings](iteminsightssettings.md) | 更新指定的 **itemInsightsSettings** 资源的属性。 |

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|id |String| 组织的设置对象的 Id。 |
|profileCardProperties|[profileCardProperty](profilecardproperty.md) 集合| 包含管理员已定义为在 Microsoft 365 配置文件卡上可见的属性的集合。 [Get organization settings](../api/organizationsettings-get.md) 返回为组织配置文件卡片配置的属性。|
|itemInsights|[itemInsightsSettings](iteminsightssettings.md)| 包含由管理员为 microsoft Graph 派生的见解的可见性配置的属性，这些属性与 Microsoft 365 中的用户和其他项目（如文档或网站）之间的可见性。 通过此导航属性[获取 itemInsightsSettings](../api/iteminsightssettings-get.md) 。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationSettings",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "profileCardProperties": [{"@odata.type": "microsoft.graph.profileCardProperty"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizationSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


