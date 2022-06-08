---
title: ediscoveryReviewSetQuery 资源类型
description: 表示一个审阅集查询，该查询用于查询和剔除电子数据展示 reviewSet 中存储的数据。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 245a998a9d5c853ddadcc6b1a194e276ad4759c0
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945161"
---
# <a name="ediscoveryreviewsetquery-resource-type"></a>ediscoveryReviewSetQuery 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个审阅集查询，该查询用于查询和剔除电子数据展示 [reviewSet](security-ediscoveryreviewset.md) 中存储的数据。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 ediscoveryReviewSetQueries](../api/security-ediscoveryreviewset-list-queries.md)|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) 集合|获取 [ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) 对象及其属性的列表。|
|[创建 ediscoveryReviewSetQuery](../api/security-ediscoveryreviewset-post-queries.md)|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|创建新的 [ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) 对象。|
|[获取 ediscoveryReviewSetQuery](../api/security-ediscoveryreviewsetquery-get.md)|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|读取 [ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) 对象的属性和关系。|
|[更新 ediscoveryReviewSetQuery](../api/security-ediscoveryreviewsetquery-update.md)|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|更新 [ediscoveryReviewSetQuery 对象的](../resources/security-ediscoveryreviewsetquery.md) 属性。|
|[删除 ediscoveryReviewSetQuery](../api/security-ediscoveryreviewset-delete-queries.md)|无|删除 [ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) 对象。|
|[出口](../api/security-ediscoveryreviewsetquery-export.md)|无|从审阅集中导出与指定查询匹配的文档。|
|[applyTags](../api/security-ediscoveryreviewsetquery-applytags.md)|无|将标记应用到与指定查询匹配的文档。|
|[运行](../api/security-ediscoveryreviewsetquery-run.md)|[microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md) 集合|从查询中获取文件。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| createdBy | [identitySet](/graph/api/resources/identityset) | 创建查询的用户。 |
| createdDateTime |DateTimeOffset| 创建查询的时间和日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
| displayName | String | 查询的名称。|
| id |字符串| 查询的唯一标识符。 只读。|
| lastModifiedBy | [identitySet](/graph/api/resources/identityset) | 上次修改查询的用户。 |
| lastModifiedDateTime |DateTimeOffset | 上次修改查询的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
| 查询 | String | KQL (关键字查询语言) 查询中的查询字符串。 有关详细信息，请参阅 [高级电子数据展示中的“文档元数据”字段](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)。  此字段直接映射到关键字条件。  可以使用与值配对的 *可搜索字段名称* 中列出的字段来优化搜索;例如， *subject：“Quarterly Financials” AND Date>=06/01/2016 AND Date<=07/01/2016*. |


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryReviewSetQuery",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryReviewSetQuery",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "contentQuery": "String"
}
```

