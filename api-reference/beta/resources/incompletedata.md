---
author: daspek
description: IncompleteData facet 指示资源是使用不完整的数据生成的。
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6505d02ee7436e02d90627cfd38a83e3e436706a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016557"
---
# <a name="incompletedata-resource-type"></a>incompleteData 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**IncompleteData** facet 指示资源是使用不完整的数据生成的。
中的属性可能提供了有关不完整数据的原因的信息。

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a>属性

| 属性                  | 类型           | 说明
|:--------------------------|:---------------|:--------------------------------
| missingDataBeforeDateTime | DateTimeOffset | 该服务在指定的时间之前没有源数据。
| wasThrottled              | Boolean        | 由于活动过多而未记录某些数据。

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->


