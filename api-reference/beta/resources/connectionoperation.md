---
title: connectionOperation 资源类型
description: 描述用于创建 Microsoft Search 连接架构的异步请求的状态。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 657d71dc6b1671b2af6011778c0b14bb299e3cf9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938882"
---
# <a name="connectionoperation-resource-type"></a>connectionOperation 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述用于创建 Microsoft Search 连接[架构](schema.md)的异步请求的状态。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 connectionOperation](../api/connectionoperation-get.md) | [connectionOperation](connectionoperation.md) | 读取 connectionOperation 对象的属性。 |

## <a name="properties"></a>属性

| 属性 | 类型                          | 描述                       |
|:---------|:------------------------------|:----------------------------------|
| error    | [errorDetail](errordetail.md) | 如果`status`为`failed`，则提供有关导致失败的错误的详细信息。 |
| id       | String                        | ConnectionOperation 的唯一标识符。 只读。 |
| 状态   | string                        | 指示异步操作的状态。 可取值为：`unspecified`、`inprogress`、`completed`、`failed`。 |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectionOperation",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.errorDetail"},
  "id": "String (identifier)",
  "status": "string"
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
