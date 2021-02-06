---
title: conditionalAccessSessionControls 资源类型
description: 表示登录后强制执行的复杂会话控件类型。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: bf50399a26999c35730e2ce0c171c1be8777841d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134887"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a>conditionalAccessSessionControls 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示登录后强制执行的会话控件。
所有会话控件都继承自 [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|applicationEnforcedRestrictions|[applicationEnforcedRestrictionsSessionControl](applicationenforcedrestrictionssessioncontrol.md)| 强制实施应用程序限制的会话控制。 只有 Exchange Online 和 Sharepoint Online 支持此会话控制。 |
|cloudAppSecurity|[cloudAppSecuritySessionControl](cloudappsecuritysessioncontrol.md)| 应用云应用安全性的会话控制。|
|persistentBrowser|[persistentBrowserSessionControl](persistentbrowsersessioncontrol.md)| 用于定义是否保留 Cookie 的会话控件。 应选择所有应用，使此会话控件正常工作。 |
|signInFrequency|[signInFrequencySessionControl](signinfrequencysessioncontrol.md)| 强制登录频率的会话控制。|

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
    "signInFrequency"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessSessionControls",
  "baseType": null
}-->

```json
{
  "applicationEnforcedRestrictions": {"@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl"},
  "cloudAppSecurity": {"@odata.type": "microsoft.graph.cloudAppSecuritySessionControl"},
  "persistentBrowser": {"@odata.type": "microsoft.graph.persistentBrowserSessionControl"},
  "signInFrequency": {"@odata.type": "microsoft.graph.signInFrequencySessionControl"}
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

