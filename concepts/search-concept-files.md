---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索文件
description: 您可以使用 Microsoft 搜索 API 搜索存储在 OneDrive 或 SharePoint 中的文件。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 37021df3124b1ff24cb0edde9a8253cf0c980fda
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597296"
---
# <a name="use-the-microsoft-search-api-to-search-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="d3616-103">使用 Microsoft 搜索 API 在 OneDrive 和 SharePoint 中搜索内容</span><span class="sxs-lookup"><span data-stu-id="d3616-103">Use the Microsoft Search API to search content in OneDrive and SharePoint</span></span>

<span data-ttu-id="d3616-104">使用 Microsoft Search API 搜索存储在 OneDrive 或 SharePoint 中的内容：文件、文件夹、列表、列表项或网站。</span><span class="sxs-lookup"><span data-stu-id="d3616-104">Use the Microsoft Search API to search content stored in OneDrive or SharePoint: files, folders, lists, list items, or sites.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="d3616-105">搜索 API 允许您通过指定 [searchRequest](/graph/api/resources/searchRequest)上的 **entityTypes** 属性来限定要在 OneDrive 或 SharePoint 中检索的内容类型。</span><span class="sxs-lookup"><span data-stu-id="d3616-105">The Search API lets you scope the types of content to retrieve in OneDrive or SharePoint by specifying the **entityTypes** property on the [searchRequest](/graph/api/resources/searchRequest).</span></span> <span data-ttu-id="d3616-106">本文介绍了一些示例。</span><span class="sxs-lookup"><span data-stu-id="d3616-106">This article describes some examples.</span></span>

## <a name="example-1-search-files"></a><span data-ttu-id="d3616-107">示例1：搜索文件</span><span class="sxs-lookup"><span data-stu-id="d3616-107">Example 1: Search files</span></span>

### <a name="request"></a><span data-ttu-id="d3616-108">请求</span><span class="sxs-lookup"><span data-stu-id="d3616-108">Request</span></span>

```HTTP
POST /search/query
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

### <a name="response"></a><span data-ttu-id="d3616-109">响应</span><span class="sxs-lookup"><span data-stu-id="d3616-109">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
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
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0",
                  "driveId": "da61a2b0-4120-4a3f-812b-0fc0d79bf16b",
                  "sharepointIds": {
                      "listId": "c61d1892-ca82-4f53-b16f-6bb8a379e2b2",
                      "listItemId": "1027",
                      "listItemUniqueId": "E320AFEB-AD73-46A2-83D7-985FAA4B206D"
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

## <a name="example-2-search-list-items"></a><span data-ttu-id="d3616-110">示例2：搜索列表项</span><span class="sxs-lookup"><span data-stu-id="d3616-110">Example 2: Search list items</span></span>

### <a name="request"></a><span data-ttu-id="d3616-111">请求</span><span class="sxs-lookup"><span data-stu-id="d3616-111">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="d3616-112">响应</span><span class="sxs-lookup"><span data-stu-id="d3616-112">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
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
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/Lists/Issue tracker list/DispForm.aspx?ID=1",
                "sharepointIds": {
                    "listId": "33498de0-d695-4d23-ac26-e1bf95a3206e",
                    "listItemId": "13"
                },
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
                  "sharepointIds":{
                    "listId":"da61a2b0-4120-4a3f-812b-0fc0d79bf16b"  
                  },
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

## <a name="example-3-search-sites"></a><span data-ttu-id="d3616-113">示例3：搜索网站</span><span class="sxs-lookup"><span data-stu-id="d3616-113">Example 3: Search sites</span></span>

### <a name="request"></a><span data-ttu-id="d3616-114">请求</span><span class="sxs-lookup"><span data-stu-id="d3616-114">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="d3616-115">响应</span><span class="sxs-lookup"><span data-stu-id="d3616-115">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
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

## <a name="example-4-search-all-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="d3616-116">示例4：搜索 OneDrive 和 SharePoint 中的所有内容</span><span class="sxs-lookup"><span data-stu-id="d3616-116">Example 4: Search all content in OneDrive and SharePoint</span></span>

<span data-ttu-id="d3616-117">此示例查询已登录用户有权读取的 OneDrive 和 SharePoint 网站中的所有内容。</span><span class="sxs-lookup"><span data-stu-id="d3616-117">This example queries all the content in OneDrive and SharePoint sites to which the signed-in user has read access.</span></span> <span data-ttu-id="d3616-118">响应中的 **resource** 属性返回的是作为 **driveItem** 对象的文件和文件夹的匹配项、作为列表的容器 (SharePoint) 列表中的匹配项，以及所有其他与 **列表** 项匹配的匹配 **项。**</span><span class="sxs-lookup"><span data-stu-id="d3616-118">The **resource** property in the response returns matches that are files and folders as **driveItem** objects, matches that are containers (SharePoint lists) as **list**, and all other matches as **listItem**.</span></span>

### <a name="request"></a><span data-ttu-id="d3616-119">请求</span><span class="sxs-lookup"><span data-stu-id="d3616-119">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="d3616-120">响应</span><span class="sxs-lookup"><span data-stu-id="d3616-120">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
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
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0",
                  "driveId": "da61a2b0-4120-4a3f-812b-0fc0d79bf16b",
                  "sharepointIds": {
                      "listId": "c61d1892-ca82-4f53-b16f-6bb8a379e2b2",
                      "listItemId": "1027",
                      "listItemUniqueId": "E320AFEB-AD73-46A2-83D7-985FAA4B206D"
                  }
                },
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

## <a name="example-5-use-filters-in-search-queries"></a><span data-ttu-id="d3616-121">示例5：在搜索查询中使用筛选器</span><span class="sxs-lookup"><span data-stu-id="d3616-121">Example 5: Use filters in search queries</span></span>

<span data-ttu-id="d3616-122">您可以在 OneDrive 和 SharePoint 查询的搜索词中使用 KQL。</span><span class="sxs-lookup"><span data-stu-id="d3616-122">You can use KQL in search terms of queries for OneDrive and SharePoint.</span></span> <span data-ttu-id="d3616-123">例如：</span><span class="sxs-lookup"><span data-stu-id="d3616-123">For example:</span></span>

- <span data-ttu-id="d3616-124">`"query": "contoso filetype:docx OR filetype:doc"` 将查询范围限定为 Word 文档。</span><span class="sxs-lookup"><span data-stu-id="d3616-124">`"query": "contoso filetype:docx OR filetype:doc"` scopes the query to Word documents.</span></span>
- <span data-ttu-id="d3616-125">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` 将查询范围限定为网站中的特定文件夹。</span><span class="sxs-lookup"><span data-stu-id="d3616-125">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>
- <span data-ttu-id="d3616-126">`"query": "contoso AND isDocument=true"` 将查询范围限定为仅返回文档。</span><span class="sxs-lookup"><span data-stu-id="d3616-126">`"query": "contoso AND isDocument=true"` scopes the query to only return documents.</span></span> <span data-ttu-id="d3616-127">将不会返回任何容器 (文件夹、文档库) 。</span><span class="sxs-lookup"><span data-stu-id="d3616-127">Any container (folder, document library) will not be returned.</span></span>
- <span data-ttu-id="d3616-128">`"query": "contoso contentclass:STS_List_Events"` 将查询范围限定为存储在 SharePoint 中的日历事件。</span><span class="sxs-lookup"><span data-stu-id="d3616-128">`"query": "contoso contentclass:STS_List_Events"` scopes the query to Calendar events stored in SharePoint.</span></span>

<span data-ttu-id="d3616-129">属性限制必须在条件中指定有效且可查询的托管属性名称，这样才能有效。</span><span class="sxs-lookup"><span data-stu-id="d3616-129">In order to be valid, properties restriction should specify a valid, queryable managed property name in the condition.</span></span>

## <a name="example-6-specify-select-properties"></a><span data-ttu-id="d3616-130">示例6：指定选择属性</span><span class="sxs-lookup"><span data-stu-id="d3616-130">Example 6: Specify select properties</span></span>

<span data-ttu-id="d3616-131">您可以在响应中的 [searchHit](/graph/api/resources/searchhit)对象的 **fields** 子属性的一部分中指定要返回的字段。</span><span class="sxs-lookup"><span data-stu-id="d3616-131">You can specify the fields you want back in the response, as part of the **fields** sub-property of a [searchHit](/graph/api/resources/searchhit) object in the response.</span></span> <span data-ttu-id="d3616-132">这是在网络上修整响应的一种方法，或者请求不是现成架构的一部分的某些特定属性。</span><span class="sxs-lookup"><span data-stu-id="d3616-132">This is a way to either trim down the response over the wire, or to request some specific properties that are not part of the out-of-the-box schema.</span></span>

<span data-ttu-id="d3616-133">请注意，属性选择仅 **适用于列表，因为** 这是 Microsoft Graph 中支持自定义属性的唯一 SharePoint 实体。</span><span class="sxs-lookup"><span data-stu-id="d3616-133">Note that property selection is only available for **listItem** since this is the only SharePoint entity in Microsoft Graph that supports custom properties.</span></span>

<span data-ttu-id="d3616-134">若要检索 **driveItem** 的自定义属性，请 **改为** 查询列表。</span><span class="sxs-lookup"><span data-stu-id="d3616-134">To retrieve a custom property for a **driveItem**, query **listItem** instead.</span></span>

### <a name="request"></a><span data-ttu-id="d3616-135">请求</span><span class="sxs-lookup"><span data-stu-id="d3616-135">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="d3616-136">响应</span><span class="sxs-lookup"><span data-stu-id="d3616-136">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
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
                "sharepointIds": {
                    "listId": "33498de0-d695-4d23-ac26-e1bf95a3206e",
                    "listItemId": "13"
                },
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

## <a name="known-limitations"></a><span data-ttu-id="d3616-137">已知限制</span><span class="sxs-lookup"><span data-stu-id="d3616-137">Known limitations</span></span>

<span data-ttu-id="d3616-138">搜索 **驱动器** 时，需要在 **查询字符串** 中包含文档库名称中包含的术语查询。</span><span class="sxs-lookup"><span data-stu-id="d3616-138">When searching for **drive**, you need to include in the **queryString** a term contained in the name of the document library.</span></span> <span data-ttu-id="d3616-139">查询 `*` 不受支持，并且不会返回所有可用的驱动器。</span><span class="sxs-lookup"><span data-stu-id="d3616-139">Querying `*` is not supported and does not return all available drives.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d3616-140">后续步骤</span><span class="sxs-lookup"><span data-stu-id="d3616-140">Next steps</span></span>

- [<span data-ttu-id="d3616-141">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="d3616-141">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview)
