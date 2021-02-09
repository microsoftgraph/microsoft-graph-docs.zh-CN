---
title: connectionOperation 资源类型
description: 描述创建 Microsoft 搜索连接架构的异步请求的状态。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e17b1f55b00fd7b9bdc69eb7a7a34d3453ab332d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158301"
---
# <a name="connectionoperation-resource-type"></a>connectionOperation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述创建 Microsoft 搜索连接架构的异步请求 [的状态](schema.md)。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 connectionOperation](../api/connectionoperation-get.md) | [connectionOperation](connectionoperation.md) | 读取 connectionOperation 对象的属性。 |

## <a name="properties"></a>属性

| 属性 | 类型                          | 说明                       |
|:---------|:------------------------------|:----------------------------------|
| error    | [errorDetail](errordetail.md) | 如果是 `status` `failed` ，则提供有关导致失败的错误的详细信息。 |
| id       | String                        | connectionOperation 的唯一标识符。 只读。 |
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


