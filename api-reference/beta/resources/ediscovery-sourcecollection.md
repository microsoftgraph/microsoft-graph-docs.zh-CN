---
title: sourceCollection 资源类型
description: 表示一个电子数据展示集合，通常称为搜索。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 86ecf3adb64be2b216fdc167b29c10a850e25af6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446149"
---
# <a name="sourcecollection-resource-type"></a>sourceCollection 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个电子数据展示集合，通常称为搜索。 有关详细信息，请参阅 ["收集高级电子数据展示](/microsoft-365/compliance/collecting-data-for-ediscovery)"中案例的数据。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 sourceCollections](../api/ediscovery-case-list-sourcecollections.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) 集合|获取 **sourceCollection** 对象及其属性的列表。|
|[创建 sourceCollection](../api/ediscovery-case-post-sourcecollections.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|创建新的 **sourceCollection** 对象。|
|[获取 sourceCollection](../api/ediscovery-sourcecollection-get.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|读取 **sourceCollection 对象的属性和** 关系。|
|[更新 sourceCollection](../api/ediscovery-sourcecollection-update.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|更新 **sourceCollection** 对象的属性。|
|[删除 sourceCollection](../api/ediscovery-sourcecollection-delete.md)|无|删除 **sourceCollection** 对象。|
|[estimateStatistics](../api/ediscovery-sourcecollection-estimatestatistics.md)|无|运行源集合中电子邮件和文档的估计数量。|
|[列出 additionalSources](../api/ediscovery-sourcecollection-list-additionalsources.md)|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 集合|获取与源集合关联的其他 **DataSource** 对象的列表。|
|[列出 custodianSources](../api/ediscovery-sourcecollection-list-custodiansources.md)|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 集合|获取与源集合关联的其他 **DataSource** 对象的列表。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|contentQuery|String|KQL 中的查询字符串 (关键字查询语言) 查询。 有关详细信息，请参阅内容搜索和电子数据展示的关键字 [查询和搜索条件](https://docs.microsoft.com/microsoft-365/compliance/keyword-queries-and-search-conditions)。  可以使用与值配对的字段来优化搜索;例如 *，subject："Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*|
|createdBy|[identitySet](../resources/identityset.md)|创建 **sourceCollection 的用户**。|
|createdDateTime|DateTimeOffset|创建 **sourceCollection 的** 日期和时间。|
|说明|String|**sourceCollection 的说明**|
|displayName|String|**sourceCollection** 显示名称|
|id|String| **sourceCollection** 的 ID。 只读。 |
|lastModifiedBy|[identitySet](../resources/identityset.md)|上次修改 **sourceCollection 的用户**。|
|lastModifiedDateTime|DateTimeOffset|上次修改 **sourceCollection** 的日期和时间。|
|tenantSources|microsoft.graph.ediscovery.tenantSources|指定此参数时，集合将跨越整个工作负荷的服务。 可取值为：`allMailboxes`、`allSites`。|

### <a name="tenantsources-values"></a>tenantSources 值

|成员|说明|
|:----|-----------|
|allMailboxes| 包含集合中所有邮箱。 |
|allSites| 包括集合中所有网站。 |

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|additionalSources|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 集合|向 **sourceCollection 添加其他源**。|
|addToReviewSetOperation|[microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md)|将 **sourceCollection 的结果** 添加到指定的 **reviewSet**。|
|custodianSources|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 集合|**sourceCollection** 中包含的保管 **人源**。|
|lastEstimateStatisticsOperation|[microsoft.graph.ediscovery.estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md)|与 **sourceCollection** 关联的最后一个估计操作。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.sourceCollection",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.sourceCollection",
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
  "tenantSources": "String"
}
```
