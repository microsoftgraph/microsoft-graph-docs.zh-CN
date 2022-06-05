---
author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
ms.localizationpriority: medium
description: columnDefinition 资源上的 lookupColumn 指示从网站中的另一个源查找列的值。
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: e37f38f9dd42e962320cf5adad856193c4fc0037
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899413"
---
# <a name="lookupcolumn-resource-type"></a>LookupColumn 资源类型

命名空间：microsoft.graph

[columnDefinition](columndefinition.md) 资源上的 **lookupColumn** 指示从网站中的另一个源查找列的值。

## <a name="json-representation"></a>JSON 表示形式

下面是 **lookupColumn** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.lookupColumn" } -->

```json
{
  "allowMultipleValues": true,
  "allowUnlimitedLength": false,
  "columnName": "string",
  "listId": "string",
  "primaryLookupColumnId": "string"
}
```

## <a name="properties"></a>属性

| 属性名称             | 类型    | 说明
|:--------------------------|:--------|:---------------------------------------
| **allowMultipleValues**   | boolean | 指示是否可以从源中选择多个值。
| **allowUnlimitedLength**  | boolean | 指示列中的值是否可以超过 255 个字符的标准限制。
| **columnName**            | string  | 查找源列的名称。
| **listId**                | string  | 查找源列表的唯一标识符。
| **primaryLookupColumnId** | string  | 如果已指定，则此列为 *辅助查找*，同时从 *主查找* 查找的列表项中拉取一个附加字段。 使用 *主查找* 查找的列表项作为此处列出的列的源。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->

