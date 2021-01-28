---
title: conditionalAccessConditionSet 资源类型
description: 表示在应用策略时控制的条件类型。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c3163bbefef420a878364f52f9dabc8dee1e7cae
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013672"
---
# <a name="conditionalaccessconditionset-resource-type"></a>conditionalAccessConditionSet 资源类型

命名空间：microsoft.graph

表示在应用策略时控制的条件类型。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|应用程序|[conditionalAccessApplications](conditionalaccessapplications.md)| 策略中包含和排除的应用程序和用户操作。 必填。 |
|users|[conditionalAccessUsers](conditionalaccessusers.md)| 策略中包含和排除的用户、组和角色。 必填。 |
|clientAppTypes|String collection| 策略中包含的客户端应用程序类型。 可取值为：`all`、`browser`、`mobileAppsAndDesktopClients`、`exchangeActiveSync`、`easSupported`、`other`。|
|locations|[conditionalAccessLocations](conditionalaccesslocations.md)| 策略中包含的位置和从策略中排除的位置。 |
|平台|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| 策略中包含的平台和从策略中排除的平台。 |
|signInRiskLevels|String collection| 策略中包含的登录风险级别。 可取值为：`low`、`medium`、`high`、`none`。|
|userRiskLevels|String collection| 策略中包含的用户风险级别。 可取值为：`low`、`medium`、`high`。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "locations",
    "platforms",
    "signInRiskLevels",
    "userRiskLevels"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessConditionSet",
  "baseType": null
}-->

```json
{
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientAppTypes": ["String"],
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"],
  "userRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

