---
title: addLargeGalleryViewOperation 资源类型
description: 描述添加大型库视图的操作的响应格式。
author: navali-msft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 312f3ea1d9c924e142e6b192a7f6542cc6e0cd19
ms.sourcegitcommit: 4ff6e89e89178cbd5aef8aa019e714d95817fae4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2022
ms.locfileid: "65017038"
---
# <a name="addlargegalleryviewoperation-resource-type"></a>addLargeGalleryViewOperation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述添加大型库视图的操作的响应格式。

继承自 [commsOperation](commsoperation.md)。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-|:-|:-|
| [获取 addLargeGalleryViewOperation](../api/addlargegalleryviewoperation-get.md) | [addLargeGalleryViewOperation](addlargegalleryviewoperation.md) | 获取将大型库视图添加到调用的操作的状态。 |

## <a name="properties"></a>属性

| 属性                       | 类型                        | 说明                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | String                      | 客户端上下文。                                                                                                                               |
| id                             | String                      | 服务器操作的 ID。 只读。                                                                                             |
| resultInfo                     | [resultInfo](resultinfo.md) | 结果信息。  只读。                                                                                             |
| 状态                         | operationStatus             | 操作的状态。 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。                                                 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addLargeGalleryViewOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addLargeGalleryViewOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


