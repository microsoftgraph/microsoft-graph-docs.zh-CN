---
title: usageDetails 资源类型
description: 包含使用项目的属性的复杂类型。 上次访问该资源的信息 （查看） 和修改用户 （编辑）。
author: simonhult
ms.openlocfilehash: ef5efcfce439e9d08784637cb02657d7cd37adf7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349348"
---
# <a name="usagedetails-resource-type"></a>usageDetails 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

包含[用于](insights-used.md)项目的属性的复杂类型。 上次访问该资源的信息 （查看） 和修改用户 （编辑）。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a>属性

| 属性              | 类型          | 说明  |
| -------------         |---------------| -------------|
| lastAccessedDateTime                  | DateTimeOffset        | 日期和时间用户上次访问资源。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。 只读。                      |
| lastModifiedDateTime              | DateTimeOffset        | 日期和时间用户上次修改资源。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。 只读。       |