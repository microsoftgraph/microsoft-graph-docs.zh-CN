---
title: usageDetails 资源类型
description: 包含 Used 项的属性的复杂类型。 有关上次访问资源 (用户)  () 修改资源的信息。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 1fe25cc2bab141b3ac29e47b4bca80d8dc24fbe7be410be32398475c9e9a7d14
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54216838"
---
# <a name="usagedetails-resource-type"></a>usageDetails 资源类型

命名空间：microsoft.graph

包含 Used 项的属性 [的复杂](insights-used.md) 类型。 有关上次访问资源 (用户)  () 修改资源的信息。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usageDetails"
}-->

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a>属性

| 属性              | 类型          | 说明  |
| -------------         |---------------| -------------|
| lastAccessedDateTime                  | DateTimeOffset        | 用户上次访问资源的日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。 只读。                      |
| lastModifiedDateTime              | DateTimeOffset        | 用户上次修改资源的日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。 只读。       |

