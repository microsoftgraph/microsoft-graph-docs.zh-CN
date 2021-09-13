---
title: persistentBrowserSessionControl 资源类型
description: 用于定义是否保留 Cookie 的会话控件。
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 52c4efd5d7a3bfb87c34ab07ba84349c6d392af3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117821"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a>persistentBrowserSessionControl 资源类型

命名空间：microsoft.graph

用于定义是否保留 Cookie 的会话控件。 继承自 [条件访问会话控件](conditionalaccesssessioncontrol.md)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | 指定是否启用会话控件。 |
|mode|persistentBrowserSessionMode| 可取值为：`always`、`never`。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.persistentBrowserSessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "mode": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "persistentBrowserSessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

