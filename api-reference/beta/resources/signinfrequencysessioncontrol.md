---
title: signInFrequencySessionControl 资源类型
description: 用于强制执行登录频率的会话控制。
ms.localizationpriority: medium
author: rckyplln
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a42697bd49f9f6742c3f6c1e61ace9a8a1362111
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944447"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a>signInFrequencySessionControl 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于强制实施登录频率的会话控制。 继承自 [条件访问会话控制](conditionalaccesssessioncontrol.md)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | 指定是否启用会话控件。 |
|type          |signinFrequencyType       | 可能的值为： `days`、 `hours`或 `null` frequencyInterval 是否为 `everyTime` 。|
|值         |Int32        | 或 `days` `hours`.|
|authenticationType |signInFrequencyAuthenticationType  | 可能的值是 `primaryAndSecondaryAuthentication`， `secondaryAuthentication`. `unknownFutureValue`|
|frequencyInterval  |signInFrequencyInterval  | 可能的值是 `timeBased`， `everyTime`. `unknownFutureValue`|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInFrequencySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled":true,
  "type": "String",
  "value": 1024,
  "authenticationType": "String",
  "frequencyInterval": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInFrequencySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


