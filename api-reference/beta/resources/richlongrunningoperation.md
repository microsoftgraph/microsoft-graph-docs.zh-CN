---
title: richLongRunningOperation 资源类型
description: 包含有关长时间运行的操作的元数据。
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 2f16e9abb8dc3a22ad7a3d3b32e707ddb595c06a
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162227"
---
# <a name="richlongrunningoperation-resource-type"></a>richLongRunningOperation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关长时间运行的操作的元数据。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出网站中的 richLongRunningOperations](../api/site-list-operations.md)|[richLongRunningOperation](../resources/richlongrunningoperation.md) 集合|获取网站中的 [richLongRunningOperation](../resources/richlongrunningoperation.md) 对象及其属性的列表。|
|[在列表中列出 richLongRunningOperations](../api/list-list-operations.md)|[richLongRunningOperation](../resources/richlongrunningoperation.md) 集合|获取列表中 [richLongRunningOperation](../resources/richlongrunningoperation.md) 对象及其属性的列表。|
|[获取 richLongRunningOperation](../api/richlongrunningoperation-get.md)|[richLongRunningOperation](../resources/richlongrunningoperation.md)|读取 [richLongRunningOperation 对象](../resources/richlongrunningoperation.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|创建此操作的时间。|
|error|[publicError](../resources/publicerror.md)| 由于操作失败而出现错误。|
|id|String|操作标识符。 继承自 [实体](../resources/entity.md)。|
|lastActionDateTime|DateTimeOffset| 上次对此操作执行的操作的时间。|
|percentageComplete|Int32|一个介于 0 和 100 之间的值，指示操作的进度。|
|resourceId|String|结果的唯一标识符。|
|resourceLocation|String|资源的规范 URL。|
|状态|longRunningOperationStatus|操作的状态。可能的值是 `notStarted` `running` `succeeded` ：、、、、。 `failed` `unknownFutureValue`|
|statusDetail|String|有关状态值的详细信息。|
|type|String| 操作的类型。|

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
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "resourceLocation": "String",
  "status": "String",
  "statusDetail": "String",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  },
  "percentageComplete": "Integer",
  "resourceId": "String",
  "type": "String"
}
```

