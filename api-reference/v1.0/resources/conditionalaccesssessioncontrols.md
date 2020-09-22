---
title: conditionalAccessSessionControls 资源类型
description: 表示登录后强制实施的会话控件的复杂类型。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 78c9ab3c3b5a55623ba13e1f7ce6d28a9425ded5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057008"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a>conditionalAccessSessionControls 资源类型

命名空间：microsoft.graph

表示登录后强制实施的会话控件。
所有会话控件都继承自 [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|applicationEnforcedRestrictions|[applicationEnforcedRestrictionsSessionControl](applicationenforcedrestrictionssessioncontrol.md)| 实施应用程序限制的会话控制。 仅 Exchange Online 和 Sharepoint Online 支持此会话控制。 |
|cloudAppSecurity|[cloudAppSecuritySessionControl](cloudappsecuritysessioncontrol.md)| 应用云应用安全性的会话控制。|
|persistentBrowser|[persistentBrowserSessionControl](persistentbrowsersessioncontrol.md)| 用于定义是否保持 cookie 的会话控制。 应选择所有应用程序以使此会话控件正常工作。 |
|signInFrequency|[signInFrequencySessionControl](signinfrequencysessioncontrol.md)| 用于强制登录频率的会话控制。|

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

