---
title: 搜索资源类型
description: 表示 Microsoft 搜索终结点的顶级Graph。
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 034e1adec8d1bcee0336abdbeed2d980ee559964
ms.sourcegitcommit: a60e5e81cfa04b666a1df1111a1d91f6c11989e9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2022
ms.locfileid: "62282032"
---
# <a name="search-resource-type"></a>搜索资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示搜索终结点的顶级对象。 它充当查询操作 [锚点](../api/search-query.md) 。

不调用此资源。 调用此资源的任何请求都将导致 HTTP `400 Bad Request` 响应。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [查询](../api/search-query.md) | [searchResponse](searchresponse.md) 集合| 运行指定的搜索查询。 |

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

无。

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


