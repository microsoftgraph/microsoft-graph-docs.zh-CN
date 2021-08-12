---
title: searchEntity 资源类型
description: 表示 API 终结点的Microsoft 搜索对象。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4ef8b062b044ed08112b68c0a61c46f1147db9c751f42c7f500f269d79afea63
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163740"
---
# <a name="searchentity-resource-type"></a>searchEntity 资源类型

命名空间：microsoft.graph

表示 API 终结点的Microsoft 搜索对象。 它不像其他资源一样Graph，而是作为查询操作[锚](../api/search-query.md)点。 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[查询](../api/search-query.md) |[searchResponse](searchresponse.md) 集合 | 运行请求正文中指定的查询。  |

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.searchEntity",
  "baseType": "microsoft.graph.entity"
}
-->
``` json
{
  
}
```


## <a name="next-steps"></a>后续步骤

浏览 [查询](../api/search-query.md) 操作。


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "A top level object representing the Microsoft Search API endpoint.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


