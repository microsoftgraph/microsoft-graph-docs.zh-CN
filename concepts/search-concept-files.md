---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索文件
description: 您可以使用 Microsoft 搜索 API 搜索存储在 SharePoint 或 OneDrive 中的文件。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 52b2d5b54577bfb744bff5f3dacf4ad77da3761a
ms.sourcegitcommit: 093d89c7583bb6880c8395e9498a1f33cdd938b4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44568808"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-files"></a><span data-ttu-id="4b683-103">在 Microsoft Graph 中使用 Microsoft Search API 搜索文件</span><span class="sxs-lookup"><span data-stu-id="4b683-103">Use the Microsoft Search API in Microsoft Graph to search files</span></span>

<span data-ttu-id="4b683-104">您可以使用 Microsoft 搜索 API 搜索存储在 SharePoint 或 OneDrive 中的文件。</span><span class="sxs-lookup"><span data-stu-id="4b683-104">You can use the Microsoft Search API to search files stored in SharePoint or OneDrive.</span></span> <span data-ttu-id="4b683-105">Microsoft Search API 使用相关性模型，该模型利用来自 Microsoft Graph 的有关用户的关系和活动的信号。</span><span class="sxs-lookup"><span data-stu-id="4b683-105">The Microsoft Search API uses a relevance model that makes use of signals from Microsoft Graph about users' relationships and activities.</span></span> <span data-ttu-id="4b683-106">这使您能够在与 SharePoint 中列出搜索结果**的文件选项卡一致**的文件搜索体验中返回和提升用户关注的内容。</span><span class="sxs-lookup"><span data-stu-id="4b683-106">This enables you to return and promote the content that users care about, in a file search experience that is consistent with the **Files** tab that lists search results in SharePoint.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="search-sharepoint-or-onedrive-files"></a><span data-ttu-id="4b683-107">搜索 SharePoint 或 OneDrive 文件</span><span class="sxs-lookup"><span data-stu-id="4b683-107">Search SharePoint or OneDrive files</span></span>

<span data-ttu-id="4b683-108">您可以在 SharePoint 和 OneDrive 查询的搜索词中使用 KQL。</span><span class="sxs-lookup"><span data-stu-id="4b683-108">You can use KQL in search terms of queries for SharePoint and OneDrive.</span></span> <span data-ttu-id="4b683-109">例如：</span><span class="sxs-lookup"><span data-stu-id="4b683-109">For example:</span></span>

- <span data-ttu-id="4b683-110">`"query": "contoso filetype:docx OR filetype:doc"`将查询范围限定为 Word 文档。</span><span class="sxs-lookup"><span data-stu-id="4b683-110">`"query": "contoso filetype:docx OR filetype:doc"` scopes the query to Word documents.</span></span>
- <span data-ttu-id="4b683-111">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""`将查询范围限定为网站中的特定文件夹。</span><span class="sxs-lookup"><span data-stu-id="4b683-111">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>

<span data-ttu-id="4b683-112">属性限制必须在条件中指定有效且可查询的托管属性名称，这样才能有效。</span><span class="sxs-lookup"><span data-stu-id="4b683-112">In order to be valid, properties restriction should specify a valid, queryable managed property name in the condition.</span></span>

### <a name="example"></a><span data-ttu-id="4b683-113">示例</span><span class="sxs-lookup"><span data-stu-id="4b683-113">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4b683-114">请求</span><span class="sxs-lookup"><span data-stu-id="4b683-114">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "driveItem"
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

#### <a name="response"></a><span data-ttu-id="4b683-115">响应</span><span class="sxs-lookup"><span data-stu-id="4b683-115">Response</span></span>

<!---TODO nmoreau team Include one example of externalItem response.-->
```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "test"
      ],
      "hitsContainers": [
        {
          "total": 350,
          "moreResultsAvailable": true,
          "hits": [
            {
              "_id": "FlULeN/ui/1GjLx1rUfio5UAAEl",
              "_score": 1,
              "_sortField": "Relevance",
              "_summary": "<c0>Contoso</c0> Detailed Design <ddd/>",
              "_source": {
                "@odata.type": "#microsoft.graph.driveItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                "name": "web_part_test_long Notebook",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/contoso-designs.docx",
                "lastModifiedBy": {
                  "user": {
                    "displayName": "Richard Mayer"
                  }
                },
                "fileSystemInfo": {
                  "createdDateTime": "2019-06-10T06:37:43Z",
                  "lastModifiedDateTime": "2019-06-10T06:37:43Z"
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

## <a name="next-steps"></a><span data-ttu-id="4b683-116">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4b683-116">Next steps</span></span>

- [<span data-ttu-id="4b683-117">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="4b683-117">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
