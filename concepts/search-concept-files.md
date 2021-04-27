---
title: 使用 Microsoft 搜索 API 在 Microsoft Graph搜索文件
description: 可以使用 Microsoft 搜索 API 搜索存储在 OneDrive 或 SharePoint。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: dc9d27255ca5306abf85462ca8e5715fe2345dac
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048650"
---
# <a name="use-the-microsoft-search-api-to-search-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="78b85-103">使用 Microsoft 搜索 API 搜索 OneDrive 和 SharePoint</span><span class="sxs-lookup"><span data-stu-id="78b85-103">Use the Microsoft Search API to search content in OneDrive and SharePoint</span></span>

<span data-ttu-id="78b85-104">使用 Microsoft 搜索 API 搜索存储在OneDrive或SharePoint：文件、文件夹、列表、列表项或网站中的内容。</span><span class="sxs-lookup"><span data-stu-id="78b85-104">Use the Microsoft Search API to search content stored in OneDrive or SharePoint: files, folders, lists, list items, or sites.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="78b85-105">搜索 API 允许你通过指定 [searchRequest](/graph/api/resources/searchRequest)的 **entityTypes** 属性OneDrive或SharePoint中检索的内容类型。</span><span class="sxs-lookup"><span data-stu-id="78b85-105">The Search API lets you scope the types of content to retrieve in OneDrive or SharePoint by specifying the **entityTypes** property on the [searchRequest](/graph/api/resources/searchRequest).</span></span> <span data-ttu-id="78b85-106">本文介绍一些示例。</span><span class="sxs-lookup"><span data-stu-id="78b85-106">This article describes some examples.</span></span>

## <a name="example-1-search-files"></a><span data-ttu-id="78b85-107">示例 1：搜索文件</span><span class="sxs-lookup"><span data-stu-id="78b85-107">Example 1: Search files</span></span>

### <a name="request"></a><span data-ttu-id="78b85-108">请求</span><span class="sxs-lookup"><span data-stu-id="78b85-108">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="78b85-109">响应</span><span class="sxs-lookup"><span data-stu-id="78b85-109">Response</span></span>

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

## <a name="example-2-search-list-items"></a><span data-ttu-id="78b85-110">示例 2：搜索列表项</span><span class="sxs-lookup"><span data-stu-id="78b85-110">Example 2: Search list items</span></span>

### <a name="request"></a><span data-ttu-id="78b85-111">请求</span><span class="sxs-lookup"><span data-stu-id="78b85-111">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="78b85-112">响应</span><span class="sxs-lookup"><span data-stu-id="78b85-112">Response</span></span>

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

## <a name="example-3-search-sites"></a><span data-ttu-id="78b85-113">示例 3：搜索网站</span><span class="sxs-lookup"><span data-stu-id="78b85-113">Example 3: Search sites</span></span>

### <a name="request"></a><span data-ttu-id="78b85-114">请求</span><span class="sxs-lookup"><span data-stu-id="78b85-114">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="78b85-115">响应</span><span class="sxs-lookup"><span data-stu-id="78b85-115">Response</span></span>

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

## <a name="example-4-search-all-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="78b85-116">示例 4：搜索 OneDrive 和 SharePoint</span><span class="sxs-lookup"><span data-stu-id="78b85-116">Example 4: Search all content in OneDrive and SharePoint</span></span>

<span data-ttu-id="78b85-117">此示例查询登录用户OneDrive SharePoint网站中的内容。</span><span class="sxs-lookup"><span data-stu-id="78b85-117">This example queries all the content in OneDrive and SharePoint sites to which the signed-in user has read access.</span></span> <span data-ttu-id="78b85-118">响应中的 **resource** 属性返回作为 **driveItem** 对象的文件和文件夹的匹配项、作为容器的匹配项 (SharePoint将) 作为列表列出，所有其他匹配项作为 **listItem** 列出。</span><span class="sxs-lookup"><span data-stu-id="78b85-118">The **resource** property in the response returns matches that are files and folders as **driveItem** objects, matches that are containers (SharePoint lists) as **list**, and all other matches as **listItem**.</span></span>

### <a name="request"></a><span data-ttu-id="78b85-119">请求</span><span class="sxs-lookup"><span data-stu-id="78b85-119">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="78b85-120">响应</span><span class="sxs-lookup"><span data-stu-id="78b85-120">Response</span></span>

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

## <a name="example-5-use-filters-in-search-queries"></a><span data-ttu-id="78b85-121">示例 5：在搜索查询中使用筛选器</span><span class="sxs-lookup"><span data-stu-id="78b85-121">Example 5: Use filters in search queries</span></span>

<span data-ttu-id="78b85-122">您可以在查询搜索词中为 OneDrive 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="78b85-122">You can use KQL in search terms of queries for OneDrive and SharePoint.</span></span> <span data-ttu-id="78b85-123">例如：</span><span class="sxs-lookup"><span data-stu-id="78b85-123">For example:</span></span>

- <span data-ttu-id="78b85-124">`"query": "contoso filetype:docx OR filetype:doc"` 将查询范围确定为 Word 文档。</span><span class="sxs-lookup"><span data-stu-id="78b85-124">`"query": "contoso filetype:docx OR filetype:doc"` scopes the query to Word documents.</span></span>
- <span data-ttu-id="78b85-125">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` 将查询的范围确定为网站中的特定文件夹。</span><span class="sxs-lookup"><span data-stu-id="78b85-125">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>
- <span data-ttu-id="78b85-126">`"query": "contoso AND isDocument=true"` 将查询的范围确定为仅返回文档。</span><span class="sxs-lookup"><span data-stu-id="78b85-126">`"query": "contoso AND isDocument=true"` scopes the query to only return documents.</span></span> <span data-ttu-id="78b85-127">不会返回 (文件夹、文档) 的任何容器。</span><span class="sxs-lookup"><span data-stu-id="78b85-127">Any container (folder, document library) will not be returned.</span></span>
- <span data-ttu-id="78b85-128">`"query": "contoso contentclass:STS_List_Events"`将查询范围确定为存储在日历SharePoint。</span><span class="sxs-lookup"><span data-stu-id="78b85-128">`"query": "contoso contentclass:STS_List_Events"` scopes the query to Calendar events stored in SharePoint.</span></span>
- <span data-ttu-id="78b85-129">`"query": "contoso (LastModifiedTime > 2021-02-01 AND Created > 2021-02-01)"`将查询的范围确定为按SharePoint OneDrive筛选项目</span><span class="sxs-lookup"><span data-stu-id="78b85-129">`"query": "contoso (LastModifiedTime > 2021-02-01 AND Created > 2021-02-01)"` scopes the query to filter SharePoint and OneDrive items by date</span></span>

<span data-ttu-id="78b85-130">为了有效，属性限制应在条件中指定有效的可查询托管属性名称。</span><span class="sxs-lookup"><span data-stu-id="78b85-130">In order to be valid, properties restriction should specify a valid, queryable managed property name in the condition.</span></span>

## <a name="example-6-specify-select-properties"></a><span data-ttu-id="78b85-131">示例 6：指定选择属性</span><span class="sxs-lookup"><span data-stu-id="78b85-131">Example 6: Specify select properties</span></span>

<span data-ttu-id="78b85-132">可以在响应中指定希望返回的字段，作为 [响应中 searchHit](/graph/api/resources/searchhit)对象的 **fields** 子属性的一部分。</span><span class="sxs-lookup"><span data-stu-id="78b85-132">You can specify the fields you want back in the response, as part of the **fields** sub-property of a [searchHit](/graph/api/resources/searchhit) object in the response.</span></span> <span data-ttu-id="78b85-133">这是一种通过线路减少响应或请求一些不是开箱即用架构一部分的特定属性的方法。</span><span class="sxs-lookup"><span data-stu-id="78b85-133">This is a way to either trim down the response over the wire, or to request some specific properties that are not part of the out-of-the-box schema.</span></span>

<span data-ttu-id="78b85-134">请注意，属性选择仅适用于 **listItem，** 因为这是 Microsoft SharePoint中唯一Graph自定义属性的实体。</span><span class="sxs-lookup"><span data-stu-id="78b85-134">Note that property selection is only available for **listItem** since this is the only SharePoint entity in Microsoft Graph that supports custom properties.</span></span>

<span data-ttu-id="78b85-135">若要检索 **driveItem** 的自定义属性，请改为查询 **listItem。**</span><span class="sxs-lookup"><span data-stu-id="78b85-135">To retrieve a custom property for a **driveItem**, query **listItem** instead.</span></span>

### <a name="request"></a><span data-ttu-id="78b85-136">请求</span><span class="sxs-lookup"><span data-stu-id="78b85-136">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="78b85-137">响应</span><span class="sxs-lookup"><span data-stu-id="78b85-137">Response</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="78b85-138">已知限制</span><span class="sxs-lookup"><span data-stu-id="78b85-138">Known limitations</span></span>

<span data-ttu-id="78b85-139">在搜索 **驱动器** 时，需要在 **queryString** 中包含文档库名称中的术语。</span><span class="sxs-lookup"><span data-stu-id="78b85-139">When searching for **drive**, you need to include in the **queryString** a term contained in the name of the document library.</span></span> <span data-ttu-id="78b85-140">不支持 `*` 查询，并且不会返回所有可用驱动器。</span><span class="sxs-lookup"><span data-stu-id="78b85-140">Querying `*` is not supported and does not return all available drives.</span></span>

## <a name="next-steps"></a><span data-ttu-id="78b85-141">后续步骤</span><span class="sxs-lookup"><span data-stu-id="78b85-141">Next steps</span></span>

- [<span data-ttu-id="78b85-142">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="78b85-142">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview)
