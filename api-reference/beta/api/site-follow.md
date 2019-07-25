---
author: learafa
title: 关注网站
description: 关注用户的网站/网站。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8ba6766305970d3dc2cf040e8a274039a2f6da34
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869699"
---
# <a name="follow-site"></a><span data-ttu-id="1c952-103">关注网站</span><span class="sxs-lookup"><span data-stu-id="1c952-103">Follow site</span></span> 

<span data-ttu-id="1c952-104">关注用户的[网站](../resources/site.md)或多个网站。</span><span class="sxs-lookup"><span data-stu-id="1c952-104">Follow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c952-105">权限</span><span class="sxs-lookup"><span data-stu-id="1c952-105">Permissions</span></span>

<span data-ttu-id="1c952-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c952-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="1c952-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c952-108">Permission type</span></span>             | <span data-ttu-id="1c952-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c952-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1c952-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c952-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c952-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c952-111">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="1c952-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c952-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c952-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c952-113">Not supported.</span></span>                              |
| <span data-ttu-id="1c952-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c952-114">Application</span></span>                            | <span data-ttu-id="1c952-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c952-115">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1c952-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c952-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/add
```

## <a name="request-body"></a><span data-ttu-id="1c952-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c952-117">Request body</span></span>

<span data-ttu-id="1c952-118">在请求正文中, 提供包含下表中所述的 id 参数的 JSON 对象的数组。</span><span class="sxs-lookup"><span data-stu-id="1c952-118">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="1c952-119">名称</span><span class="sxs-lookup"><span data-stu-id="1c952-119">Name</span></span>                 | <span data-ttu-id="1c952-120">值</span><span class="sxs-lookup"><span data-stu-id="1c952-120">Value</span></span>  | <span data-ttu-id="1c952-121">说明</span><span class="sxs-lookup"><span data-stu-id="1c952-121">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="1c952-122">id</span><span class="sxs-lookup"><span data-stu-id="1c952-122">id</span></span>                 | <span data-ttu-id="1c952-123">string</span><span class="sxs-lookup"><span data-stu-id="1c952-123">string</span></span> | <span data-ttu-id="1c952-124">项的[唯一标识符](../resources/site.md#id-property)。</span><span class="sxs-lookup"><span data-stu-id="1c952-124">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |


## <a name="response"></a><span data-ttu-id="1c952-125">响应</span><span class="sxs-lookup"><span data-stu-id="1c952-125">Response</span></span> 

* <span data-ttu-id="1c952-126">如果请求成功, 此方法将返回已遵循的网站数组。</span><span class="sxs-lookup"><span data-stu-id="1c952-126">If the request is successful, this method returns an array of sites that were followed.</span></span>  
* <span data-ttu-id="1c952-127">如果在执行任何指定的网站时出现错误, 则此方法将返回`207`状态代码, 并且响应正文将包含包含[Error](/graph/errors)对象和 siteIds 的条目的数组, 这些条目指示无法遵循哪些网站。</span><span class="sxs-lookup"><span data-stu-id="1c952-127">If an error occured while following any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites were unable to be followed.</span></span>

## <a name="example"></a><span data-ttu-id="1c952-128">示例</span><span class="sxs-lookup"><span data-stu-id="1c952-128">Example</span></span>

<span data-ttu-id="1c952-129">下面的示例展示了如何跟踪多个网站。</span><span class="sxs-lookup"><span data-stu-id="1c952-129">The following example shows how to follow multiple sites.</span></span> 

### <a name="request"></a><span data-ttu-id="1c952-130">请求</span><span class="sxs-lookup"><span data-stu-id="1c952-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1c952-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1c952-131">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1c952-132">C#</span><span class="sxs-lookup"><span data-stu-id="1c952-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c952-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="1c952-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1c952-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="1c952-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1c952-135">Java</span><span class="sxs-lookup"><span data-stu-id="1c952-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/follow-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1c952-136">响应</span><span class="sxs-lookup"><span data-stu-id="1c952-136">Response</span></span>

<span data-ttu-id="1c952-137">如果成功, 它将返回以下 JSON 响应。</span><span class="sxs-lookup"><span data-stu-id="1c952-137">If successful, it returns the following JSON response.</span></span> 

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

<span data-ttu-id="1c952-138">如果发生错误, 它将返回以下 JSON 响应</span><span class="sxs-lookup"><span data-stu-id="1c952-138">If an error occured, it returns the following JSON response</span></span> 

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
  "tocPath": "Sites/Follow site",
  "suppressions": [
  ]
} -->
