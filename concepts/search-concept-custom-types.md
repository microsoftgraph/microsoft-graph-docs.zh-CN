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
# <a name="search-custom-types-externalitem"></a><span data-ttu-id="a1a7e-103">搜索自定义类型 (externalItem)</span><span class="sxs-lookup"><span data-stu-id="a1a7e-103">Search custom types (externalItem)</span></span>

<span data-ttu-id="a1a7e-104">Microsoft 搜索 API 允许您通过[externalItem](/graph/api/resources/externalitem?view=graph-rest-beta)资源导入外部数据，并对此外部内容运行搜索查询。</span><span class="sxs-lookup"><span data-stu-id="a1a7e-104">The Microsoft Search API lets you import external data via the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) resource, and run search queries on this external content.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="a1a7e-105">若要搜索自定义类型，请在[查询](/graph/api/search-query?view=graph-rest-beta)方法请求正文中指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="a1a7e-105">To search for custom types, specify the following in the [query](/graph/api/search-query?view=graph-rest-beta) method request body:</span></span>

- <span data-ttu-id="a1a7e-106">**ContentSources**属性，以包含在连接器安装过程中分配的连接 ID</span><span class="sxs-lookup"><span data-stu-id="a1a7e-106">The **contentSources** property to include the connection ID which is assigned during the connector setup</span></span>

- <span data-ttu-id="a1a7e-107">**EntityType**属性作为`externalItem`</span><span class="sxs-lookup"><span data-stu-id="a1a7e-107">The **entityType** property as `externalItem`</span></span>

- <span data-ttu-id="a1a7e-108">**Stored_fields**属性，以包含要检索的外部项中的字段</span><span class="sxs-lookup"><span data-stu-id="a1a7e-108">The **stored_fields** property to include the fields in the external item you want to retrieve</span></span>

## <a name="example"></a><span data-ttu-id="a1a7e-109">示例</span><span class="sxs-lookup"><span data-stu-id="a1a7e-109">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1a7e-110">请求</span><span class="sxs-lookup"><span data-stu-id="a1a7e-110">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="a1a7e-111">响应</span><span class="sxs-lookup"><span data-stu-id="a1a7e-111">Response</span></span>

<span data-ttu-id="a1a7e-112">响应</span><span class="sxs-lookup"><span data-stu-id="a1a7e-112">Response</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="a1a7e-113">已知限制</span><span class="sxs-lookup"><span data-stu-id="a1a7e-113">Known limitations</span></span>

- <span data-ttu-id="a1a7e-114">自定义类型不支持跨多个源进行搜索（在**contentSources**中指定）。</span><span class="sxs-lookup"><span data-stu-id="a1a7e-114">Custom types don’t support searching across multiple sources (specified in **contentSources**).</span></span> <span data-ttu-id="a1a7e-115">一次只能搜索一个连接。</span><span class="sxs-lookup"><span data-stu-id="a1a7e-115">You can search only one connection at a time.</span></span>

- <span data-ttu-id="a1a7e-116">您必须指定**stored_fields**属性，否则不会返回搜索结果。</span><span class="sxs-lookup"><span data-stu-id="a1a7e-116">You must specify the **stored_fields** property, otherwise search results are not returned.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a1a7e-117">后续步骤</span><span class="sxs-lookup"><span data-stu-id="a1a7e-117">Next steps</span></span>

<span data-ttu-id="a1a7e-118">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="a1a7e-118">Find out more about:</span></span>

- [<span data-ttu-id="a1a7e-119">使用搜索 API</span><span class="sxs-lookup"><span data-stu-id="a1a7e-119">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
