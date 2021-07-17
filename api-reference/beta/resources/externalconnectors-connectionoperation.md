---
title: connectionOperation 资源类型
description: 描述创建连接架构的异步请求Microsoft 搜索状态。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1b9e3bf811807213970694ebe4e7748bf59e32ef
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467644"
---
# <a name="connectionoperation-resource-type"></a>connectionOperation 资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述创建连接架构的异步Microsoft 搜索[状态](externalconnectors-schema.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 connectionOperation](../api/externalconnectors-connectionoperation-get.md) | [connectionOperation](externalconnectors-connectionoperation.md) | 读取 connectionOperation 对象的属性。 |

## <a name="properties"></a>属性

| 属性 | 类型                          | 说明                       |
|:---------|:------------------------------|:----------------------------------|
| error    | [publicError](publicerror.md) | 如果 `status` 为 `failed` ，则提供有关导致失败的错误的详细信息。 |
| id       | String                        | connectionOperation 的唯一标识符。 只读。 |
| 状态   | String                        | 指示异步操作的状态。 可取值为：`unspecified`、`inprogress`、`completed`、`failed`。 |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectionOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
