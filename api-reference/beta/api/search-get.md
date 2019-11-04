---
title: 搜索
description: 检索用于执行查询的搜索资源
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d7b84fdad96530f88f09c7da7b00a6013b19017e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938384"
---
# <a name="search"></a>搜索

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

搜索资源是表示搜索终结点的顶级对象。 它不像 Graph 中的任何其他资源一样工作，而是用作搜索操作（查询）的定位。 图表中没有资源表示形式。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 阅读文章、文件、读取、ExternalItem、阅读、全部 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /search
```

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

此资源不应按此方式调用。 对资源的任何请求都将导致错误请求。

## <a name="next-steps"></a>后续步骤

- 在搜索时浏览[/query](search-query.md)操作。


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
