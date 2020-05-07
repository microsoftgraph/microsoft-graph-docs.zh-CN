---
title: openShiftItem 资源类型
description: 表示打开的班次的单个计数。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2fb690d06a2ca20fe8c4c50d41a06bc2d247ef1f
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154975"
---
# <a name="openshiftitem-resource-type"></a>openShiftItem 资源类型

命名空间：microsoft.graph

表示[openShift](../resources/openshift.md)的单个计数。

## <a name="properties"></a>属性

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|openSlotCount|Int32| 给定的打开班次的槽数的计数。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftItem",
  "baseType": "microsoft.graph.shiftItem"
}-->

```json
{
  "openSlotCount": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
