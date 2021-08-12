---
author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
description: columnDefinition 资源上的 lookupColumn 指示从网站中的另一个源查找列的值。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7a619323598f3e648341ba533371f9a9c56026ab7ffa6196313aaaec13e39c74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149756"
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

