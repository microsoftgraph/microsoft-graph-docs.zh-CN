---
title: ediscoveryCase 资源类型
description: 电子数据展示事例是包含保管人、保留、集合、审阅集和导出的容器。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 12d2901ff6a61213affd14d681c0ec7b6a74470c
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597401"
---
# <a name="ediscoverycase-resource-type"></a>ediscoveryCase 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

电子数据展示事例是包含保管人、保留、集合、审阅集和导出的容器。  了解有关案例和 [高级电子数据展示](/microsoft-365/compliance/overview-ediscovery-20)的详细信息。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [列出 ediscoveryCases](../api/ediscoverycase-list.md)          | [ediscoveryCase](ediscoverycase.md) 集合   | 获取电子数据展示事例的列表。|
| [获取 ediscoveryCase](../api/ediscoverycase-get.md)            | [ediscoveryCase](ediscoverycase.md)               | 阅读电子数据展示事例属性。 |
| [创建 ediscoveryCase](../api/ediscoverycase-post.md)        | [ediscoveryCase](ediscoverycase.md)               | 通过发布到事例集合创建新的 **ediscoveryCase** 。 |
| [更新 ediscoveryCase](../api/ediscoverycase-update.md)      | [ediscoveryCase](ediscoverycase.md)               | 更新电子数据展示事例。 |
| [删除 ediscoveryCase](../api/ediscoverycase-delete.md)      | 无                                              | 删除电子数据展示事例。 |
| [关闭 ediscoveryCase](../api/ediscoverycase-close.md)        | 无                                              | 关闭电子数据展示事例。 |
| [重新打开 ediscoveryCase](../api/ediscoverycase-reopen.md)      | 无                                              | 重新打开已关闭的电子数据展示事例。|
| [列出保管人](../api/custodian-get.md)   | [保管人](../resources/custodian.md) 集合 |从保管人导航属性中获取保管人资源。|
| [创建保管人](../api/ediscoverycase-post-custodians.md)  | [保管人](../resources/custodian.md)           |创建新的保管人对象。|
| [列出 reviewSets](../api/reviewset-list.md)   | [reviewSet](../resources/reviewset.md) 集合 | 从 reviewSets 导航属性中获取 reviewSet 资源。|
| [创建 reviewSets](../api/reviewset-post.md)  | [reviewSet](../resources/reviewset.md)           | 创建新的 reviewSet 对象。|

## <a name="properties"></a>属性

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|closedBy|[identitySet](/graph/api/resources/identityset)|关闭该事例的用户。|
|closedDateTime|DateTimeOffset|关闭事例的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|createdBy|[identitySet](/graph/api/resources/identityset)|创建案例的用户。|
|createdDateTime|DateTimeOffset|实体的创建日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|说明|String|事例说明。|
|displayName|String|事例名称。|
|externalId|String|Customer reference 的外部事例编号。|
|id|String| 电子数据展示事例的 ID。 只读。 |
|lastModifiedBy|[identitySet](/graph/api/resources/identityset)|上次修改实体的用户。|
|lastModifiedDateTime|DateTimeOffset| 修改事例的最新日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|status|String| 案例状态。 可能的值为、、、、 `unknown` `active` `pendingDelete` `closing` `closed` 和 `closedWithError` 。 有关详细信息，请参阅下表。|

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

| 关系 | 类型        | Description |
|:-------------|:------------|:------------|
|保管人|[保管人](../resources/custodian.md) 集合| 组织中可能拥有与案例相关的数据的人员。 |
|reviewSets|[reviewSet](reviewset.md) 集合| 案例中的审阅集集合。 只读。 可为 Null。 |

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
  "@odata.type": "#microsoft.graph.ediscoveryCase",
  "description": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "closedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "closedDateTime": "String (timestamp)",
  "externalId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
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
