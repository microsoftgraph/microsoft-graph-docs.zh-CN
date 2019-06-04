---
author: learafa
title: 关注网站
description: 关注用户的网站/网站。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: ba7bd36b08b63735d793de8602244f612202f122
ms.sourcegitcommit: 895a03cb2706a9b3a2236b30d6a7e9f5cbc6a89e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34692778"
---
# <a name="follow-site"></a><span data-ttu-id="bb940-103">关注网站</span><span class="sxs-lookup"><span data-stu-id="bb940-103">Follow site</span></span> 

<span data-ttu-id="bb940-104">关注用户的[网站](../resources/site.md)或多个网站。</span><span class="sxs-lookup"><span data-stu-id="bb940-104">Follow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb940-105">权限</span><span class="sxs-lookup"><span data-stu-id="bb940-105">Permissions</span></span>

<span data-ttu-id="bb940-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb940-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="bb940-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb940-108">Permission type</span></span>             | <span data-ttu-id="bb940-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb940-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bb940-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb940-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb940-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb940-111">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="bb940-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb940-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb940-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb940-113">Not supported.</span></span>                              |
| <span data-ttu-id="bb940-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb940-114">Application</span></span>                            | <span data-ttu-id="bb940-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb940-115">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bb940-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb940-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/add
```

## <a name="request-body"></a><span data-ttu-id="bb940-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb940-117">Request body</span></span>

<span data-ttu-id="bb940-118">在请求正文中, 提供包含下表中所述的 id 参数的 JSON 对象的数组。</span><span class="sxs-lookup"><span data-stu-id="bb940-118">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="bb940-119">名称</span><span class="sxs-lookup"><span data-stu-id="bb940-119">Name</span></span>                 | <span data-ttu-id="bb940-120">值</span><span class="sxs-lookup"><span data-stu-id="bb940-120">Value</span></span>  | <span data-ttu-id="bb940-121">说明</span><span class="sxs-lookup"><span data-stu-id="bb940-121">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="bb940-122">id</span><span class="sxs-lookup"><span data-stu-id="bb940-122">id</span></span>                 | <span data-ttu-id="bb940-123">string</span><span class="sxs-lookup"><span data-stu-id="bb940-123">string</span></span> | <span data-ttu-id="bb940-124">项的[唯一标识符](../resources/site.md#id-property)。</span><span class="sxs-lookup"><span data-stu-id="bb940-124">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |


## <a name="response"></a><span data-ttu-id="bb940-125">响应</span><span class="sxs-lookup"><span data-stu-id="bb940-125">Response</span></span> 

* <span data-ttu-id="bb940-126">如果请求成功, 此方法将返回已遵循的网站数组。</span><span class="sxs-lookup"><span data-stu-id="bb940-126">If the request is successful, this method returns an array of sites that were followed.</span></span>  
* <span data-ttu-id="bb940-127">如果在执行任何指定的网站时出现错误, 则此方法将返回`207`状态代码, 并且响应正文将包含包含[Error](/graph/errors)对象和 siteIds 的条目的数组, 这些条目指示无法遵循哪些网站。</span><span class="sxs-lookup"><span data-stu-id="bb940-127">If an error occured while following any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites were unable to be followed.</span></span>

## <a name="example"></a><span data-ttu-id="bb940-128">示例</span><span class="sxs-lookup"><span data-stu-id="bb940-128">Example</span></span>

<span data-ttu-id="bb940-129">下面的示例展示了如何跟踪多个网站。</span><span class="sxs-lookup"><span data-stu-id="bb940-129">The following example shows how to follow multiple sites.</span></span> 

### <a name="request"></a><span data-ttu-id="bb940-130">请求</span><span class="sxs-lookup"><span data-stu-id="bb940-130">Request</span></span>

<!-- { "blockType": "request", "name": "follow-site", "scopes": "sites.readwrite.all" } -->

```http
POST /users/{user-id}/followedSites/add
Content-Type: application/json

{
    "value":
    [
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740"
        },
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851"
        }
    ] 
}
```
### <a name="response"></a><span data-ttu-id="bb940-131">响应</span><span class="sxs-lookup"><span data-stu-id="bb940-131">Response</span></span>

<span data-ttu-id="bb940-132">如果成功, 它将返回以下 JSON 响应。</span><span class="sxs-lookup"><span data-stu-id="bb940-132">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
            "webUrl": "http://contoso.sharepoint.com/sites/SiteFollowed1",
            "name": "SiteFollowed1",
            "sharepointIds": {
                "siteId": "da60e844-ba1d-49bc-b4d4-d5e36bae9019",
                "siteUrl": "http://contoso.sharepoint.com/sites/SiteFollowed1",
                "webId": "712a596e-90a1-49e3-9b48-bfa80bee8740"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        },
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
            "webUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
            "name": "SiteFollowed2",
            "sharepointIds": {
                "siteId": "da60e844-ba1d-49bc-b4d4-d5e36bae9019",
                "siteUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
                "webId": "0271110f-634f-4300-a841-3a8a2e851851"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        }
    ]
}
```

<span data-ttu-id="bb940-133">如果发生错误, 它将返回以下 JSON 响应</span><span class="sxs-lookup"><span data-stu-id="bb940-133">If an error occured, it returns the following JSON response</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 207 Multi-Status
Content-type: application/json
{
    "value": [
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,512a596e-90a1-49e3-9b48-bfa80bee8740",
            "error": {
                "@odata.type": "#oneDrive.error",
                "code": "invalidRequest",
                "message": "The site Id information that is provided in the request is incorrect",
                "innerError": {
                    "code": "invalidRequest",
                    "errorType": "expected",
                    "message": "The site Id information that is provided in the request is incorrect",
                    "stackTrace": "",
                    "throwSite": ""
                }
            }
        },
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
            "webUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
            "name": "SiteFollowed2",
            "sharepointIds": {
                "siteId": "da60e844-ba1d-49bc-b4d4-d5e36bae9019",
                "siteUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
                "webId": "0271110f-634f-4300-a841-3a8a2e851851"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        }
    ]
}
```  

<!-- {
  "type": "#page.annotation",
  "description": "Follow sharepoint site for a user.",
  "keywords": "follow site",
  "section": "documentation",
  "tocPath": "Sites/Follow site"
} -->
