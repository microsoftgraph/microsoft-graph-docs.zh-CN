---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
ms.openlocfilehash: 4319ab0f36e12ddd28ca9bb6c7bfd48043228504
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042516"
---
# <a name="incompletedata-resource-type"></a>incompleteData 资源类型

 > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**IncompleteData**方面指示资源生成不完整的数据。
内的属性可能提供有关信息，为什么不完整数据。

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
| missingDataBeforeDateTime | DateTimeOffset | 该服务不具有之前指定的时间的源数据。
| wasThrottled              | 布尔        | 由于活动太多而未录制一些数据。

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData"
} -->
