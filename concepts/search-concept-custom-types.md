---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索自定义类型
description: 您可以使用 Microsoft 搜索 API 通过[externalItem](/graph/api/resources/externalitem?view=graph-rest-beta)资源导入外部数据，并对此外部内容运行搜索查询。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 2e6def957cbfe5ac07750394941536941dc72b80
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897433"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-custom-types"></a><span data-ttu-id="8187a-103">在 Microsoft Graph 中使用 Microsoft Search API 搜索自定义类型</span><span class="sxs-lookup"><span data-stu-id="8187a-103">Use the Microsoft Search API in Microsoft Graph to search custom types</span></span>

<span data-ttu-id="8187a-104">您可以使用 Microsoft 搜索 API 通过[externalItem](/graph/api/resources/externalitem?view=graph-rest-beta)资源导入外部数据，并对此外部内容运行搜索查询。</span><span class="sxs-lookup"><span data-stu-id="8187a-104">You can use the Microsoft Search API to import external data via the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) resource, and run search queries on this external content.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="8187a-105">若要搜索自定义类型，请在[查询](/graph/api/search-query?view=graph-rest-beta)方法请求正文中指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="8187a-105">To search for custom types, specify the following in the [query](/graph/api/search-query?view=graph-rest-beta) method request body:</span></span>

- <span data-ttu-id="8187a-106">**ContentSources**属性，以包含在连接器安装过程中分配的连接 ID</span><span class="sxs-lookup"><span data-stu-id="8187a-106">The **contentSources** property to include the connection ID that is assigned during the connector setup</span></span>

- <span data-ttu-id="8187a-107">**EntityTypes**属性用作`externalItem`</span><span class="sxs-lookup"><span data-stu-id="8187a-107">The **entityTypes** property as `externalItem`</span></span>

- <span data-ttu-id="8187a-108">**Stored_fields**属性，以包含要检索的外部项中的字段</span><span class="sxs-lookup"><span data-stu-id="8187a-108">The **stored_fields** property to include the fields in the external item you want to retrieve</span></span>

## <a name="example"></a><span data-ttu-id="8187a-109">示例</span><span class="sxs-lookup"><span data-stu-id="8187a-109">Example</span></span>

### <a name="request"></a><span data-ttu-id="8187a-110">请求</span><span class="sxs-lookup"><span data-stu-id="8187a-110">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "externalItem"
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

### <a name="response"></a><span data-ttu-id="8187a-111">响应</span><span class="sxs-lookup"><span data-stu-id="8187a-111">Response</span></span>

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
                  "previewContent": "Description:  Setting Office for the first time.  Resolution:    To setup any Office app for the first time, tap any Office app like Word to launch it.    Tap Sign in if you already have a Microsoft Account or a Microsoft 365 work or school account."
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

## <a name="known-limitations"></a><span data-ttu-id="8187a-112">已知限制</span><span class="sxs-lookup"><span data-stu-id="8187a-112">Known limitations</span></span>

- <span data-ttu-id="8187a-113">自定义类型不支持跨多个源进行搜索（在**contentSources**中指定）。</span><span class="sxs-lookup"><span data-stu-id="8187a-113">Custom types don’t support searching across multiple sources (specified in **contentSources**).</span></span> <span data-ttu-id="8187a-114">一次只能搜索一个连接。</span><span class="sxs-lookup"><span data-stu-id="8187a-114">You can search only one connection at a time.</span></span>

- <span data-ttu-id="8187a-115">您必须指定**stored_fields**属性;否则，不会返回搜索结果。</span><span class="sxs-lookup"><span data-stu-id="8187a-115">You must specify the **stored_fields** property; otherwise, search results are not returned.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8187a-116">后续步骤</span><span class="sxs-lookup"><span data-stu-id="8187a-116">Next steps</span></span>

- [<span data-ttu-id="8187a-117">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="8187a-117">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
