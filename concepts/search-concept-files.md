---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索文件
description: 您可以使用 Microsoft 搜索 API 搜索存储在 OneDrive 或 SharePoint 中的文件。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 38915d4ec4e38f5bd41e67e31d5708caf34272ec
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192539"
---
# <a name="use-the-microsoft-search-api-to-search-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="bc3c2-103">使用 Microsoft 搜索 API 在 OneDrive 和 SharePoint 中搜索内容</span><span class="sxs-lookup"><span data-stu-id="bc3c2-103">Use the Microsoft Search API to search content in OneDrive and SharePoint</span></span>

<span data-ttu-id="bc3c2-104">使用 Microsoft Search API 搜索存储在 OneDrive 或 SharePoint 中的内容：文件、文件夹、列表、列表项或网站。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-104">Use the Microsoft Search API to search content stored in OneDrive or SharePoint: files, folders, lists, list items, or sites.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="bc3c2-105">搜索 API 允许您通过指定[searchRequest](/graph/api/resources/searchRequest?view=graph-rest-beta&preserve-view=true)上的**entityTypes**属性来限定要在 OneDrive 或 SharePoint 中检索的内容类型。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-105">The Search API lets you scope the types of content to retrieve in OneDrive or SharePoint by specifying the **entityTypes** property on the [searchRequest](/graph/api/resources/searchRequest?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="bc3c2-106">本文的后面部分显示了几个示例：</span><span class="sxs-lookup"><span data-stu-id="bc3c2-106">The later part of this article shows a few examples:</span></span>

- [<span data-ttu-id="bc3c2-107">示例1：搜索文件</span><span class="sxs-lookup"><span data-stu-id="bc3c2-107">Example 1: Search files</span></span>](#example-1-search-files)
- [<span data-ttu-id="bc3c2-108">示例2：搜索列表项</span><span class="sxs-lookup"><span data-stu-id="bc3c2-108">Example 2: Search list items</span></span>](#example-2-search-list-items)
- [<span data-ttu-id="bc3c2-109">示例3：搜索网站</span><span class="sxs-lookup"><span data-stu-id="bc3c2-109">Example 3: Search sites</span></span>](#example-3-search-sites)
- [<span data-ttu-id="bc3c2-110">示例4：搜索 OneDrive 和 SharePoint 中的所有内容</span><span class="sxs-lookup"><span data-stu-id="bc3c2-110">Example 4: Search all content in OneDrive and SharePoint</span></span>](#example-4-search-all-content-in-onedrive-and-sharepoint)

## <a name="specify-select-properties"></a><span data-ttu-id="bc3c2-111">指定选择属性</span><span class="sxs-lookup"><span data-stu-id="bc3c2-111">Specify select properties</span></span>

<span data-ttu-id="bc3c2-112">您可以在响应中的[searchHit](/graph/api/resources/searchhit?view=graph-rest-beta&preserve-view=true)对象的**fields**子属性的一部分中指定要返回的字段。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-112">You can specify the fields you want back in the response, as part of the **fields** sub-property of a [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta&preserve-view=true) object in the response.</span></span> <span data-ttu-id="bc3c2-113">这是在网络上修整响应的一种方法，或者请求不是现成架构的一部分的某些特定属性。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-113">This is a way to either trim down the response over the wire, or to request some specific properties that are not part of the out-of-the-box schema.</span></span>

<span data-ttu-id="bc3c2-114">请注意，属性选择仅 **适用于列表，因为** 这是 Microsoft Graph 中支持自定义属性的唯一 SharePoint 实体。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-114">Note that property selection is only available for **listItem** since this is the only SharePoint entity in Microsoft Graph that supports custom properties.</span></span>

<span data-ttu-id="bc3c2-115">若要检索 **driveItem**的自定义属性，请 **改为** 查询列表。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-115">To retrieve a custom property for a **driveItem**, query **listItem** instead.</span></span>

### <a name="request"></a><span data-ttu-id="bc3c2-116">请求</span><span class="sxs-lookup"><span data-stu-id="bc3c2-116">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="bc3c2-117">响应</span><span class="sxs-lookup"><span data-stu-id="bc3c2-117">Response</span></span>

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

## <a name="use-filters-in-search-queries"></a><span data-ttu-id="bc3c2-118">在搜索查询中使用筛选器</span><span class="sxs-lookup"><span data-stu-id="bc3c2-118">Use filters in search queries</span></span>

<span data-ttu-id="bc3c2-119">您可以在 OneDrive 和 SharePoint 查询的搜索词中使用 KQL。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-119">You can use KQL in search terms of queries for OneDrive and SharePoint.</span></span> <span data-ttu-id="bc3c2-120">例如：</span><span class="sxs-lookup"><span data-stu-id="bc3c2-120">For example:</span></span>

- <span data-ttu-id="bc3c2-121">`"query": "contoso filetype:docx OR filetype:doc"` 将查询范围限定为 Word 文档。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-121">`"query": "contoso filetype:docx OR filetype:doc"` scopes the query to Word documents.</span></span>
- <span data-ttu-id="bc3c2-122">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` 将查询范围限定为网站中的特定文件夹。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-122">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>
- <span data-ttu-id="bc3c2-123">`"query": "contoso AND isDocument=true"` 将查询范围限定为仅返回文档。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-123">`"query": "contoso AND isDocument=true"` scopes the query to only return documents.</span></span> <span data-ttu-id="bc3c2-124">将不会返回任何容器 (文件夹、文档库) 。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-124">Any container (folder, document library) will not be returned.</span></span>
- <span data-ttu-id="bc3c2-125">`"query": "contoso contentclass:STS_List_Events"` 将查询范围限定为存储在 SharePoint 中的日历事件。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-125">`"query": "contoso contentclass:STS_List_Events"` scopes the query to Calendar events stored in SharePoint.</span></span>

<span data-ttu-id="bc3c2-126">属性限制必须在条件中指定有效且可查询的托管属性名称，这样才能有效。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-126">In order to be valid, properties restriction should specify a valid, queryable managed property name in the condition.</span></span>

## <a name="example-1-search-files"></a><span data-ttu-id="bc3c2-127">示例1：搜索文件</span><span class="sxs-lookup"><span data-stu-id="bc3c2-127">Example 1: Search files</span></span>

### <a name="request"></a><span data-ttu-id="bc3c2-128">请求</span><span class="sxs-lookup"><span data-stu-id="bc3c2-128">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="bc3c2-129">响应</span><span class="sxs-lookup"><span data-stu-id="bc3c2-129">Response</span></span>

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

## <a name="example-2-search-list-items"></a><span data-ttu-id="bc3c2-130">示例2：搜索列表项</span><span class="sxs-lookup"><span data-stu-id="bc3c2-130">Example 2: Search list items</span></span>

### <a name="request"></a><span data-ttu-id="bc3c2-131">请求</span><span class="sxs-lookup"><span data-stu-id="bc3c2-131">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="bc3c2-132">响应</span><span class="sxs-lookup"><span data-stu-id="bc3c2-132">Response</span></span>

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

## <a name="example-3-search-sites"></a><span data-ttu-id="bc3c2-133">示例3：搜索网站</span><span class="sxs-lookup"><span data-stu-id="bc3c2-133">Example 3: Search sites</span></span>

### <a name="request"></a><span data-ttu-id="bc3c2-134">请求</span><span class="sxs-lookup"><span data-stu-id="bc3c2-134">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="bc3c2-135">响应</span><span class="sxs-lookup"><span data-stu-id="bc3c2-135">Response</span></span>

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

## <a name="example-4-search-all-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="bc3c2-136">示例4：搜索 OneDrive 和 SharePoint 中的所有内容</span><span class="sxs-lookup"><span data-stu-id="bc3c2-136">Example 4: Search all content in OneDrive and SharePoint</span></span>

<span data-ttu-id="bc3c2-137">此示例查询已登录用户有权读取的 OneDrive 和 SharePoint 网站中的所有内容。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-137">This example queries all the content in OneDrive and SharePoint sites to which the signed-in user has read access.</span></span> <span data-ttu-id="bc3c2-138">响应中的**resource**属性返回的是作为**driveItem**对象的文件和文件夹的匹配项、作为列表的容器 (SharePoint) 列表中的匹配项，以及所有其他与**列表**项匹配的匹配**项。**</span><span class="sxs-lookup"><span data-stu-id="bc3c2-138">The **resource** property in the response returns matches that are files and folders as **driveItem** objects, matches that are containers (SharePoint lists) as **list**, and all other matches as **listItem**.</span></span>

### <a name="request"></a><span data-ttu-id="bc3c2-139">请求</span><span class="sxs-lookup"><span data-stu-id="bc3c2-139">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="bc3c2-140">响应</span><span class="sxs-lookup"><span data-stu-id="bc3c2-140">Response</span></span>

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

## <a name="next-steps"></a><span data-ttu-id="bc3c2-141">后续步骤</span><span class="sxs-lookup"><span data-stu-id="bc3c2-141">Next steps</span></span>

- [<span data-ttu-id="bc3c2-142">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="bc3c2-142">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
