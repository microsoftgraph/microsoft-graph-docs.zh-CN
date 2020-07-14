---
title: conditionalAccessGrantControls 资源类型
description: 表示授予通过策略所需满足的控件。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7465ecc3f8e1b99c001fca5d6f43391cf0ef682d
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122502"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>conditionalAccessGrantControls 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示授予通过策略所需满足的控件。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| operator | String | 定义授予控件的关系。 可能的值： `AND` 、 `OR` 。 |
| builtInControls | String collection | 策略所需的内置控件的值列表。 可能的值：、、、、、 `block` `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` 、 `passwordChange` 。 |
| customAuthenticationFactors | String collection | 策略所需的自定义控件 Id 的列表。 在此处了解有关自定义控件的详细信息：https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview |
| termsOfUse | String collection | 策略所需的[使用条款](agreement.md)id 的列表。 |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a>使用 `passwordChange` 作为控件时的特殊注意事项

使用控件时，请注意以下 `passwordChange` 几点： 

- `passwordChange`必须 `mfa` 与运算符一起使用 `AND` 。 此组合可确保密码将以安全的方式进行更新。
- `passwordChange`必须在包含的策略中使用 `userRiskLevels` 。 这旨在实现用户必须使用安全更改密码重置其用户风险的方案。
- 该策略应以 `all` 应用程序为目标，而不排除任何应用程序。
- 策略不能包含任何其他条件。

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
