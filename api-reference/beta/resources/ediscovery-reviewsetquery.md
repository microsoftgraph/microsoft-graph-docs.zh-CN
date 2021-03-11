---
title: reviewSetQuery 资源类型
description: 表示审阅集查询，用于查询和剔除电子数据展示 reviewSet 中存储的数据。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 8eb674ed70eac47d4e29d127ebfc9f48b7b988a1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720317"
---
# <a name="reviewsetquery-resource-type"></a>reviewSetQuery 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示审阅集查询，用于查询和剔除电子数据展示 [reviewSet 中存储的数据](ediscovery-reviewset.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出查询](../api/ediscovery-reviewsetquery-list.md) | [microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) 集合 | 在审阅集内列出审阅集查询。 |
| [创建查询](../api/ediscovery-reviewsetquery-post.md) | [microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) | 创建新的审阅集查询。 |
| [获取查询](../api/ediscovery-reviewsetquery-get.md) | [microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) | 读取 **reviewSetQuery** 对象的属性和关系。 |
| [更新 reviewSetQuery](../api/ediscovery-reviewsetquery-update.md) | 无 | 更新审阅集查询。 |
| [删除 reviewSetQuery](../api/ediscovery-reviewsetquery-delete.md) | 无 | 删除审阅集查询。 |
| [applyTags](../api/ediscovery-reviewsetquery-applytags.md)|无|将标记应用于与指定查询匹配的文档。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| createdBy | [identitySet](/graph/api/resources/identityset) | 创建查询的用户。 |
| createdDateTime |DateTimeOffset| 创建查询的时间和日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
| displayName | String | 查询的名称。|
| id |String| 查询的唯一标识符。 只读。|
| lastModifiedBy | [identitySet](/graph/api/resources/identityset) | 上次修改查询的用户。 |
| lastModifiedDateTime |DateTimeOffset | 上次修改查询的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
| 查询 | String | KQL 中的查询字符串 (关键字查询语言) 查询。 有关详细信息，请参阅 [高级电子数据展示中的文档元数据字段](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)。  此字段直接映射到关键字条件。  您可以使用与值配对的可搜索字段 *名称中列出的字段来* 优化搜索;例如 *，subject："Quarterly Financials" and Date>=06/01/2016 AND Date<=07/01/2016*. |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.reviewSetQuery",
  "query": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSetQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
