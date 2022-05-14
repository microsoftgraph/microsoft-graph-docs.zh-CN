---
author: daspek
description: 不完整的Data 方面指示使用不完整的数据生成了资源。
ms.date: 10/06/2017
title: IncompleteData
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: b24b10db7f38ee17356c77d40bcda3b08576e45b
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420675"
---
# <a name="incompletedata-resource-type"></a>incompleteData 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**不完整的Data** 方面指示使用不完整的数据生成了资源。
其中的属性可能会提供有关数据不完整原因的信息。

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
| missingDataBeforeDateTime | DateTimeOffset | 服务在指定时间之前没有源数据。
| wasThrottled              | Boolean        | 由于活动过多，某些数据未记录。

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->


