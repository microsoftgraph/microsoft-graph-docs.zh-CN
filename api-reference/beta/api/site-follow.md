---
author: learafa
title: 关注网站
description: 关注用户的网站/网站。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 18044f2a6459fa7d145d29bbf2a66d8b2eee7f5f
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475780"
---
# <a name="follow-site"></a><span data-ttu-id="725da-103">关注网站</span><span class="sxs-lookup"><span data-stu-id="725da-103">Follow site</span></span> 

<span data-ttu-id="725da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="725da-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="725da-105">关注用户 [的网站或](../resources/site.md) 多个网站。</span><span class="sxs-lookup"><span data-stu-id="725da-105">Follow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="725da-106">权限</span><span class="sxs-lookup"><span data-stu-id="725da-106">Permissions</span></span>

<span data-ttu-id="725da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="725da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="725da-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="725da-109">Permission type</span></span>             | <span data-ttu-id="725da-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="725da-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="725da-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="725da-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="725da-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="725da-112">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="725da-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="725da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="725da-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="725da-114">Not supported.</span></span>                              |
| <span data-ttu-id="725da-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="725da-115">Application</span></span>                            | <span data-ttu-id="725da-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="725da-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="725da-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="725da-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/add
```

## <a name="request-body"></a><span data-ttu-id="725da-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="725da-118">Request body</span></span>

<span data-ttu-id="725da-119">在请求正文中，提供包含下表中提到的 id 参数的 JSON 对象的数组。</span><span class="sxs-lookup"><span data-stu-id="725da-119">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="725da-120">名称</span><span class="sxs-lookup"><span data-stu-id="725da-120">Name</span></span>                 | <span data-ttu-id="725da-121">值</span><span class="sxs-lookup"><span data-stu-id="725da-121">Value</span></span>  | <span data-ttu-id="725da-122">说明</span><span class="sxs-lookup"><span data-stu-id="725da-122">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="725da-123">id</span><span class="sxs-lookup"><span data-stu-id="725da-123">id</span></span>                 | <span data-ttu-id="725da-124">string</span><span class="sxs-lookup"><span data-stu-id="725da-124">string</span></span> | <span data-ttu-id="725da-125">项的[唯一标识符](../resources/site.md#id-property)。</span><span class="sxs-lookup"><span data-stu-id="725da-125">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |


## <a name="response"></a><span data-ttu-id="725da-126">响应</span><span class="sxs-lookup"><span data-stu-id="725da-126">Response</span></span> 

* <span data-ttu-id="725da-127">如果请求成功，此方法将返回一组已关注的网站。</span><span class="sxs-lookup"><span data-stu-id="725da-127">If the request is successful, this method returns an array of sites that were followed.</span></span>  
* <span data-ttu-id="725da-128">如果在关注任何指定网站时发生错误，此方法将返回状态代码，响应正文将包含包含错误对象和 siteId 的条目数组，这些条目指示无法关注哪些 `207` 网站[](/graph/errors)。</span><span class="sxs-lookup"><span data-stu-id="725da-128">If an error occurred while following any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites were unable to be followed.</span></span>

## <a name="example"></a><span data-ttu-id="725da-129">示例</span><span class="sxs-lookup"><span data-stu-id="725da-129">Example</span></span>

<span data-ttu-id="725da-130">以下示例演示如何关注多个网站。</span><span class="sxs-lookup"><span data-stu-id="725da-130">The following example shows how to follow multiple sites.</span></span> 

### <a name="request"></a><span data-ttu-id="725da-131">请求</span><span class="sxs-lookup"><span data-stu-id="725da-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="725da-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="725da-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="725da-133">C#</span><span class="sxs-lookup"><span data-stu-id="725da-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="725da-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="725da-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="725da-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="725da-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="725da-136">Java</span><span class="sxs-lookup"><span data-stu-id="725da-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/follow-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="725da-137">响应</span><span class="sxs-lookup"><span data-stu-id="725da-137">Response</span></span>

<span data-ttu-id="725da-138">如果成功，它将返回以下 JSON 响应。</span><span class="sxs-lookup"><span data-stu-id="725da-138">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```http
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

<span data-ttu-id="725da-139">如果发生错误，它将返回以下 JSON 响应</span><span class="sxs-lookup"><span data-stu-id="725da-139">If an error occured, it returns the following JSON response</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```http
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


