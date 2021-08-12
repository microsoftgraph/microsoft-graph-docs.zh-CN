---
title: 搜索
description: 检索用于执行查询的搜索资源
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7f20a7d0513f084dadc8dc3f3693a7dd51109fb7e9ccbb163a80a17a29d6978f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251806"
---
# <a name="search-resource-type"></a>搜索资源类型

命名空间：microsoft.graph

搜索资源是表示搜索终结点的顶级对象。 它充当查询操作 [锚点](../api/search-query.md) 。

不应这样调用此资源。 资源上的任何请求都会导致错误的请求。

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
| [查询](../api/search-query.md) | [searchResponse](searchresponse.md) 集合| 执行 [searchRequest 中指定的查询](../resources/searchrequest.md) |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


