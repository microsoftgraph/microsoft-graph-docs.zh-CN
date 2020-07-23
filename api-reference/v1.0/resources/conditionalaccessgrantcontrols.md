---
title: conditionalAccessGrantControls 资源类型
description: 表示授予通过策略所需满足的控件。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aadf38ac5cff15e4c085f77df36aa6fd48fa272f
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384471"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>conditionalAccessGrantControls 资源类型

命名空间：microsoft.graph

表示授予通过策略所需满足的控件。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| operator | String | 定义授予控件的关系。 可能的值： `AND` 、 `OR` 。 |
| builtInControls | String collection | 策略所需的内置控件的值列表。 可能的值： `Block` 、、、、 `Mfa` `CompliantDevice` `DomainJoinedDevice` `ApprovedApplication` 、`CompliantApplication` |
| customAuthenticationFactors | String collection | 策略所需的自定义控件 Id 的列表。 有关详细信息，请参阅[自定义控件](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)。 |
| termsOfUse | String collection | 策略所需的[使用条款](https://docs.microsoft.com/graph/api/resources/agreement)id 的列表。 |

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
