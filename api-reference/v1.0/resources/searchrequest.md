---
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中的预期实体类型、基础源、分页参数、字段请求和实际搜索查询。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f673c551ce27c16fd4fddabc26e55cd234a9f19e
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377970"
---
# <a name="searchrequest-resource-type"></a>searchRequest 资源类型

命名空间：microsoft.graph

JSON blob 中格式化的搜索请求。 

JSON blob 包含响应中预期的资源类型、基础源、分页参数、排序选项、请求的聚合和字段以及实际搜索查询。 请参阅各种资源上的搜索请求的 [示例](#see-also) 。

> [!NOTE]
> 了解有关搜索实体类型的特定组合以及对搜索结果进行排序或聚合的 [已知限制](search-api-overview.md#known-limitations) 。


## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|:------------|
|contentSources|String collection|包含要设定的连接。|
|enableTopResults|Boolean|这将触发邮件的混合排序：前3个邮件最相关。 此属性仅适用于 entityType = `message` 。 可选。|
|entityTypes|entityType 集合| 响应中预期的一种或多种类型的资源。 可取值为：`list`、`site`、`listItem`、`message`、`event`、`drive` 或 `driveItem`。 请参阅相同搜索请求中支持的两个或更多实体类型的组合的 [已知限制](search-api-overview.md#known-limitations) 。 必填。|
|fields|String collection |包含要为 **entityTypes** 中指定的每个资源对象返回的字段，允许自定义默认情况下返回的字段，包括其他字段，如来自 SharePoint 和 OneDrive 的自定义托管属性。 可选。|
|起始数量|Int32|指定搜索结果的偏移量。 偏移量0返回的第一个结果。 可选。|
|查询|[searchQuery](searchquery.md)|包含查询词。 必填。|
|大小|Int32|要检索的页面的大小。 可选。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

```json
{
  "entityTypes": ["String"],
  "contentSources": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "fields": ["String"],
  "enableTopResults": true  
}
```

## <a name="see-also"></a>另请参阅
- 搜索 [邮件消息](/graph/search-concept-messages)
- 搜索 [日历事件](/graph/search-concept-events)
- 在 SharePoint 和 OneDrive 中搜索内容 ([文件、列表和网站](/graph/search-concept-files)) 



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


