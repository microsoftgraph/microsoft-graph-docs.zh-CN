---
title: conditionalAccessGrantControls 资源类型
description: 表示必须通过策略而必须实现的授予控制。
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 03b1b717b59e91d115f5974ff691ad2db956b4a3
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162054"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>conditionalAccessGrantControls 资源类型

命名空间：microsoft.graph

表示必须通过策略而必须实现的授予控制。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| operator | String | 定义授予控件的关系。 可能的值 `AND` `OR` ：、。 |
| builtInControls | conditionalAccessGrantControl 集合 | 策略所需的内置控件的值列表。 可能的值 `block` `mfa` `compliantDevice` ：、、、、、、、。 `domainJoinedDevice` `approvedApplication` `compliantApplication` `passwordChange` `unknownFutureValue` |
| customAuthenticationFactors | 字符串集合 | 策略所需的自定义控件的 ID 列表。 有关详细信息，请参阅自定义 [控件](/azure/active-directory/conditional-access/controls)。 |
| termsOfUse | String 集合 | 策略 [所需的使用条款](/graph/api/resources/agreement) ID 列表。 |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a>用作控件时 `passwordChange` 的特殊注意事项

使用控件时，请考虑 `passwordChange` 以下事项： 

- `passwordChange` 必须附带 `mfa` 使用 `AND` 运算符。 此组合可确保以安全方式更新密码。
- `passwordChange` 必须在包含 的策略中使用 `userRiskLevels` 。 这旨在支持用户必须使用安全更改密码重置其用户风险的方案。
- 该策略应面向 `all` 应用程序，而不是排除任何应用程序。
- 该策略不能包含除 和 之外 `users` 的其他 `applications` 条件 `userRiskLevels` 。

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
