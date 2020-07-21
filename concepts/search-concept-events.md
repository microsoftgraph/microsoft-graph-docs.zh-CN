---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索日历事件
description: 您可以在用户自己的日历中进行搜索。
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 8cafb01337581d1b1d2e355363aec14f658ee4f6
ms.sourcegitcommit: 79267b6d78c3510ef609953c5a664e692794caaa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/21/2020
ms.locfileid: "45196825"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-calendar-events"></a>在 Microsoft Graph 中使用 Microsoft Search API 搜索日历事件

您可以使用 Microsoft 搜索 API 在用户的主日历中搜索事件。 搜索的用户标识基于身份验证令牌。

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="example"></a>示例

### <a name="request"></a>请求

本示例将在用户的日历中搜索关键字 "contoso"，并返回最大25个结果。

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "event"
      ],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

## <a name="known-limitations"></a>已知限制

您只能访问用户自己的日历。 不支持共享日历和委派访问方案。

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview?view=graph-rest-beta)
