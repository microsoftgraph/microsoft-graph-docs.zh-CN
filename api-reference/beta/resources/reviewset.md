---
title: reviewSet 资源类型
description: 表示为在诉讼、调查或管理法规请求中使用而收集的以电子方式存储的信息的静态集。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f1bf04c8357fbd57876b460848c549b3edd6f1f7
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48400738"
---
# <a name="reviewset-resource-type"></a>reviewSet 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示为在诉讼、调查或管理法规请求中使用而收集的以电子方式存储的信息的静态集。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/reviewset-list.md) | [reviewSet](reviewset.md) 集合 | 获取审阅集的集合。 |
| [获取](../api/reviewset-get.md) | [reviewSet](reviewset.md) | 读取 **reviewSet** 对象的属性和关系。 |
| [创建](../api/reviewset-post.md) | [reviewSet](reviewset.md) | 创建新的审阅集。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|createdBy| [identitySet](/graph/api/resources/identityset) | 创建评审集的用户。 只读。 |
|createdDateTime|DateTimeOffset| 创建评审集时的日期时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。 |
|displayName|字符串| 审阅集名称。 名称是唯一的，最大限制为64个字符。 |
|id|字符串| 审阅集的唯一标识符。 只读。 |

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
| 审阅集查询 |[reviewSetQuery](reviewsetquery.md) 集合| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSet",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->