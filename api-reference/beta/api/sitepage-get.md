---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: 获取网站中的页面
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a97ee8f52a6276664b3349c01c545c711707ceea
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330363"
---
# <a name="get-a-page-in-the-site-pages-list-of-a-site"></a><span data-ttu-id="94b3c-102">在网站的 "网站页面" 列表中获取页面</span><span class="sxs-lookup"><span data-stu-id="94b3c-102">Get a page in the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94b3c-103">返回[网站][]的 "网站页面"[列表][]中的[sitePage][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="94b3c-103">Returns the metadata for a [sitePage][] in the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[网站]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="94b3c-107">权限</span><span class="sxs-lookup"><span data-stu-id="94b3c-107">Permissions</span></span>

<span data-ttu-id="94b3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94b3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94b3c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="94b3c-110">Permission type</span></span>      | <span data-ttu-id="94b3c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94b3c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94b3c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94b3c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94b3c-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94b3c-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="94b3c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94b3c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94b3c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="94b3c-115">Not supported.</span></span>    |
|<span data-ttu-id="94b3c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="94b3c-116">Application</span></span> | <span data-ttu-id="94b3c-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94b3c-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94b3c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94b3c-118">HTTP request</span></span>

```http
GET /sites/{site-id}/pages/{page-id}
```

## <a name="example"></a><span data-ttu-id="94b3c-119">示例</span><span class="sxs-lookup"><span data-stu-id="94b3c-119">Example</span></span>

##### <a name="request"></a><span data-ttu-id="94b3c-120">请求</span><span class="sxs-lookup"><span data-stu-id="94b3c-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-page", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET /sites/{site-id}/pages/{page-id}
```

##### <a name="response"></a><span data-ttu-id="94b3c-121">响应</span><span class="sxs-lookup"><span data-stu-id="94b3c-121">Response</span></span>

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
  "suppressions": []
}
-->
