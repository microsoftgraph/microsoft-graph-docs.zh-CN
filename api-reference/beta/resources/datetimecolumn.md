---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
ms.openlocfilehash: 9854ad35c602ff474604f2ca88e7182c325e797d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042195"
---
# <a name="datetimecolumn-resource-type"></a>DateTimeColumn 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

[columnDefinition](columndefinition.md) 资源上的 **dateTimeColumn** 指示该列的值为日期或时间。

## <a name="json-representation"></a>JSON 表示形式

下面是 **dateTimeColumn** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a>属性

| 属性名称      | 类型               | 说明
|:-------------------|:-------------------|:----------------------------------------------
| **displayAs**      | string             | 值在用户体验中的显示方式。 必须为 `default`、`friendly` 或 `standard` 的其中一个。 有关详细信息，请参阅下文。 如果未指定，则视为 `default`。
| **format**         | string             | 指示值是否应该只显示为日期或日期和时间。 必须为 `dateOnly` 或 `dateTime` 的其中一个

## <a name="displayas-values"></a>DisplayAs 值

| 值        | 说明
|:-------------|:--------------------------------------------------------------
| **default**  | 使用用户体验中呈现的默认值。
| **friendly** | 使用友好相对表示形式（如 “今天下午 3:00”）
| **standard** | 使用标准绝对表示形式（如 “2017 年 5 月 10 日下午 3:20”）


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
