---
title: timeRange 资源类型
description: 具有开始时间和结束时间的时间范围资源。
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6bcfb783537616d6a30436e0d3685b21a664053c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094049"
---
# <a name="timerange-resource-type"></a>timeRange 资源类型

命名空间：microsoft.graph

具有开始时间和结束时间的时间范围资源。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|endTime|TimeOfDay|该时间范围的结束时间。|
|startTime|TimeOfDay|该时间范围的开始时间。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeRange",
  "baseType": null
}-->

```json
{
  "endTime": "String (timestamp)",
  "startTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
