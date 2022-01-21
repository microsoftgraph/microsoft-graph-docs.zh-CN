---
title: conditionalAccessSessionControls 资源类型
description: 表示登录后强制执行的复杂会话控件类型。
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c60d87cfab617bea22df27e8a289e90fb889b78a
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161621"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a>conditionalAccessSessionControls 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示登录后强制执行的会话控件。
所有会话控件都继承自 [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|applicationEnforcedRestrictions|[applicationEnforcedRestrictionsSessionControl](applicationenforcedrestrictionssessioncontrol.md)| 强制执行应用程序限制的会话控制。 只有 Exchange Online 和 Sharepoint Online 支持此会话控制。 |
|cloudAppSecurity|[cloudAppSecuritySessionControl](cloudappsecuritysessioncontrol.md)| 应用云应用安全性的会话控制。|
|continuousAccessEvaluation|[continuousAccessEvaluationSessionControl](../resources/continuousaccessevaluationsessioncontrol.md)|连续访问评估设置的会话控制。|
|disableResilienceDefaults|布尔| 会话控制，用于确定用户是否可以Azure AD中断之前收集的信息来扩展现有会话。|
|persistentBrowser|[persistentBrowserSessionControl](persistentbrowsersessioncontrol.md)| 用于定义是否保留 Cookie 的会话控件。 应选择所有应用，使此会话控件正常工作。 |
|signInFrequency|[signInFrequencySessionControl](signinfrequencysessioncontrol.md)| 强制执行登录频率的会话控制。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "applicationEnforcedRestrictions",
    "persistentBrowser",
    "cloudAppSecurity",
    "signInFrequency",
    "continuousAccessEvaluation",
    "disableResilienceDefaults"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessSessionControls",
  "baseType": null
}-->

```json
{
  "applicationEnforcedRestrictions": {"@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl"},
  "cloudAppSecurity": {"@odata.type": "microsoft.graph.cloudAppSecuritySessionControl"},
  "continuousAccessEvaluation": {"@odata.type": "microsoft.graph.continuousAccessEvaluationSessionControl"},
  "persistentBrowser": {"@odata.type": "microsoft.graph.persistentBrowserSessionControl"},
  "signInFrequency": {"@odata.type": "microsoft.graph.signInFrequencySessionControl"},
  "disableResilienceDefaults": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessSessionControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

