---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索文件
description: 您可以使用 Microsoft 搜索 API 搜索存储在 SharePoint 或 OneDrive 中的文件。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 0b8db24a8b9ccd63ac3d3be800b209a64eb3aa9d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866915"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-files"></a><span data-ttu-id="78756-103">在 Microsoft Graph 中使用 Microsoft Search API 搜索文件</span><span class="sxs-lookup"><span data-stu-id="78756-103">Use the Microsoft Search API in Microsoft Graph to search files</span></span>

<span data-ttu-id="78756-104">您可以使用 Microsoft 搜索 API 搜索存储在 SharePoint 或 OneDrive 中的文件。</span><span class="sxs-lookup"><span data-stu-id="78756-104">You can use the Microsoft Search API to search files stored in SharePoint or OneDrive.</span></span> <span data-ttu-id="78756-105">Microsoft Search API 使用相关性模型，该模型利用来自 Microsoft Graph 的有关用户的关系和活动的信号。</span><span class="sxs-lookup"><span data-stu-id="78756-105">The Microsoft Search API uses a relevance model that makes use of signals from Microsoft Graph about users' relationships and activities.</span></span> <span data-ttu-id="78756-106">这使您能够在与 SharePoint 中列出搜索结果**的文件选项卡一致**的文件搜索体验中返回和提升用户关注的内容。</span><span class="sxs-lookup"><span data-stu-id="78756-106">This enables you to return and promote the content that users care about, in a file search experience that is consistent with the **Files** tab that lists search results in SharePoint.</span></span> 

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="78756-107">API 还可以通过[externalFile](/graph/api/resources/externalfile?view=graph-rest-beta)资源公开公开的外部文件。</span><span class="sxs-lookup"><span data-stu-id="78756-107">The API can also surface external files exposed via the [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) resource.</span></span>

## <a name="search-sharepoint-or-onedrive-files"></a><span data-ttu-id="78756-108">搜索 SharePoint 或 OneDrive 文件</span><span class="sxs-lookup"><span data-stu-id="78756-108">Search SharePoint or OneDrive files</span></span>

<span data-ttu-id="78756-109">您可以在 SharePoint 和 OneDrive 查询的搜索词中使用 KQL。</span><span class="sxs-lookup"><span data-stu-id="78756-109">You can use KQL in search terms of queries for SharePoint and OneDrive.</span></span> <span data-ttu-id="78756-110">例如：</span><span class="sxs-lookup"><span data-stu-id="78756-110">For example:</span></span>

- <span data-ttu-id="78756-111">`"query": "contoso filetype:docx OR filetype:doc"`将查询范围限定为 Word 文档。</span><span class="sxs-lookup"><span data-stu-id="78756-111">`"query": "contoso filetype:docx OR filetype:doc"` scopes the query to Word documents.</span></span>
- <span data-ttu-id="78756-112">`"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""`将查询范围限定为网站中的特定文件夹。</span><span class="sxs-lookup"><span data-stu-id="78756-112">`"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>

<span data-ttu-id="78756-113">属性限制必须在条件中指定有效且可查询的托管属性名称，这样才能有效。</span><span class="sxs-lookup"><span data-stu-id="78756-113">In order to be valid, properties restriction should specify a valid, queryable managed property name in the condition.</span></span>

### <a name="example"></a><span data-ttu-id="78756-114">示例</span><span class="sxs-lookup"><span data-stu-id="78756-114">Example</span></span>

#### <a name="request"></a><span data-ttu-id="78756-115">请求</span><span class="sxs-lookup"><span data-stu-id="78756-115">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.driveItem"
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

#### <a name="response"></a><span data-ttu-id="78756-116">响应</span><span class="sxs-lookup"><span data-stu-id="78756-116">Response</span></span>

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

## <a name="search-external-files-well-known-types"></a><span data-ttu-id="78756-117">搜索外部文件（已知类型）</span><span class="sxs-lookup"><span data-stu-id="78756-117">Search external files (well-known types)</span></span>

<span data-ttu-id="78756-118">默认情况下，[文件共享连接器](/MicrosoftSearch/file-share-connector)在 Microsoft Search 中可用。</span><span class="sxs-lookup"><span data-stu-id="78756-118">The [file share connector](/MicrosoftSearch/file-share-connector) is available in Microsoft Search by default.</span></span> <span data-ttu-id="78756-119">您可以使用它来索引文件共享上可用的文件。</span><span class="sxs-lookup"><span data-stu-id="78756-119">You can use it to index files available on a file share.</span></span> <span data-ttu-id="78756-120">您可以使用查询 API 查询所有外部文件。</span><span class="sxs-lookup"><span data-stu-id="78756-120">You can use the query API to query all external files.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="example"></a><span data-ttu-id="78756-121">示例</span><span class="sxs-lookup"><span data-stu-id="78756-121">Example</span></span>

<span data-ttu-id="78756-122">下面的示例返回租户的所有已配置的外部文件，并按相关性对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="78756-122">The following example returns all configured external files for the tenant, and sorts the results by relevance.</span></span>

#### <a name="request"></a><span data-ttu-id="78756-123">请求</span><span class="sxs-lookup"><span data-stu-id="78756-123">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.externalFile"
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

#### <a name="response"></a><span data-ttu-id="78756-124">响应</span><span class="sxs-lookup"><span data-stu-id="78756-124">Response</span></span>

```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 4,
          "moreResultsAvailable": true,
          // Hits represent the search results
          "hits": [
            {
              "_id": "FsHvoeTuRRVLnuEZLEVBfSQAAWTp",
              "_score": 1,
              "_sortField": "Relevance",
              "_source": {
                "@odata.type": "#microsoft.graph.externalFile",
                "id": "FsHvoeTuRRVLnuEZLEVBfSQAAWTp",
                "extension": "pptx",
                "name": "Contoso-Overview.pptx",
                "lastModifiedTime": "2018-05-09T04:01:14Z",
                "modifiedBy": "Baala Vedantam",
                "title": "Contoso Overview 2018",
                "url": "file://fileshare01/External Presentations/Contoso-Overview.pptx"
              }
            },
            {
              //Another searchHit
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="search-all-files-including-externalfile-instances"></a><span data-ttu-id="78756-125">搜索所有文件（包括 externalFile 实例）</span><span class="sxs-lookup"><span data-stu-id="78756-125">Search all files (including externalFile instances)</span></span>

<span data-ttu-id="78756-126">您可以通过在搜索请求中指定两个实体类型来搜索租户中的所有文件，包括存储在[driveitem](/graph/api/resources/driveitem?view=graph-rest-beta)和外部文件中的文件。</span><span class="sxs-lookup"><span data-stu-id="78756-126">You can search all the files in a tenant, including files stored in [driveItems](/graph/api/resources/driveitem?view=graph-rest-beta) and external files, by specifying two entity types in the search request.</span></span>

<span data-ttu-id="78756-127">响应包括每个[searchHit](/graph/api/resources/searchhit?view=graph-rest-beta)对象的`_sources`字段中的**driveItem**和**externalItem**实例。</span><span class="sxs-lookup"><span data-stu-id="78756-127">The response includes **driveItem** and **externalItem** instances in the `_sources` field of each [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta) object.</span></span>

### <a name="example"></a><span data-ttu-id="78756-128">示例</span><span class="sxs-lookup"><span data-stu-id="78756-128">Example</span></span>

<span data-ttu-id="78756-129">下面的示例返回租户中满足搜索词的所有已配置的**externalFile**和**driveItem**对象。</span><span class="sxs-lookup"><span data-stu-id="78756-129">The following example returns all configured **externalFile** and **driveItem** objects in the tenant that satisfy the search terms.</span></span> <span data-ttu-id="78756-130">它按相关性对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="78756-130">It sorts the results by relevance.</span></span>

### <a name="request"></a><span data-ttu-id="78756-131">请求</span><span class="sxs-lookup"><span data-stu-id="78756-131">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.driveItem",
        "microsoft.graph.externalFile"
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

## <a name="known-limitations"></a><span data-ttu-id="78756-132">已知限制</span><span class="sxs-lookup"><span data-stu-id="78756-132">Known limitations</span></span>

<span data-ttu-id="78756-133">无法将查询限定为特定的连接 ID。</span><span class="sxs-lookup"><span data-stu-id="78756-133">You cannot scope a query to a particular connection ID.</span></span>

## <a name="next-steps"></a><span data-ttu-id="78756-134">后续步骤</span><span class="sxs-lookup"><span data-stu-id="78756-134">Next steps</span></span>

- [<span data-ttu-id="78756-135">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="78756-135">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)

