---
title: reviewSet 资源类型
description: 代表收集用于诉讼、调查或监管请求的静态存储信息集。
ms.localizationpriority: medium
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c8e7f51e32a48556ece3d5bfd34b3224b50b8b70
ms.sourcegitcommit: e75969aa44a1aab722ac44d09c37508ffbad8738
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2021
ms.locfileid: "61307620"
---
# <a name="reviewset-resource-type"></a>reviewSet 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示收集用于诉讼、调查或监管请求的静态存储信息集。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 reviewSets](../api/ediscovery-case-list-reviewsets.md) | [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) 集合 | 获取 **reviewSet 对象** 的集合。 |
| [创建 reviewSet](../api/ediscovery-case-post-reviewsets.md) | [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) | 创建新的 **reviewSet**。 |
| [获取 reviewSet](../api/ediscovery-reviewset-get.md) | [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) | 读取 **reviewSet** 对象的属性和关系。 |
| [列出查询](../api/ediscovery-reviewsetquery-list.md)|[microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) 集合|获取 **reviewSetQuery 资源** 的列表。|
| [export](../api/ediscovery-reviewset-export.md) | 无 | 启动从审阅集 导出 **数据**。 |
| [addToReviewSet](../api/ediscovery-reviewset-addtoreviewset.md)|无|将数据从 **sourceCollection** 添加到 **审阅集**。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|createdBy        | [identitySet](/graph/api/resources/identityset) | 创建审阅集的用户。 只读。 |
|createdDateTime  |DateTimeOffset| 创建审阅集的日期/时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |
|displayName      |String| 审阅集名称。 名称是唯一的，最大限制为 64 个字符。 |
|id               |String| 审阅集唯一标识符。 只读。 |

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
| 查询 |[microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) 集合| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ediscovery.reviewSet",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.reviewSet",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
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
