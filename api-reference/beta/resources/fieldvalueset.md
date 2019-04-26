---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
ms.openlocfilehash: 4f8b193045bdc7c4e0286067c46c31693a66dfb4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340242"
---
# <a name="fieldvalueset-resource"></a>FieldValueSet 资源

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [listItem](listitem.md) 资源中的列值。

## <a name="json-representation"></a>JSON 表示形式

下面是 **fieldValueSet** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
       "keyProperty": "id", "openType": true } -->

```json
{
    "Author": "Brad Cleaver",
    "AuthorLookupId": "13",
    "Name": "Kangaroos and Wallabies: A Deep Dive",
    "Color": "Red",
    "Quantity": 350,
}
```

## <a name="properties"></a>属性

**listItem** 中的每个用户可见字段作为 **fieldValueSet** 中的名称/值对返回。
上面是针对包含**作者**、**名称**、**颜色**和**数量**这四列列表的一个示例。

默认情况下不返回查找字段（如上述 `Author`）。
相反，服务器会返回一个引用查找中锁定的 listItem 的“LookupId”字段（如上述 `AuthorLookupId`）。
“LookupId”字段的名称是原始字段名称，后跟 `LookupId`。

单个查询中可能请求最多 12 个查找字段。
如果请求包含带所需字段的 `select` 语句，服务器将返回查找值。
示例：

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

你可以在单个查询中请求最多 12 个查找字段以及任意数量的常规字段。

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet",
  "suppressions": []
}
-->
