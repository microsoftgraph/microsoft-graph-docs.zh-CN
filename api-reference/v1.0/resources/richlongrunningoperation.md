---
title: richLongRunningOperation 资源类型
description: 表示站点或列表上长时间运行的操作的状态。
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 73f57e5daaf2f55aca6fa03f0958d19d8323bdf8
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191835"
---
# <a name="richlongrunningoperation-resource-type"></a>richLongRunningOperation 资源类型

命名空间：microsoft.graph

表示 [站点](../resources/site.md) 或 [列表](../resources/list.md)上长时间运行的操作的状态。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 richLongRunningOperation](../api/richlongrunningoperation-get.md)|[richLongRunningOperation](../resources/richlongrunningoperation.md)|获取[网站](../resources/site.md)或[列表](../resources/list.md)上[长时间运行的丰富操作](../resources/richlongrunningoperation.md)的状态。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|创建此操作的日期和时间。|
|error|[publicError](../resources/publicerror.md)| 导致操作失败的错误。|
|id|String|操作的唯一标识符。 继承自 [entity](../resources/entity.md)。|
|lastActionDateTime|DateTimeOffset| 对此操作执行最后一个操作的日期和时间。|
|percentageComplete|Int32|一个介于 0 和 100 之间的值，指示操作的进度。|
|resourceId|String|结果的唯一标识符。|
|resourceLocation|String|资源的规范 URL。|
|状态|longRunningOperationStatus|长时间运行的操作的状态。 可取值为：`notStarted`、`running`、`succeeded`、`failed`、`unknownFutureValue`。|
|statusDetail|String|有关状态值的详细信息。|
|type|字符串| 操作的类型。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.richLongRunningOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.richLongRunningOperation",
  "createdDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  },
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "percentageComplete": "Integer",
  "resourceId": "String",
  "resourceLocation": "String",
  "status": "String",
  "statusDetail": "String",
  "type": "String"
}
```

