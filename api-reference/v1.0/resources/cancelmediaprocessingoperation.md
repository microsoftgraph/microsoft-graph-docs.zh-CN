---
title: cancelMediaProcessingOperation 资源类型
description: 此资源类型用于描述取消媒体处理操作的响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6896a7a4d08aea0c4d394bfbaef8a54bd4c789b310f0079dbbf08daac99606d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235686"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a>CancelMediaProcessingOperation 资源类型

命名空间：microsoft.graph

描述取消媒体处理操作的响应格式。

## <a name="properties"></a>属性

| 属性      | 类型                        | 说明                                                                     |
| :------------ | :-------------------------- | :------------------------------------------------------------------------------ |
| all           | Boolean                     | 指示是停止所有操作还是当前操作。                            |
| clientContext | String                      | 客户端上下文。                                                             |
| id            | String                      | 服务器操作 ID。 只读。                                             |
| resultInfo    | [resultInfo](resultinfo.md) | 结果信息。  只读。                                             |
| status        | String                      | 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cancelMediaProcessingOperation"
}-->
```json
{
  "all": true,
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cancelMediaProcessingOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

