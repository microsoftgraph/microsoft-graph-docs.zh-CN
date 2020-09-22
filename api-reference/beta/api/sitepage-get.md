---
author: rahmit
description: 返回网站的 "网站页面" 列表中的 sitePage 的元数据。
ms.date: 03/15/2018
title: 获取网站中的页面
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2c7e93ea3fc2378bb056dbd60a8616eefcfbae20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044450"
---
# <a name="get-a-page-in-the-site-pages-list-of-a-site"></a><span data-ttu-id="e1b41-103">在网站的 "网站页面" 列表中获取页面</span><span class="sxs-lookup"><span data-stu-id="e1b41-103">Get a page in the site pages list of a site</span></span>

<span data-ttu-id="e1b41-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1b41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1b41-105">返回[网站][]的 "网站页面"[列表][]中的[sitePage][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="e1b41-105">Returns the metadata for a [sitePage][] in the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="e1b41-109">权限</span><span class="sxs-lookup"><span data-stu-id="e1b41-109">Permissions</span></span>

<span data-ttu-id="e1b41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1b41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1b41-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1b41-112">Permission type</span></span>      | <span data-ttu-id="e1b41-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1b41-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1b41-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1b41-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e1b41-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b41-115">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1b41-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1b41-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1b41-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1b41-117">Not supported.</span></span>    |
|<span data-ttu-id="e1b41-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1b41-118">Application</span></span> | <span data-ttu-id="e1b41-119">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b41-119">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1b41-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1b41-120">HTTP request</span></span>

```http
GET /sites/{site-id}/pages/{page-id}
```

## <a name="example"></a><span data-ttu-id="e1b41-121">示例</span><span class="sxs-lookup"><span data-stu-id="e1b41-121">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e1b41-122">请求</span><span class="sxs-lookup"><span data-stu-id="e1b41-122">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e1b41-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1b41-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-page", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```msgraph-interactive
GET /sites/{site-id}/pages/{page-id}
```
# <a name="c"></a>[<span data-ttu-id="e1b41-124">C#</span><span class="sxs-lookup"><span data-stu-id="e1b41-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1b41-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1b41-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1b41-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1b41-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e1b41-127">响应</span><span class="sxs-lookup"><span data-stu-id="e1b41-127">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.sitePage", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2",
    "eTag": "75bc70e2-6587-45be-8493-c99a956b2e05,7",
    "createdDateTime": "2016-12-06T20:04:40Z",
    "lastModifiedDateTime": "2016-12-06T20:05:09Z",
    "webUrl": "https://www.contoso.com/sites/Engineering/SitePages/Events.aspx",
    "createdBy": {
        "user": {
            "email": "rahmit@microsoft.com",
            "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
            "displayName": "Rahul Mittal (ODSP)"
        }
    },
    "lastModifiedBy": {
        "user": {
            "email": "rahmit@microsoft.com",
            "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
            "displayName": "Rahul Mittal (ODSP)"
        }
    },
    "parentReference": {
        "id": "eb3bfd48-56f8-4c1e-8312-e58588b22e7c"
    },
    "contentType": {
        "id": "0x0101009D1CB255DA76424F860D91F20E6C411800C9E7033636784C4B88A284B1823C45FD",
        "name": "Site Page"
    },
    "description": "",
    "title": "Upcoming Events",
    "publishingState": {
        "level": "published",
        "versionId": "1.0"
    },
    "webParts": [
        {
            "type": "rte",
            "data": {
                "innerHTML": "<p>Here are the team's upcoming events:</p>"
            }
        },
        {
            "type": "d1d91016-032f-456d-98a4-721247c305e8",
            "data": {
                "title": "Events",
                "description": "Display upcoming events",
                "serverProcessedContent": {
                    "htmlStrings": {},
                    "searchablePlainTexts": {
                        "title": ""
                    },
                    "imageSources": {},
                    "links": {
                        "baseUrl": "https://www.contoso.com/sites/Engineering"
                    },
                    "componentDependencies": {
                        "layoutComponentId": "8ac0c53c-e8d0-4e3e-87d0-7449eb0d4027"
                    }
                },
                "dataVersion": "1.0",
                "properties": {
                    "selectedListId": "032e08ab-89b0-4d8f-bc10-73094233615c",
                    "selectedCategory": "",
                    "dateRangeOption": 0,
                    "startDate": "",
                    "endDate": "",
                    "isOnSeeAllPage": false,
                    "layoutId": "FilmStrip",
                    "dataProviderId": "Event",
                    "webId": "0764c419-1ecc-4126-ba32-0c25ae0fffe8",
                    "siteId": "6b4ffc7a-cfc2-4a76-903a-1cc3686dee23"
                }
            }
        }
    ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get a page in a site",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Enumerate",
  "suppressions": [
  ]
}
-->


