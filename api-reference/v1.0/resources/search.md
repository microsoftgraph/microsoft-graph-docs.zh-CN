---
title: 搜索
description: 检索用于执行查询的搜索资源
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8e9d8bc133a050701543f2a978e56b662bafcc33
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377976"
---
# <a name="search-resource-type"></a>搜索资源类型

命名空间：microsoft.graph

搜索资源是表示搜索终结点的顶级对象。 它充当 [查询](../api/search-query.md) 操作的定位。

此资源不应按此方式调用。 对资源的任何请求都将导致错误请求。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a>JSON 表示形式

无

## <a name="properties"></a>属性

无

## <a name="relationships"></a>关系

无

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [查询](../api/search-query.md) | [searchResponse](searchresponse.md) 组| 执行[searchRequest](../resources/searchrequest.md)中指定的查询 |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


