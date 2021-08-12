---
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中预期的实体类型、基础源、分页参数、字段请求和实际搜索查询。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ec5ce984ac98c34c219e87e956a3e102ca5834ad39c748f17af33fcb1db79740
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196542"
---
# <a name="searchrequest-resource-type"></a>searchRequest 资源类型

命名空间：microsoft.graph

JSON blob 中格式化的搜索请求。 

JSON blob 包含响应中预期的资源类型、基础源、分页参数、排序选项、请求的聚合和字段以及实际搜索查询。 请参阅 [各种](#see-also) 资源上的搜索请求示例。

> [!NOTE]
> 请注意搜索 [实体](search-api-overview.md#known-limitations) 类型的特定组合以及排序或聚合搜索结果的已知限制。


## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |             |
|:-------------|:------------|:------------|:------------|
|contentSources|String collection|包含要定向的连接。|
|enableTopResults|Boolean|这将触发邮件的混合排序：前 3 个邮件最相关。 此属性仅适用于 entityType= `message` 。 可选。|
|entityTypes|entityType 集合| 响应中预期的一种或多种资源类型。 可取值为：`list`、`site`、`listItem`、`message`、`event`、`drive`、`driveItem`、`externalItem`。 有关 [同一](search-api-overview.md#known-limitations) 搜索请求中支持的两个或多个实体类型的组合，请参阅已知限制。 必填。|
|fields|String collection |包含为 **entityTypes** 中指定的每个资源对象返回的字段，允许自定义默认情况下返回的字段，包括其他字段，如 SharePoint 和 OneDrive。 可选。|
|起始数量|Int32|指定搜索结果的偏移量。 偏移量 0 返回第一个结果。 可选。|
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
- 搜索 [邮件](/graph/search-concept-messages)
- 搜索 [日历事件](/graph/search-concept-events)
- 搜索网站[SharePoint OneDrive (、列表和网站) ](/graph/search-concept-files)



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


