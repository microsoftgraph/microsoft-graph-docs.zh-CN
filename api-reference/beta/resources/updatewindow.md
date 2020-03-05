---
title: updateWindow 资源类型
description: updateWindow 资源类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d0f509accba2cb73709a4a5fa504a5d2a716b038
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519580"
---
# <a name="updatewindow-resource-type"></a>updateWindow 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[代理](onpremisesagent.md)可以接收更新的时间窗口。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|updateWindowEndTime|TimeOfDay|代理可以在其中接收更新的时间窗口结束|
|updateWindowStartTime|TimeOfDay|代理可在其中接收更新的时间范围的开始时间|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateWindow",
  "baseType": null
}-->

```json
{
  "updateWindowEndTime": "String (timestamp)",
  "updateWindowStartTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "updateWindow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
