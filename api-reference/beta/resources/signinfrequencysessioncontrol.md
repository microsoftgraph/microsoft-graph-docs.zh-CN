---
title: signInFrequencySessionControl 资源类型
description: 强制执行登录频率的会话控制。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: bc5123975dc15c7c49f0dcbec507c345cf057850
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761049"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a>signInFrequencySessionControl 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

强制执行登录频率的会话控制。 继承自 [条件访问会话控件](conditionalaccesssessioncontrol.md)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | 指定是否启用会话控件。 |
|type          |String       | 可取值为：`days`、`hours`。|
|值         |Int32        | 或 `days` 的编号 `hours` 。|

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
  "isEnabled": true,
  "type": "String",
  "value": 1024
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


