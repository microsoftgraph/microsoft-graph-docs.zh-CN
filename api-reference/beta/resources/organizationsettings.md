---
title: organizationSettings 资源类型
description: 包含适用于组织或其中用户对象的设置。
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2c351cfe0f55ef7a2bfb1cf6d62a379ee335a644
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780581"
---
# <a name="organizationsettings-resource-type"></a>organizationSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含适用于组织 [或](organization.md) 应用于组织中用户 [对象的](user.md) 设置。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取组织设置](../api/organizationsettings-get.md) | [organizationSettings](organizationsettings.md) | 读取组织设置对象。 |
| [创建 profileCardProperty](../api/organizationsettings-post-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | 通过发布到 **profileCardProperty** 对象集合创建新的 **profileCardProperty。** |
| [列出 profileCardProperties](../api/organizationsettings-list-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) 集合 | 获取 **profileCardProperty** 对象集合。 |
| [List itemInsights](../api/organizationsettings-list-iteminsights.md) | [insightsSettings](insightssettings.md) | 获取 [insightsSettings](insightssettings.md) 对象的属性，用于显示或返回组织中项目见解。 |
| [列出 peopleInsights](../api/organizationsettings-list-peopleinsights.md) | [insightsSettings](insightssettings.md) | 获取 [insightsSettings](insightssettings.md) 对象的属性，用于显示或返回组织中人员见解。 |


## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|id |String| 组织的设置对象的 ID。 |
|profileCardProperties|[profileCardProperty](profilecardproperty.md) 集合| 包含管理员在配置文件卡上定义为可见的Microsoft 365集合。 [Get organization settings](../api/organizationsettings-get.md) returns the properties configured for profile cards for the organization.|
|itemInsights|[insightsSettings](insightssettings.md)| 包含由管理员配置的属性，用于查看 Microsoft Graph 派生的见解（用户与 Microsoft 365 中其他项目（如文档或网站）之间的可见性。 [List itemInsights](../api/organizationsettings-list-iteminsights.md) 返回 _在_ 组织中显示或返回项目见解的设置。|
|peopleInsights|[insightsSettings](insightssettings.md)| 包含由管理员配置的属性，用于查看与用户相关的人员列表以及与 Microsoft 365。 [](/graph/people-example#including-a-person-as-relevant-or-working-with) [列出 peopleInsights](../api/organizationsettings-list-peopleinsights.md) 返回 _在_ 组织中显示或返回人员见解的设置。|

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


