---
author: daspek
ms.author: dspektor
title: incompleteData 资源类型
description: IncompleteData facet 指示资源是使用不完整的数据生成的。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5fdf78b0fdb0a34e87296619c477d9f868d0756e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531324"
---
# <a name="incompletedata-resource-type"></a>incompleteData 资源类型

命名空间：microsoft.graph

**IncompleteData** facet 指示资源是使用不完整的数据生成的。
中的属性可能提供有关数据不完整的原因的信息。

## <a name="properties"></a>属性

| 属性                  | 类型           | 说明
|:--------------------------|:---------------|:--------------------------------
| missingDataBeforeDateTime | DateTimeOffset | 该服务在指定的时间之前没有源数据。
| wasThrottled              | Boolean        | 由于活动过多而未记录某些数据。

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/incompleteData",
  "suppressions": []
}
-->
