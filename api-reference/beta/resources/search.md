---
title: 搜索
description: 检索用于执行查询的搜索资源
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: bb38d281895ac11d97a026a4352f68b93e8ba801
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704060"
---
# <a name="search-resource-type"></a>搜索资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

搜索资源是表示搜索终结点的顶级对象。 它充当[查询](../api/search-query.md)操作的定位。

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
| [查询](../api/search-query.md) | [searchResponse](searchresponse.md)组| 执行[searchRequest](../resources/searchrequest.md)中指定的查询 |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
