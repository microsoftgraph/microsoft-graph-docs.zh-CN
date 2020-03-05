---
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中的预期实体类型、基础源、分页参数、字段请求和实际搜索查询。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: fe3117eae0e514bea979281220da12820574cb4a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520897"
---
# <a name="searchrequest-resource-type"></a>searchRequest 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

要发送到查询终结点的搜索请求。 它包含响应中的预期实体类型、基础源、分页参数、字段请求和实际搜索查询。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|stored_fields|String 集合 |包含要为搜索 _so urces 对象返回的字段。 注释仅当在响应中指定了`externalItem` entityType = 时，这才适用。|
|contentSources|String 集合|包含要设定的连接。 <br>遵循以下格式：在`/external/connections/connectionid`连接器`connectionid`管理中定义 ConnectionId 的位置。 <br> 注释 contentSource 仅当 entityType =`externalItem`时适用。 |
|enableTopResults|布尔|这将触发邮件的混合排序：前3个邮件最相关<br> 这仅适用于 entityType =`message`。|
|entityTypes|`entityType` 集合| 可取值为：`event`、`message`、`driveItem`、`externalFile`、`externalItem`。|
|发件人|Int32|指定搜索结果的偏移量。 偏移量0返回的第一个结果。|
|查询|[searchQuery](searchquery.md)|包含查询词。|
|size|Int32|要检索的页面的大小。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchRequest",
  "baseType": null
}-->

```json
{
  "stored_fields": ["String"],
  "contentSources": ["String"],
  "entityTypes": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "enableTopResults": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
