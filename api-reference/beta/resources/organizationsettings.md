---
title: organizationSettings 资源类型
description: 包含适用于组织或其中用户对象的设置。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 105a57c7cb5827e9017df7494d32802ef7ac6fa5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158322"
---
# <a name="organizationsettings-resource-type"></a>organizationSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含适用于组织 [或](organization.md) 应用于组织中 [用户对象的](user.md) 设置。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取组织设置](../api/organizationsettings-get.md) | [organizationSettings](organizationsettings.md) | 读取组织设置对象。 |
| [创建 profileCardProperty](../api/organizationsettings-post-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | 通过发布到 **profileCardProperty** 对象集合创建新的 **profileCardProperty。** |
| [列出 profileCardProperties](../api/organizationsettings-list-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) 集合 | 获取 **profileCardProperty** 对象集合。 |
| [获取 itemInsightsSettings](../api/iteminsightssettings-get.md) | [itemInsightsSettings](iteminsightssettings.md) | 获取 **itemInsightsSettings 对象** 的属性。 |
| [更新 itemInsightsSettings](../api/iteminsightssettings-update.md) | [itemInsightsSettings](iteminsightssettings.md) | 更新指定 **itemInsightsSettings 资源** 的属性。 |

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|id |String| 组织的设置对象的 ID。 |
|profileCardProperties|[profileCardProperty](profilecardproperty.md) 集合| 包含管理员已定义为在 Microsoft 365 配置文件卡上可见的属性的集合。 [获取组织设置](../api/organizationsettings-get.md) 将返回为组织的配置文件卡配置的属性。|
|itemInsights|[itemInsightsSettings](iteminsightssettings.md)| 包含管理员为在用户与 Microsoft 365 中其他项目（如文档或网站）之间可见性 Microsoft Graph 派生的见解而配置的属性。 [通过此导航属性获取 itemInsightsSettings。](../api/iteminsightssettings-get.md)|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationSettings",
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


