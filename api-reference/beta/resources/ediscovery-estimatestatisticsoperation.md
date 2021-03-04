---
title: estimateStatisticsOperation 资源类型
description: 表示处理估计源集合的计数和大小的操作。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e816ba01d4bb648a8e78b5b96369236f63fb163e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446623"
---
# <a name="estimatestatisticsoperation-resource-type"></a>estimateStatisticsOperation 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示处理估计 [sourceCollection](../resources/ediscovery-sourcecollection.md)的计数和大小的操作。 有关详细信息，请参阅 ["收集高级电子数据展示](/microsoft-365/compliance/collecting-data-for-ediscovery)"中案例的数据。

继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。

## <a name="methods"></a>Methods

无。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|action|microsoft.graph.ediscovery.caseAction| 操作类型。 此实体的大小写操作将始终为 `estimateStatistics` 。 只读。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|completedDateTime|DateTimeOffset|操作完成的日期和时间。 只读。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|createdBy|[identitySet](../resources/identityset.md)|创建操作的用户。 只读。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|createdDateTime|DateTimeOffset|操作开始的日期和时间。 只读。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|id|String| 操作 ID。 只读。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|indexedItemCount|Int64|与内容查询匹配的 **sourceCollection** 的预计项目计数。|
|indexedItemsSize|Int64|与内容查询匹配的 **sourceCollection** 项目的估计大小。|
|mailboxCount|Int32|搜索命中的邮箱数。|
|percentProgress|Int32|操作的进度。 只读。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|resultInfo|[resultInfo](../resources/resultinfo.md)|包含特定于成功和失败的结果信息。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|siteCount|Int32|搜索命中的邮箱数。|
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|案例操作的状态。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。 可取值为：`notStarted`、`submissionFailed`、`running`、`succeeded`、`partiallySucceeded`、`failed`。|
|unindexedItemCount|Int64|集合的未索引项的估计计数。|
|unindexedItemsSize|Int64|集合的未索引项的估计大小。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|sourceCollection|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|电子数据展示集合，通常称为搜索。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.estimateStatisticsOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/operations/$entity",
    "@odata.type": "#microsoft.graph.ediscovery.estimateStatisticsOperation",
    "createdDateTime": "2021-01-12T18:47:23.3974907Z",
    "completedDateTime": "2021-01-12T18:47:51.1461805Z",
    "percentProgress": 100,
    "status": "succeeded",
    "action": "estimateStatistics",
    "id": "82edd40e182a464fa02c24a36fa94873",
    "indexedItemCount": 2,
    "indexedItemsSize": 39276,
    "unindexedItemCount": 0,
    "unindexedItemsSize": 0,
    "mailboxCount": 1,
    "siteCount": 0,
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null,
            "userPrincipalName": "admin@contoso.com"
        }
    }
}
```
