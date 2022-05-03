---
author: JeremyKelley
description: columnDefinition 资源上的 lookupColumn 指示从网站中的另一个源查找列的值。
ms.date: 09/11/2017
title: LookupColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: d5ddc59f00b171d6ba7d125e8a626aa97ddcfff9
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176555"
---
# <a name="lookupcolumn-resource-type"></a>LookupColumn 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

| 属性                  | 类型    | Description                                                                                                                                                                                                                |
| :------------------------ | :------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **allowMultipleValues**   | boolean | 指示是否可以从源中选择多个值。                                                                                                                                                         |
| **allowUnlimitedLength**  | boolean | 指示列中的值是否可以超过 255 个字符的标准限制。                                                                                                                      |
| **columnName**            | string  | 查找源列的名称。                                                                                                                                                                                      |
| **listId**                | string  | 查找源列表的唯一标识符。                                                                                                                                                                           |
| **primaryLookupColumnId** | string  | 如果已指定，则此列为 *辅助查找*，同时从 *主查找* 查找的列表项中拉取一个附加字段。 使用 *主查找* 查找的列表项作为此处列出的列的源。 |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn",
  "suppressions": []
}
-->
