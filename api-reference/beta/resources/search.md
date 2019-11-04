---
title: 搜索
description: 检索用于执行查询的搜索资源
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 65a099ea0ae57b116bcf6a251170e507945226c9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938770"
---
# <a name="search-resource-type"></a>搜索资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

搜索资源是表示搜索终结点的顶级对象。 它充当[查询](../api/search-query.md)操作的定位。

此资源不应按此方式调用。 对资源的任何请求都将导致错误请求。

## <a name="json-representation"></a>JSON 表示形式

无

## <a name="properties"></a>属性

无

## <a name="relationships"></a>关系

无

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [query](../api/search-query.md) | [searchResponse](searchresponse.md)组| 执行[searchRequest](../resources/searchrequest.md)中指定的查询 |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
