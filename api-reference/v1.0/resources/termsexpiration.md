---
title: termsExpiration 资源类型
description: 提供协议计划到期的其他设置。
ms.localizationpriority: medium
ms.prod: governance
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: a3786a922bb5bbff220836b2a24abeb519bece38
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128051"
---
# <a name="termsexpiration-resource-type"></a>termsExpiration 资源类型

命名空间：microsoft.graph

提供协议计划到期的其他设置。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| startDateTime|DateTimeOffset | 协议设置为对所有用户过期的 DateTime。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
| frequency| 期限 | 表示术语在 **startDateTime** 中设置的首次过期后到期的频率。 该值以 ISO 8601 格式表示，持续时间为。 例如， `PT1M` 表示 1 个月的时间段。|

## <a name="json-representation"></a>JSON 表示形式

下面是此资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.termsExpiration",
}-->

```json
{
   "startDateTime": "2018-10-01T00:00:00.0000000Z",
   "frequency": "Duration"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "termsExpiration complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


