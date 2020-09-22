---
title: usageDetails 资源类型
description: 包含已使用项的属性的复杂类型。 有关上次访问资源的时间的信息 (查看由用户) 编辑的) 或修改的 (。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 79007d71ef44971bfab250c22abc6795a6b38dd4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054761"
---
# <a name="usagedetails-resource-type"></a>usageDetails 资源类型

命名空间：microsoft.graph

包含已 [使用](insights-used.md) 项的属性的复杂类型。 有关上次访问资源的时间的信息 (查看由用户) 编辑的) 或修改的 (。


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
| lastAccessedDateTime                  | DateTimeOffset        | 用户上次访问该资源的日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。 只读。                      |
| lastModifiedDateTime              | DateTimeOffset        | 用户上次修改资源的日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。 只读。       |

