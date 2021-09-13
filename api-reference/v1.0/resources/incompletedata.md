---
author: daspek
title: incompleteData 资源类型
description: incompleteData Facet 指示生成的资源包含不完整的数据。
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f4d8c852a08780ecc0f48ac8a1dcef11b246673c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128310"
---
# <a name="incompletedata-resource-type"></a>incompleteData 资源类型

命名空间：microsoft.graph

**incompleteData** Facet 指示生成的资源包含不完整的数据。
中的属性可能会提供有关数据不完整的原因的信息。

## <a name="properties"></a>属性

| 属性                  | 类型           | 说明
|:--------------------------|:---------------|:--------------------------------
| missingDataBeforeDateTime | DateTimeOffset | 服务在指定的时间之前没有源数据。
| wasThrottled              | Boolean        | 由于活动过多，某些数据未记录。

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

