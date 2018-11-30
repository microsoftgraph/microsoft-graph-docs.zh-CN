---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: edb8d97094b4d26dbbcc008664bf5dfee3a4ddf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042807"
---
# <a name="columnlink-resource-type"></a>ColumnLink 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

[contentType][] 上的 **columnLink** 将网站 **columnDefinition** 附加到该内容类型。

[contentType]: contenttype.md

## <a name="json-representation"></a>JSON 表示形式

下面是 **columnLink** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| **id**        | string | 列的唯一标识符。
| **name**      | string | 此内容类型中的列的名称。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
