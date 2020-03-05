---
title: conditionalAccessGrantControls 资源类型
description: 表示授予通过策略所需满足的控件。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b91afb44cc43c3c6ac4970afc36914abcb08c4c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507546"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>conditionalAccessGrantControls 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示授予通过策略所需满足的控件。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| operator | String | 定义授予控件的关系。 可能的值`AND`： `OR`、。 |
| builtInControls | String 集合 | 策略所需的内置控件的值列表。 可能的值`Block`： `Mfa`、 `CompliantDevice`、 `DomainJoinedDevice`、 `ApprovedApplication`、、`CompliantApplication` |
| customAuthenticationFactors | String 集合 | 策略所需的自定义控件 Id 的列表。 在此处了解有关自定义控件的详细信息：https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview |
| termsOfUse | String 集合 | 策略所需的[使用条款](agreement.md)id 的列表。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "operator",
    "builtInControls",
    "customAuthenticationFactors",
    "termsOfUse"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessGrantControls",
  "baseType": null
}-->

```json
{
  "builtInControls": ["String"],
  "customAuthenticationFactors": ["String"],
  "operator": "String",
  "termsOfUse": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessGrantControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->