---
title: case 资源类型
description: 在电子数据展示的上下文中，包含保管人、保留项、集合、审阅集和导出。
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 8c38006d4794463fd7960706e0afa1320302321f
ms.sourcegitcommit: 94dc71a6d4fbdc46f2681a1add13416bc9b4a6e9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2021
ms.locfileid: "60115282"
---
# <a name="case-resource-type"></a>case 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在电子数据展示的上下文中，包含保管人、保留项、集合、审阅集和导出。 有关详细信息[，请参阅](/microsoft-365/compliance/overview-ediscovery-20)Advanced eDiscovery。

>[!NOTE]
>从 2021 年 9 月开始，POST 操作将创建大案例。 若要了解有关大案例的更多信息，请参阅在 Advanced eDiscovery[中Advanced eDiscovery。](/microsoft-365/compliance/advanced-ediscovery-large-cases) 有关详细信息，请参阅高级电子数据展示[Microsoft 365案例 API](https://go.microsoft.com/fwlink/?linkid=2172604)的变更博客文章。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出事例](../api/ediscovery-case-list.md) | [microsoft.graph.ediscovery.case](ediscovery-case.md) 集合 | 检索 case [对象](../resources/ediscovery-case.md) 的列表。|
| [创建案例](../api/ediscovery-case-post.md) | [microsoft.graph.ediscovery.case](ediscovery-case.md) | 创建新的 **case** 对象。 |
| [获取案例](../api/ediscovery-case-get.md) | [microsoft.graph.ediscovery.case](ediscovery-case.md) | 检索 case **对象的属性和** 关系。 |
| [更新案例](../api/ediscovery-case-update.md) | [microsoft.graph.ediscovery.case](ediscovery-case.md) | 更新 **case** 对象的属性。 |
| [删除大小写](../api/ediscovery-case-delete.md) | 无 | 删除 **case** 对象。 |
| [关闭案例](../api/ediscovery-case-close.md)        | 无                                              | 关闭电子数据展示案例。 有关详细信息，请参阅 [关闭案例](/microsoft-365/compliance/close-or-delete-case#close-a-case)。 |
| [重新打开案例](../api/ediscovery-case-reopen.md)      | 无                                              | 重新打开已关闭电子数据展示案例。 有关详细信息，请参阅 [重新打开已关闭的案例](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case)。|
| Custodians |
| [列出保管人](../api/ediscovery-case-list-custodians.md)   | [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) 集合 |获取保管 [人对象及其](../resources/ediscovery-custodian.md) 属性的列表。|
| [创建保管人](../api/ediscovery-case-post-custodians.md)  | [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)           |创建新的保管 [人](../resources/ediscovery-custodian.md) 对象。 创建保管人对象后，你需要创建保管人[的用户来源](../resources/ediscovery-usersource.md)，以引用其邮箱和OneDrive for Business网站。|
| 合法保留 |
| [列出 legalHolds](../api/ediscovery-case-list-legalholds.md)   | [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) 集合 | 获取[适用于案例的 legalHolds。](../resources/ediscovery-legalhold.md)|
| [创建 legalHold](../api/ediscovery-case-post-legalholds.md)  | [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)           | 创建新的 [legalHold](../resources/ediscovery-legalhold.md) 对象。|
| 审阅集 |
| [列出 reviewSets](../api/ediscovery-case-list-reviewsets.md)   | [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) 集合 | 从 case [对象获取 reviewSets](../resources/ediscovery-reviewset.md)**列表。**|
| [创建 reviewSet](../api/ediscovery-case-post-reviewsets.md)  | [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md)           | 创建新的 [reviewSet](../resources/ediscovery-reviewset.md) 对象。 请求正文包含显示名称审阅集的唯一可写属性的正文。|
| 案例设置 |
| [获取设置](../api/ediscovery-settings-get.md)|[microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md)|读取 [microsoft.graph.ediscovery.settings 对象的属性和](../resources/ediscovery-settings.md) 关系。 |
| [更新设置](../api/ediscovery-settings-update.md)|[microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md)|更新 [microsoft.graph.ediscovery.settings 对象](../resources/ediscovery-settings.md) 的属性。 |
| [resetToDefault](../api/ediscovery-settings-resettodefault.md)|无|将所有设置重置为默认值。 |
| 源集合 |
| [列出 sourceCollections](../api/ediscovery-case-list-sourcecollections.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) 集合|从[case 对象获取 sourceCollection。](../resources/ediscovery-sourcecollection.md) |
| [创建 sourceCollection](../api/ediscovery-case-post-sourcecollections.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|创建新的 **sourceCollection** 对象。|
| 标记 |
| [列出标记](../api/ediscovery-case-list-tags.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合|从电子数据展示 [案例](../resources/ediscovery-tag.md) 检索标记对象列表。|
| [创建标记](../api/ediscovery-case-post-tags.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|为指定案例创建新标记。 标记在审阅内容时用于审阅集。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|closedBy|[identitySet](/graph/api/resources/identityset)|关闭案例的用户。|
|closedDateTime|DateTimeOffset|案例关闭的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|createdBy|[identitySet](/graph/api/resources/identityset)|创建案例的用户。|
|createdDateTime|DateTimeOffset|实体的创建日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|说明|String|案例描述。|
|displayName|字符串|大小写名称。|
|externalId|String|客户参考的外部案例编号。|
|id|String| 电子数据展示案例的 ID。 只读。 |
|lastModifiedBy|[identitySet](/graph/api/resources/identityset)|最后一个修改实体的用户。|
|lastModifiedDateTime|DateTimeOffset| 修改案例的最新日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|status|microsoft.graph.ediscovery.caseStatus| 大小写状态。 可能的值为 `unknown` `active` `pendingDelete` 、、、、 `closing` 和 `closed` `closedWithError` 。 有关详细信息，请参阅下表。|

### <a name="casestatus-values"></a>caseStatus 值

|成员|说明|
|:----|-----------|
| unknown | 案例状态未知。 |
| active | 案例处于活动状态。 |
| pendingDelete | 案例已被删除，但删除操作尚未完全处理。 |
| closing | 案例已关闭，但操作尚未完全处理。 |
| closed | 案例已关闭。 |
| closedWithError | 案例已关闭，但在这种情况下释放保留时出现错误。 |

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|custodians|[microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) 集合| 返回此案例的 **case custodian** 对象 **列表**。  可为 Null。|
|legalHolds|[microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) 集合| 返回此案例的 **case legalHold** 对象 **列表**。  可为 Null。 |
|noncustodialDataSources|[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 集合| 返回大小写非 **custodialDataSource** **对象的列表。**  可为 NULL。 |
|operations|[microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md) 集合| 返回此案例的 **case 操作** 对象 **列表**。 可为 Null。 |
|reviewSets|[microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) 集合| 返回一个 **reviewSet** 对象列表（在这种情况下）。 只读。 可为 Null。 |
|设置|[microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md) 集合| 返回在这种情况下 **的设置** 对象列表。 只读。 可为 Null。 |
|sourceCollections|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) 集合|返回与 **这种情况相关联的 sourceCollection** 对象的列表。|
|标记|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合|返回与这种情况 **相关联的 tag** 对象列表。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
 
  ],
  "@odata.type": "microsoft.graph.ediscovery.case"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.case",
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
  "description": "case resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
