---
title: 搜索自定义类型
description: 利用查询 API，您可以通过索引 API 在自定义类型引入中进行搜索。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 53203d300fd3cf42fd5e6993fe8ba016de06669a
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703979"
---
# <a name="search-custom-types-externalitem"></a>搜索自定义类型 (externalItem)

Microsoft 搜索 API 允许您通过[externalItem](/graph/api/resources/externalitem?view=graph-rest-beta)资源导入外部数据，并对此外部内容运行搜索查询。

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

若要搜索自定义类型，请在[查询](/graph/api/search-query?view=graph-rest-beta)方法请求正文中指定以下内容：

- **ContentSources**属性，以包含在连接器安装过程中分配的连接 ID

- **EntityType**属性作为`externalItem`

- **Stored_fields**属性，以包含要检索的外部项中的字段

## <a name="example"></a>示例

### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.externalItem"
      ],
      "contentSources": [
        "/external/connections/servicenow-connector-contoso"
      ],
      "query": {
        "query_string": {
          "query": "contoso tickets"
        }
      },
      "from": 0,
      "size": 25,
      "stored_fields": [
        "title",
        "priority",
        "description"
      ]
    }
  ]
}
```

### <a name="response"></a>响应

响应

```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
  "value": [
    {
      "hitsContainers": [
        {
          "total": 2,
          "moreResultsAvailable": false,
          "hits": [
            {
              "_id": "AAMkADc0NDNlNTE0",
              "_score": 1,
              "_sortField": "Relevance",
              "_source": {
                "@odata.type": "#microsoft.graph.externalItem",
                "properties": {
                  "number": "KB0010025",
                  "shortdescription": "Contoso maintenance guidelines",
                  "syscreatedon": "2019-10-14T22:45:02Z",
                  "accessurl": "https://contoso.service-now.com/kb_view.do?sys_kb_id=6b5465781ba000104793877ddc4bcb81",
                  "previewContent": "Contoso maintenance guidelines"
                }
              }
            },
            {
              "_id": "MG+1glPAAAAAAl3AAA=",
              "_score": 2,
              "_sortField": "Relevance",
              "_source": {
                "@odata.type": "#microsoft.graph.externalItem",
                "properties": {
                  "number": "KB0054396",
                  "shortdescription": "Contoso : Setting Office for the first time.",
                  "syscreatedon": "2019-08-09T01:53:26Z",
                  "accessurl": "https://contoso.service-now.com/kb_view.do?sys_kb_id=004d8d931b0733004793877ddc4bcb29",
                  "previewContent": "Description:  Setting Office for the first time.  Resolution:    To setup any Office app for the first time, tap any Office app like Word to launch it.    Tap Sign in if you already have a Microsoft Account or an Office 365 work or school account."
                }
              }
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="known-limitations"></a>已知限制

- 自定义类型不支持跨多个源进行搜索（在**contentSources**中指定）。 一次只能搜索一个连接。

- 您必须指定**stored_fields**属性，否则不会返回搜索结果。

## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [使用搜索 API](/graph/api/resources/search-api-overview?view=graph-rest-beta)
