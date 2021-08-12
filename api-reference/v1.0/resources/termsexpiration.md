---
title: termsExpiration 资源类型
description: 提供协议计划到期的其他设置。
localization_priority: Normal
ms.prod: governance
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: cd1e7f437e8bf942d69368bc4c78410eed95dd2e42ac0a0f0dd77319578d0991
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54174869"
---
# <a name="termsexpiration-resource-type"></a>termsExpiration 资源类型

命名空间：microsoft.graph

提供协议计划到期的其他设置。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| startDateTime|DateTimeOffset | 协议设置为对所有用户过期的 DateTime。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。|
| frequency| 期限 | 表示术语在 **startDateTime** 中设置的首次过期后到期的频率。 该值以 ISO 8601 格式表示持续时间。 例如， `PT1M` 表示 1 个月的时间段。|

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


