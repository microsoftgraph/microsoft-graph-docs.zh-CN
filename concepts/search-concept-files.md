---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索文件
description: 您可以使用 Microsoft 搜索 API 搜索存储在 OneDrive 或 SharePoint 中的文件。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: f080dae0413f2f261a05299299235aaaed16f7fb
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48417924"
---
# <a name="use-the-microsoft-search-api-to-search-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="a2384-103">使用 Microsoft 搜索 API 在 OneDrive 和 SharePoint 中搜索内容</span><span class="sxs-lookup"><span data-stu-id="a2384-103">Use the Microsoft Search API to search content in OneDrive and SharePoint</span></span>

<span data-ttu-id="a2384-104">使用 Microsoft Search API 搜索存储在 OneDrive 或 SharePoint 中的内容：文件、文件夹、列表、列表项或网站。</span><span class="sxs-lookup"><span data-stu-id="a2384-104">Use the Microsoft Search API to search content stored in OneDrive or SharePoint: files, folders, lists, list items, or sites.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="a2384-105">搜索 API 允许您通过指定[searchRequest](/graph/api/resources/searchRequest?view=graph-rest-beta&preserve-view=true)上的**entityTypes**属性来限定要在 OneDrive 或 SharePoint 中检索的内容类型。</span><span class="sxs-lookup"><span data-stu-id="a2384-105">The Search API lets you scope the types of content to retrieve in OneDrive or SharePoint by specifying the **entityTypes** property on the [searchRequest](/graph/api/resources/searchRequest?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="a2384-106">本文的后面部分显示了几个示例：</span><span class="sxs-lookup"><span data-stu-id="a2384-106">The later part of this article shows a few examples:</span></span>

- [<span data-ttu-id="a2384-107">示例1：搜索文件</span><span class="sxs-lookup"><span data-stu-id="a2384-107">Example 1: Search files</span></span>](#example-1-search-files)
- [<span data-ttu-id="a2384-108">示例2：搜索列表项</span><span class="sxs-lookup"><span data-stu-id="a2384-108">Example 2: Search list items</span></span>](#example-2-search-list-items)
- [<span data-ttu-id="a2384-109">示例3：搜索网站</span><span class="sxs-lookup"><span data-stu-id="a2384-109">Example 3: Search sites</span></span>](#example-3-search-sites)
- [<span data-ttu-id="a2384-110">示例4：搜索 OneDrive 和 SharePoint 中的所有内容</span><span class="sxs-lookup"><span data-stu-id="a2384-110">Example 4: Search all content in OneDrive and SharePoint</span></span>](#example-4-search-all-content-in-onedrive-and-sharepoint)
- [<span data-ttu-id="a2384-111">示例5：在搜索查询中使用筛选器</span><span class="sxs-lookup"><span data-stu-id="a2384-111">Example 5: Use filters in search queries</span></span>](#example-5-use-filters-in-search-queries)
- [<span data-ttu-id="a2384-112">示例6：指定选择属性</span><span class="sxs-lookup"><span data-stu-id="a2384-112">Example 6: Specify select properties</span></span>](#example-6-specify-select-properties)


## <a name="example-1-search-files"></a><span data-ttu-id="a2384-113">示例1：搜索文件</span><span class="sxs-lookup"><span data-stu-id="a2384-113">Example 1: Search files</span></span>

### <a name="request"></a><span data-ttu-id="a2384-114">请求</span><span class="sxs-lookup"><span data-stu-id="a2384-114">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "driveItem"
      ],
      "query": {
        "queryString": "contoso"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a2384-115">响应</span><span class="sxs-lookup"><span data-stu-id="a2384-115">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "FlULeN/ui/1GjLx1rUfio5UAAEl",
              "rank": 1,
              "summary": "<c0>Contoso</c0> Detailed Design <ddd/>",
              "resource": {
                "@odata.type": "#microsoft.graph.driveItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                "name": "web_part_test_long Notebook",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/contoso-designs.docx",
                "createdBy": {
                 "user": {
                   "displayName": "Michaelvincent Santos;Provisioning User"
                  }
                },
                "lastModifiedBy": {
                  "user": {
                    "displayName": "Richard Mayer"
                  }
                },
                "parentReference": {
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
                }
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

## <a name="example-2-search-list-items"></a><span data-ttu-id="a2384-116">示例2：搜索列表项</span><span class="sxs-lookup"><span data-stu-id="a2384-116">Example 2: Search list items</span></span>

### <a name="request"></a><span data-ttu-id="a2384-117">请求</span><span class="sxs-lookup"><span data-stu-id="a2384-117">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "listItem"
      ],
      "query": {
        "queryString": "contoso"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a2384-118">响应</span><span class="sxs-lookup"><span data-stu-id="a2384-118">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "FlULeN/ui/1GjLx1rUfio5UAAEl",
              "rank": 1,
              "summary": "",
              "resource": {
                "@odata.type": "#microsoft.graph.listItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                "name": "web_part_test_long Notebook",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/Lists/Issue tracker list/DispForm.aspx?ID=1"
                "createdBy": {
                 "user": {
                   "displayName": "Michaelvincent Santos;Provisioning User"
                  }
                },
                "lastModifiedBy": {
                  "user": {
                    "displayName": "Richard Mayer"
                  }
                },
                "parentReference": {
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
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

## <a name="example-3-search-sites"></a><span data-ttu-id="a2384-119">示例3：搜索网站</span><span class="sxs-lookup"><span data-stu-id="a2384-119">Example 3: Search sites</span></span>

### <a name="request"></a><span data-ttu-id="a2384-120">请求</span><span class="sxs-lookup"><span data-stu-id="a2384-120">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "site"
      ],
      "query": {
        "queryString": "contoso"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a2384-121">响应</span><span class="sxs-lookup"><span data-stu-id="a2384-121">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "contoso.sharepoint.com,6598ee0b-0f5f-4416-a0ae-66d864efb43a,60024ce8-e74d-4d63-a939-ad00cd738670",
              "rank": 1,
              "summary": "",
              "resource": {
                "@odata.type": "#microsoft.graph.site",
                "id": "contoso.sharepoint.com,6598ee0b-0f5f-4416-a0ae-66d864efb43a,60024ce8-e74d-4d63-a939-ad00cd738670",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "description": "Contoso Communication Site",
                "lastModifiedDateTime": "2020-08-30T06:41:56Z",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/"
              }
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="example-4-search-all-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="a2384-122">示例4：搜索 OneDrive 和 SharePoint 中的所有内容</span><span class="sxs-lookup"><span data-stu-id="a2384-122">Example 4: Search all content in OneDrive and SharePoint</span></span>

<span data-ttu-id="a2384-123">此示例查询已登录用户有权读取的 OneDrive 和 SharePoint 网站中的所有内容。</span><span class="sxs-lookup"><span data-stu-id="a2384-123">This example queries all the content in OneDrive and SharePoint sites to which the signed-in user has read access.</span></span> <span data-ttu-id="a2384-124">响应中的**resource**属性返回的是作为**driveItem**对象的文件和文件夹的匹配项、作为列表的容器 (SharePoint) 列表中的匹配项，以及所有其他与**列表**项匹配的匹配**项。**</span><span class="sxs-lookup"><span data-stu-id="a2384-124">The **resource** property in the response returns matches that are files and folders as **driveItem** objects, matches that are containers (SharePoint lists) as **list**, and all other matches as **listItem**.</span></span>

### <a name="request"></a><span data-ttu-id="a2384-125">请求</span><span class="sxs-lookup"><span data-stu-id="a2384-125">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "driveItem", "listItem", "list"
      ],
      "query": {
        "queryString": "contoso"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a2384-126">响应</span><span class="sxs-lookup"><span data-stu-id="a2384-126">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "@odata.type": "#microsoft.graph.searchHitsContainer",
              "hitId": "FlULeN/ui/1GjLx1rUfio5UAAEl",
              "rank": 1,
              "summary": "<c0>Contoso</c0> Detailed Design <ddd/>",
              "resource": {
                "@odata.type": "#microsoft.graph.driveItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                "name": "web_part_test_long Notebook",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/contoso-designs.docx",
                "createdBy": {
                 "user": {
                   "displayName": "Michaelvincent Santos;Provisioning User"
                  }
                },
                "lastModifiedBy": {
                  "user": {
                    "displayName": "Richard Mayer"
                  }
                },
                "parentReference": {
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
                }
                "fileSystemInfo": {
                  "createdDateTime": "2019-06-10T06:37:43Z",
                  "lastModifiedDateTime": "2019-06-10T06:37:43Z"
                }
              }
            },
            {
              "@odata.type": "#microsoft.graph.searchHit",
              "hitId": "51eef59e-5d49-4d28-96f0-864cf90765e0",
              "rank": 2,
              "summary": "",
              "resource": {
                "@odata.type": "#microsoft.graph.list",
                "displayName": "Contoso - Documents",
                "id": "51eef59e-5d49-4d28-96f0-864cf90765e0",
                "description": "",
                "lastModifiedDateTime": "2020-07-08T18:17:59+00:00",
                "name": "Shared Documents",
                "parentReference": {
                "siteId": "microsoft.sharepoint-df.com,220fd155-0ea2-477c-a816-5c08fdc45f5d,fad16ab6-0736-4fbc-a053-087296b47c99"
                },
                "webUrl": "https://microsoft.sharepoint-df.com/teams/spoppe/collab/TaskBoard/Contoso/Shared Documents/Forms/AllItems.aspx"
              }
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="example-5-use-filters-in-search-queries"></a><span data-ttu-id="a2384-127">示例5：在搜索查询中使用筛选器</span><span class="sxs-lookup"><span data-stu-id="a2384-127">Example 5: Use filters in search queries</span></span>

<span data-ttu-id="a2384-128">您可以在 OneDrive 和 SharePoint 查询的搜索词中使用 KQL。</span><span class="sxs-lookup"><span data-stu-id="a2384-128">You can use KQL in search terms of queries for OneDrive and SharePoint.</span></span> <span data-ttu-id="a2384-129">例如：</span><span class="sxs-lookup"><span data-stu-id="a2384-129">For example:</span></span>

- <span data-ttu-id="a2384-130">`"query": "contoso filetype:docx OR filetype:doc"` 将查询范围限定为 Word 文档。</span><span class="sxs-lookup"><span data-stu-id="a2384-130">`"query": "contoso filetype:docx OR filetype:doc"` scopes the query to Word documents.</span></span>
- <span data-ttu-id="a2384-131">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` 将查询范围限定为网站中的特定文件夹。</span><span class="sxs-lookup"><span data-stu-id="a2384-131">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>
- <span data-ttu-id="a2384-132">`"query": "contoso AND isDocument=true"` 将查询范围限定为仅返回文档。</span><span class="sxs-lookup"><span data-stu-id="a2384-132">`"query": "contoso AND isDocument=true"` scopes the query to only return documents.</span></span> <span data-ttu-id="a2384-133">将不会返回任何容器 (文件夹、文档库) 。</span><span class="sxs-lookup"><span data-stu-id="a2384-133">Any container (folder, document library) will not be returned.</span></span>
- <span data-ttu-id="a2384-134">`"query": "contoso contentclass:STS_List_Events"` 将查询范围限定为存储在 SharePoint 中的日历事件。</span><span class="sxs-lookup"><span data-stu-id="a2384-134">`"query": "contoso contentclass:STS_List_Events"` scopes the query to Calendar events stored in SharePoint.</span></span>

<span data-ttu-id="a2384-135">属性限制必须在条件中指定有效且可查询的托管属性名称，这样才能有效。</span><span class="sxs-lookup"><span data-stu-id="a2384-135">In order to be valid, properties restriction should specify a valid, queryable managed property name in the condition.</span></span>

## <a name="example-6-specify-select-properties"></a><span data-ttu-id="a2384-136">示例6：指定选择属性</span><span class="sxs-lookup"><span data-stu-id="a2384-136">Example 6: Specify select properties</span></span>

<span data-ttu-id="a2384-137">您可以在响应中的[searchHit](/graph/api/resources/searchhit?view=graph-rest-beta&preserve-view=true)对象的**fields**子属性的一部分中指定要返回的字段。</span><span class="sxs-lookup"><span data-stu-id="a2384-137">You can specify the fields you want back in the response, as part of the **fields** sub-property of a [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta&preserve-view=true) object in the response.</span></span> <span data-ttu-id="a2384-138">这是在网络上修整响应的一种方法，或者请求不是现成架构的一部分的某些特定属性。</span><span class="sxs-lookup"><span data-stu-id="a2384-138">This is a way to either trim down the response over the wire, or to request some specific properties that are not part of the out-of-the-box schema.</span></span>

<span data-ttu-id="a2384-139">请注意，属性选择仅 **适用于列表，因为** 这是 Microsoft Graph 中支持自定义属性的唯一 SharePoint 实体。</span><span class="sxs-lookup"><span data-stu-id="a2384-139">Note that property selection is only available for **listItem** since this is the only SharePoint entity in Microsoft Graph that supports custom properties.</span></span>

<span data-ttu-id="a2384-140">若要检索 **driveItem**的自定义属性，请 **改为** 查询列表。</span><span class="sxs-lookup"><span data-stu-id="a2384-140">To retrieve a custom property for a **driveItem**, query **listItem** instead.</span></span>

### <a name="request"></a><span data-ttu-id="a2384-141">请求</span><span class="sxs-lookup"><span data-stu-id="a2384-141">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "listItem"
      ],
      "query": {
        "queryString": "contoso"
      },
      "fields": [
          "title",
          "contentclass"
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a2384-142">响应</span><span class="sxs-lookup"><span data-stu-id="a2384-142">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "contoso.sharepoint.com,6598ee0b-0f5f-4416-a0ae-66d864efb43a,60024ce8-e74d-4d63-a939-ad00cd738670",
              "rank": 1,
              "summary": "",
              "resource": {
                "@odata.type": "#microsoft.graph.listItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/contoso-designs.docx",
                "parentReference": {
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
                },
                "fields": {
                  "contentclass": "STS_ListItem_GenericList",
                  "title": "Contoso issue "
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

## <a name="known-limitations"></a><span data-ttu-id="a2384-143">已知限制</span><span class="sxs-lookup"><span data-stu-id="a2384-143">Known limitations</span></span>

<span data-ttu-id="a2384-144">搜索 **驱动器**时，需要在 **查询字符串** 中包含文档库名称中包含的术语查询。</span><span class="sxs-lookup"><span data-stu-id="a2384-144">When searching for **drive**, you need to include in the **queryString** a term contained in the name of the document library.</span></span> <span data-ttu-id="a2384-145">查询 `*` 不受支持，并且不会返回所有可用的驱动器。</span><span class="sxs-lookup"><span data-stu-id="a2384-145">Querying `*` is not supported and does not return all available drives.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a2384-146">后续步骤</span><span class="sxs-lookup"><span data-stu-id="a2384-146">Next steps</span></span>

- [<span data-ttu-id="a2384-147">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="a2384-147">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
