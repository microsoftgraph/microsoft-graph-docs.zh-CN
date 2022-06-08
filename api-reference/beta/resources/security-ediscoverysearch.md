---
title: ediscoverySearch 资源类型
description: 表示电子数据展示搜索。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: d32540ccfd74f79fdad282f7d708a458bdf7705f
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945156"
---
# <a name="ediscoverysearch-resource-type"></a>ediscoverySearch 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示电子数据展示搜索。 有关详细信息，请参阅 [电子数据展示 (高级) 中的案例收集数据 ](/microsoft-365/compliance/collecting-data-for-ediscovery)。


## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 ediscoverySearches](../api/security-ediscoverycase-list-searches.md)|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md) 集合|获取 [ediscoverySearch](../resources/security-ediscoverysearch.md) 对象及其属性的列表。|
|[创建 ediscoverySearch](../api/security-ediscoverycase-post-searches.md)|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|创建新的 [ediscoverySearch](../resources/security-ediscoverysearch.md) 对象。|
|[获取 ediscoverySearch](../api/security-ediscoverysearch-get.md)|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|读取 [ediscoverySearch](../resources/security-ediscoverysearch.md) 对象的属性和关系。|
|[更新 ediscoverySearch](../api/security-ediscoverysearch-update.md)|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|更新 [ediscoverySearch 对象的](../resources/security-ediscoverysearch.md) 属性。|
|[删除 ediscoverySearch](../api/security-ediscoverycase-delete-searches.md)|无|删除 [ediscoverySearch](../resources/security-ediscoverysearch.md) 对象。|
|[estimateStatistics](../api/security-ediscoverysearch-estimatestatistics.md)|无|对电子数据展示搜索中包含的数据运行估算统计信息操作。|
|[purgeData](../api/security-ediscoverysearch-purgedata.md)|无|对电子数据展示搜索中包含的 Teams 数据运行清除数据操作。|
|[列出 additionalSources](../api/security-ediscoverysearch-list-custodiansources.md)|[microsoft.graph.security.dataSource](../resources/security-datasource.md) 集合|从 additionalSources 导航属性获取 dataSource 资源。|
|[创建 dataSource](../api/security-ediscoverysearch-post-additionalsources.md)|[microsoft.graph.security.dataSource](../resources/security-datasource.md)|创建新的 dataSource 对象。|
|[列出 ediscoveryEstimateOperation](../api/security-ediscoverysearch-list-lastestimatestatisticsoperation.md)|[microsoft.graph.security.ediscoveryEstimateOperation](../resources/security-ediscoveryestimateoperation.md) 集合|从 lastEstimateStatisticsOperation 导航属性获取 ediscoveryEstimateOperation 资源。|
|[列出保管人来源](../api/security-ediscoverysearch-list-custodiansources.md)|[microsoft.graph.security.dataSource](../resources/security-datasource.md) 集合|从 CustodianSources 导航属性获取 dataSource 资源。|
|[添加保管人源](../api/security-ediscoverysearch-post-custodiansources.md)|[microsoft.graph.security.dataSource](../resources/security-datasource.md)|通过发布到 custodianSources 集合来添加 custodianSources。|
|[删除保管人源](../api/security-ediscoverysearch-delete-custodiansources.md)|无|删除 [dataSource](../resources/security-datasource.md) 对象。|
|[列出 noncustodialSources](../api/security-ediscoverysearch-list-noncustodialsources.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) 集合|从 noncustodialSources 导航属性获取 ediscoveryNoncustodialDataSource 资源。|
|[添加 ediscoveryNoncustodialDataSource](../api/security-ediscoverysearch-post-noncustodialsources.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|通过发布到 noncustodialSources 集合来添加 noncustodialSources。|
|[删除 noncustodialSources](../api/security-ediscoverysearch-delete-noncustodialsources.md)|无|删除 [ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|contentQuery|String|KQL (关键字查询语言) 查询中的查询字符串。 有关详细信息，请参阅 [内容搜索和电子数据展示的关键字查询和搜索条件](/microsoft-365/compliance/keyword-queries-and-search-conditions)。 可以使用与值配对的字段来优化搜索;例如， *主题：“季度财务”和日期>=06/01/2016 AND Date<=07/01/2016*.|
|createdBy|[identitySet](../resources/identityset.md)|创建 **电子数据展示搜索** 的用户。|
|createdDateTime|DateTimeOffset|电子 **数据展示搜索** 的创建日期和时间。|
|dataSourceScopes|microsoft.graph.ediscovery.dataSourceScopes|指定后，集合将跨整个工作负荷的服务。 可取值为：`none`、`allTenantMailboxes`、`allTenantSites`、`allCaseCustodians`、`allCaseNoncustodialDataSources`。|
|description|String|**电子数据展示搜索** 的说明。|
|displayName|String|**电子数据展示搜索** 的显示名称。|
|id|字符串| **电子数据展示搜索** 的 ID。 只读。 |
|lastModifiedBy|[identitySet](../resources/identityset.md)|最后一个修改 **电子数据展示搜索的** 用户。|
|lastModifiedDateTime|DateTimeOffset|上次修改 **电子数据展示搜索的** 日期和时间。|

### <a name="datasourcescopes-values"></a>dataSourceScopes 值

|成员|说明|
|:----|-----------|
|无|请勿指定任何范围 - 将单独引用位置。|
|allTenantMailboxes|在 **电子数据展示搜索** 中包括所有租户邮箱。|
|allTenantSites|在 **电子数据展示搜索** 中包括所有租户站点。|
|allCaseCustodians|在 **电子数据展示搜索** 中包括所有保管人位置。|
|allCaseNoncustodialDataSources|在 **电子数据展示搜索** 中包括所有非托管数据源。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|additionalSources|[microsoft.graph.security.dataSource](../resources/security-datasource.md) 集合|向 **电子数据展示搜索** 添加其他源。|
|addToReviewSetOperation|[microsoft.graph.security.ediscoveryAddToReviewSetOperation](../resources/security-ediscoveryaddtoreviewsetoperation.md)|将 **电子数据展示搜索** 的结果添加到指定的 **reviewSet**。|
|custodianSources|[microsoft.graph.security.dataSource](../resources/security-datasource.md) 集合|**电子数据展示搜索** 中包含的 **保管** 人源。|
|lastEstimateStatisticsOperation|[microsoft.graph.security.ediscoveryEstimateOperation](../resources/security-ediscoveryestimateoperation.md)|与 **电子数据展示搜索** 关联的最后一个估计操作。|
|noncustodialSources|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) 集合|**电子数据展示搜索** 中包含的 **noncustodialDataSource** 源|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoverySearch",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoverySearch",
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
  "contentQuery": "String",
  "dataSourceScopes": "String"
}
```