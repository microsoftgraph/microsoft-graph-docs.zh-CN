---
title: ediscoveryCase 资源类型
description: 电子数据展示事例是包含保管人、保留、集合、审阅集和导出的容器。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 930d04449f24d05d8c9225869506bfc1ed2720aa
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510025"
---
# <a name="ediscoverycase-resource-type"></a>ediscoveryCase 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

电子数据展示事例是包含保管人、保留、集合、审阅集和导出的容器。  了解有关案例和[高级电子数据展示](https://docs.microsoft.com/microsoft-365/compliance/overview-ediscovery-20)的详细信息。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [List](../api/ediscoverycase-list.md) | [ediscoveryCase](ediscoverycase.md)集合 | 获取电子数据展示事例的列表。|
| [获取](../api/ediscoverycase-get.md) | [ediscoveryCase](ediscoverycase.md) | 阅读电子数据展示事例属性。 |
| [创建](../api/ediscoverycase-post.md) | [ediscoveryCase](ediscoverycase.md) | 通过发布到事例集合创建新的**ediscoveryCase** 。 |
| [更新](../api/ediscoverycase-update.md) | [ediscoveryCase](ediscoverycase.md) | 更新电子数据展示事例。 |
| [删除](../api/ediscoverycase-delete.md) | 无 | 删除电子数据展示事例。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|closedBy|[identitySet](https://docs.microsoft.com/graph/api/resources/identityset)|关闭该事例的用户。|
|closedDateTime|DateTimeOffset|关闭事例的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|createdBy|[identitySet](https://docs.microsoft.com/graph/api/resources/identityset)|创建案例的用户。|
|createdDateTime|DateTimeOffset|实体的创建日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|说明|字符串|事例说明。|
|displayName|字符串|事例名称。|
|externalId|String|Customer reference 的外部事例编号。|
|id|String| 电子数据展示事例的 ID。 只读。 |
|lastModifiedBy|[identitySet](https://docs.microsoft.com/graph/api/resources/identityset)|上次修改实体的用户。|
|lastModifiedDateTime|DateTimeOffset| 修改事例的最新日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|状态|字符串| 案例状态。 可能的值为、、、、 `unknown` `active` `pendingDelete` `closing` `closed` 和 `closedWithError` 。 有关详细信息，请参阅下表。|

### <a name="casestatus-values"></a>caseStatus 值

|成员|说明|
|:----|-----------|
| unknown | 未知的案例状态。 |
| 工作 | 案例处于活动状态。 |
| pendingDelete | 已删除事例，但尚未完全处理该删除。 |
| 结束语 | 事例已关闭，但操作尚未完全进行事务处理。 |
| 停止 | 事例已关闭。 |
| closedWithError | 事例已关闭，但在这种情况下释放保留时出现错误。 |

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|评审集|[reviewSet](reviewset.md)集合| 案例中的审阅集集合。 只读。 可为 Null。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
 
  ],
  "@odata.type": "microsoft.graph.ediscoveryCase"
}-->

```json
{
  "closedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "closedDateTime": "String (timestamp)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "status": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ediscoveryCase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
