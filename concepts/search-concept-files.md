---
title: 搜索文件（包括 externalFile）
description: 查询 API 允许您跨文件搜索（DriveItem 或外部文件）。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 95a8b99b9970ec239935ee2c35afeec581a1b35f
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703945"
---
# <a name="search-files-including-externalfile"></a><span data-ttu-id="b2964-103">搜索文件（包括 externalFile）</span><span class="sxs-lookup"><span data-stu-id="b2964-103">Search files (including externalFile)</span></span>

<span data-ttu-id="b2964-104">Microsoft Search API 允许你搜索存储在 SharePoint 或 OneDrive 中的文件。</span><span class="sxs-lookup"><span data-stu-id="b2964-104">The Microsoft Search API lets you search files stored in SharePoint or OneDrive.</span></span> <span data-ttu-id="b2964-105">它使用相关性模型，该模型利用来自 Microsoft Graph 的有关用户的关系和活动的信号。</span><span class="sxs-lookup"><span data-stu-id="b2964-105">It uses a relevance model which makes use of signals from Microsoft Graph about users' relations and activities.</span></span> <span data-ttu-id="b2964-106">这样，就可以在与 SharePoint 中列出搜索结果的 "**文件**" 选项卡一致的文件搜索体验中，返回和提升用户关注的内容。</span><span class="sxs-lookup"><span data-stu-id="b2964-106">This allows returning and promoting content that users care about, in a file search experience that is consistent with the **Files** tab that lists search results in SharePoint.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="b2964-107">此外，API 还可以通过[externalFile](/graph/api/resources/externalfile?view=graph-rest-beta)资源公开公开外部文件。</span><span class="sxs-lookup"><span data-stu-id="b2964-107">In addition, the API can surface external files exposed via the [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) resource.</span></span>

## <a name="search-sharepoint-or-onedrive-files"></a><span data-ttu-id="b2964-108">搜索 SharePoint 或 OneDrive 文件</span><span class="sxs-lookup"><span data-stu-id="b2964-108">Search SharePoint or OneDrive files</span></span>

<span data-ttu-id="b2964-109">您可以在 SharePoint 和 OneDrive 查询的搜索词中使用 KQL。</span><span class="sxs-lookup"><span data-stu-id="b2964-109">You can use KQL in search terms of queries for SharePoint and OneDrive.</span></span> <span data-ttu-id="b2964-110">例如：</span><span class="sxs-lookup"><span data-stu-id="b2964-110">For example:</span></span>

- <span data-ttu-id="b2964-111">`"query" : "contoso filetype:docx OR filetype:doc"`将查询范围限定为 Word 文档</span><span class="sxs-lookup"><span data-stu-id="b2964-111">`"query" : "contoso filetype:docx OR filetype:doc"` scopes queries to Word documents</span></span>
- <span data-ttu-id="b2964-112">`"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""`将查询范围限定为网站中的特定文件夹。</span><span class="sxs-lookup"><span data-stu-id="b2964-112">`"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>

<span data-ttu-id="b2964-113">属性限制必须在条件中指定有效的可查询托管属性名称，这样才能有效。</span><span class="sxs-lookup"><span data-stu-id="b2964-113">In order to be valid, properties restriction should specify a valid Queryable managed property name in the condition.</span></span>

### <a name="example"></a><span data-ttu-id="b2964-114">示例</span><span class="sxs-lookup"><span data-stu-id="b2964-114">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b2964-115">请求</span><span class="sxs-lookup"><span data-stu-id="b2964-115">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b2964-116">响应</span><span class="sxs-lookup"><span data-stu-id="b2964-116">Response</span></span>

<span data-ttu-id="b2964-117">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b2964-117">Here is an example of the response.</span></span>

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

## <a name="search-external-files-well-known-types"></a><span data-ttu-id="b2964-118">搜索外部文件（已知类型）</span><span class="sxs-lookup"><span data-stu-id="b2964-118">Search external files (well-known types)</span></span>

<span data-ttu-id="b2964-119">[文件共享连接器](/MicrosoftSearch/file-share-connector)是 Microsoft Search 中可用的 "开箱即用" 连接器。</span><span class="sxs-lookup"><span data-stu-id="b2964-119">[File share connector](/MicrosoftSearch/file-share-connector) is an "out of the box" connector available in Microsoft Search.</span></span> <span data-ttu-id="b2964-120">它使您能够索引文件共享上可用的文件。</span><span class="sxs-lookup"><span data-stu-id="b2964-120">It enables you to index files available on a file share.</span></span> <span data-ttu-id="b2964-121">您可以使用查询 API 查询所有外部文件。</span><span class="sxs-lookup"><span data-stu-id="b2964-121">You can use the query API to query all external files.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="example"></a><span data-ttu-id="b2964-122">示例</span><span class="sxs-lookup"><span data-stu-id="b2964-122">Example</span></span>

<span data-ttu-id="b2964-123">下面的示例返回租户的所有已配置的 externalFile 连接器，并按相关性对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="b2964-123">The following example returns all configured externalFile connector for the tenant, and sorts the results by relevance.</span></span>

#### <a name="request"></a><span data-ttu-id="b2964-124">请求</span><span class="sxs-lookup"><span data-stu-id="b2964-124">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b2964-125">响应</span><span class="sxs-lookup"><span data-stu-id="b2964-125">Response</span></span>

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

## <a name="search-all-files-including-externalfile-instances"></a><span data-ttu-id="b2964-126">搜索所有文件（包括 externalFile 实例）</span><span class="sxs-lookup"><span data-stu-id="b2964-126">Search all files (including externalFile instances)</span></span>

<span data-ttu-id="b2964-127">您可以通过在搜索请求中指定两个实体类型来搜索租户中的所有文件，包括[driveItem](/graph/api/resources/driveitem?view=graph-rest-beta)和所有外部文件。</span><span class="sxs-lookup"><span data-stu-id="b2964-127">You can search all the files in a tenant, including [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) and all external files, by specifying two entity types in the search request.</span></span>

<span data-ttu-id="b2964-128">响应在每个[searchHit](/graph/api/resources/searchhit?view=graph-rest-beta)对象\*\*\*\* 的`_sources`字段中提供了 driveItem 和 externalItem 实例的组合。</span><span class="sxs-lookup"><span data-stu-id="b2964-128">The response provide a mix of **driveItem** and externalItem instances in the `_sources` field of each [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta) object.</span></span>

### <a name="example"></a><span data-ttu-id="b2964-129">示例</span><span class="sxs-lookup"><span data-stu-id="b2964-129">Example</span></span>

<span data-ttu-id="b2964-130">下面的示例返回满足搜索词的租户的所有配置的**externalFile**连接器和**driveItem**对象。</span><span class="sxs-lookup"><span data-stu-id="b2964-130">The following example returns all configured **externalFile** connector and **driveItem** objects of the tenant's that satisfy the search terms.</span></span> <span data-ttu-id="b2964-131">它按相关性对结果进行排序。</span><span class="sxs-lookup"><span data-stu-id="b2964-131">It sorts the results by relevance.</span></span>

### <a name="request"></a><span data-ttu-id="b2964-132">请求</span><span class="sxs-lookup"><span data-stu-id="b2964-132">Request</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="b2964-133">已知限制</span><span class="sxs-lookup"><span data-stu-id="b2964-133">Known limitations</span></span>

<span data-ttu-id="b2964-134">无法将查询限定为特定 connectionId。</span><span class="sxs-lookup"><span data-stu-id="b2964-134">You cannot scope a query to a particular connectionId.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b2964-135">后续步骤</span><span class="sxs-lookup"><span data-stu-id="b2964-135">Next steps</span></span>

<span data-ttu-id="b2964-136">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="b2964-136">Find out more about:</span></span>

- [<span data-ttu-id="b2964-137">使用搜索 API</span><span class="sxs-lookup"><span data-stu-id="b2964-137">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
