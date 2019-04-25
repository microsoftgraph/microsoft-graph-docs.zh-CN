---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
ms.openlocfilehash: dbb2fe0f651a269d69b880d18748b27a5b6f457c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525472"
---
# <a name="lookupcolumn-resource-type"></a>LookupColumn 资源类型

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
| **allowMultipleValues**   | 布尔 | 指示是否可以从源中选择多个值。
| **allowUnlimitedLength**  | boolean | 指示列中的值是否可以超过 255 个字符的标准限制。
| **columnName**            | string  | 查找源列的名称。
| **listId**                | string  | 查找源列表的唯一标识符。
| **primaryLookupColumnId** | string  | 如果已指定，则此列为*辅助查找*，同时从*主查找*查找的列表项中拉取一个附加字段。 使用*主查找*查找的列表项作为此处列出的列的源。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
