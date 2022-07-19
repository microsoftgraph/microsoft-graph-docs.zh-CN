---
title: ediscoveryCase 资源类型
description: 在电子数据展示的上下文中，包含保管人、保存、集合和审阅集。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 3348c6c718a1ccd23977b4b1164cc21111198eac
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839449"
---
# <a name="ediscoverycase-resource-type"></a>ediscoveryCase 资源类型

命名空间：microsoft.graph.security



在电子数据展示的上下文中，包含保管人、搜索、审阅集。 有关详细信息，请参阅[Microsoft Purview 电子数据展示 (高级) 概述](/microsoft-365/compliance/overview-ediscovery-20)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 ediscoveryCases](../api/security-casesroot-list-ediscoverycases.md)|[microsoft.graph.security.ediscoveryCase](../resources/security-ediscoverycase.md) 集合|获取 [ediscoveryCase](../resources/security-ediscoverycase.md) 对象及其属性的列表。|
|[创建 ediscoveryCase](../api/security-casesroot-post-ediscoverycases.md)|[microsoft.graph.security.ediscoveryCase](../resources/security-ediscoverycase.md)|创建新的 [ediscoveryCase](../resources/security-ediscoverycase.md) 对象。|
|[获取 ediscoveryCase](../api/security-ediscoverycase-get.md)|[microsoft.graph.security.ediscoveryCase](../resources/security-ediscoverycase.md)|读取 [ediscoveryCase](../resources/security-ediscoverycase.md) 对象的属性和关系。|
|[更新 ediscoveryCase](../api/security-ediscoverycase-update.md)|[microsoft.graph.security.ediscoveryCase](../resources/security-ediscoverycase.md)|更新 [ediscoveryCase 对象的](../resources/security-ediscoverycase.md) 属性。|
|[删除 ediscoveryCase](../api/security-casesroot-delete-ediscoverycases.md)|无|删除 [ediscoveryCase](../resources/security-ediscoverycase.md) 对象。|
|[列出保管人](../api/security-ediscoverycase-list-custodians.md)|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md) 集合|从保管人导航属性获取 ediscoveryCustodian 资源。|
|[创建 ediscoveryCustodian](../api/security-ediscoverycase-post-custodians.md)|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|创建新的 ediscoveryCustodian 对象。|
|[列出 noncustodialDataSources](../api/security-ediscoverysearch-list-noncustodialsources.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) 集合|从 noncustodialDataSources 导航属性获取 ediscoveryNoncustodialDataSource 资源。|
|[创建 ediscoveryNoncustodialDataSource](../api/security-ediscoverycase-post-noncustodialdatasources.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|创建新的 ediscoveryNoncustodialDataSource 对象。|
|[列举操作](../api/security-ediscoverycase-list-operations.md)|[microsoft.graph.security.caseOperation](../resources/security-caseoperation.md) 集合|从操作导航属性获取 caseOperation 资源。|
|[列出 reviewSets](../api/security-ediscoverycase-list-reviewsets.md)|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) 集合|从 reviewSets 导航属性获取 ediscoveryReviewSet 资源。|
|[创建 ediscoveryReviewSet](../api/security-ediscoverycase-post-reviewsets.md)|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|创建新的 ediscoveryReviewSet 对象。|
|[列出搜索](../api/security-ediscoverycase-list-searches.md)|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md) 集合|从搜索导航属性获取 ediscoverySearch 资源。|
|[创建 ediscoverySearch](../api/security-ediscoverycase-post-searches.md)|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|创建新的 ediscoverySearch 对象。|
|[列出标记](../api/security-ediscoverycase-list-tags.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 集合|从标记导航属性获取 ediscoveryReviewTag 资源。|
|[创建 ediscoveryReviewTag](../api/security-ediscoverycase-post-tags.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|创建新的 ediscoveryReviewTag 对象。|

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|closedBy|[microsoft.graph.identitySet](../resources/identityset.md)|结案的用户。|
|closedDateTime|DateTimeOffset|结案的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|createdBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|创建案例的用户。|
|createdDateTime|DateTimeOffset|创建实体的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|说明|String|事例说明。|
|displayName|String|事例名称。|
|externalId|String|客户引用的外部事例号。|
|id|String|电子数据展示案例的 ID。 只读。 |
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|修改案例的最后一个用户。
|lastModifiedDateTime|DateTimeOffset|修改案例的最新日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|status|microsoft.graph.security.caseStatus|事例状态。 可能的值包括`unknown`、`active`、`pendingDelete`、`closed``closing`和 `closedWithError`。 有关详细信息，请参阅下表。

### <a name="casestatus-values"></a>caseStatus 值

|成员|说明|
|:----|-----------|
| unknown | 事例状态未知。 |
| 积极 | 案例处于活动状态。 |
| pendingDelete | 案例已删除，但删除尚未完全处理。 |
| 关闭 | 案例已结案，但操作尚未完全处理。 |
| 关闭 | 案件已结案。 |
| closedWithError | 案件已结案，但该案存在释放保留的错误。 |

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|保管员|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md) 集合|返回此 **事例** 的案例 **ediscoveryCustodian** 对象的列表。|
|noncustodialDataSources|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) 集合|返回 **这种情况的** 案例 **ediscoveryNoncustodialDataSource** 对象的列表。|
|operations|[microsoft.graph.security.caseOperation](../resources/security-caseoperation.md) 集合|返回此 **事例** 的 **caseOperation** 对象列表。|
|reviewSets|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) 集合|返回本例中 **电子数据展示ReviewSet** 对象的列表。|
|搜索|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md) 集合|返回与此事例关联的 **电子数据展示Search** 对象的列表。|
|settings|[microsoft.graph.security.ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md)|返回 **在这种情况下的 eDIscoverySettings** 对象的列表。|
|tags|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 集合|返回与这种情况关联的 **ediscoveryReviewTag** 对象的列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryCase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryCase",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "closedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "closedDateTime": "String (timestamp)",
  "externalId": "String"
}
```

