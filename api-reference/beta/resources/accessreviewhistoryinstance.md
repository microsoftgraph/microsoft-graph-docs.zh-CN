---
title: accessReviewHistoryInstance 资源类型
description: 表示 accessReviewHistoryDefinition 对象的重复周期。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c6b1d137c470bdf384bc60d2a20834860f7dbd01
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697909"
---
# <a name="accessreviewhistoryinstance-resource-type"></a>accessReviewHistoryInstance 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 表示 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象的重复周期。 不重复的历史记录定义将完全有一个实例。

 每个 **accessReviewHistoryInstance** 及其关联 **的 accessReviewHistoryDefinition** 都包含属性 **reviewHistoryPeriodStartDateTime**、 **reviewHistoryPeriodEndDateTime**、 **决策**、 **scheduleSettings** 和 **范围**。 这些属性在计划重复周期以及选择审阅数据时使用，并且可以修改。 每个 **accessReviewHistoryInstance** 对象和数据仅可用 30 天。 将 **accessReviewHistoryInstance** 状态移动到 `done` 链接后，可以通过调用 [generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md) 来检索实例的数据。

## <a name="methods"></a>方法

| 方法  | 返回类型 | 说明 |
|:---|:---|:---|
|[列出 accessReviewHistoryInstances](../api/accessreviewhistorydefinition-list-instances.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md) 集合| 检索 [accessReviewHistoryInstance](accessreviewhistoryinstance.md) 对象及其属性的列表。|
|[generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|生成可用于检索实例的审阅历史记录数据的 URI。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|downloadUri|String|可用于检索审阅历史记录数据的 Uri。 生成后，此 URI 将处于活动状态 24 小时。 必填。|
|expirationDateTime|DateTimeOffset|此实例和关联的数据过期并删除历史记录的时间戳。 必填。|
|fulfilledDateTime|DateTimeOffset|收集此实例的所有可用数据的时间戳。 此实例的状态设置为 `done`后，将设置此值。 必需。|
|id|String|访问评审历史记录实例的分配的唯一标识符。 只读。 必填。|
|reviewHistoryPeriodEndDateTime|DateTimeOffset|此日期或之前结束的时间戳、审阅将包含在提取的历史记录数据中。|
|reviewHistoryPeriodStartDateTime|DateTimeOffset|从此日期开始或之后的时间戳、审阅将包含在提取的历史记录数据中。|
|runDateTime|DateTimeOffset|计划生成实例的历史记录数据的时间戳。|
|status|accessReviewHistoryStatus|表示审阅历史记录数据收集的状态。 可能的值包括 `done`、`inProgress`、`error`、`requested`、`unknownFutureValue`。 将 **状态** 标记为 `done`后，可以通过调用 [generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md) 方法生成一个链接来检索实例的数据。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewHistoryInstance",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.accessReviewHistoryInstance",
  "id": "String (identifier)",
  "reviewHistoryPeriodStartDateTime": "String (timestamp)",
  "reviewHistoryPeriodEndDateTime": "String (timestamp)",
  "status": "String",
  "runDateTime": "String (timestamp)",
  "fulfilledDateTime": "String (timestamp)",
  "downloadUri": "String",
  "expirationDateTime": "String (timestamp)"
}
```
