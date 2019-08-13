---
author: learafa
title: 取消追随网站
description: 取消追随用户的网站
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 12cb4cc6d5336924ca7c5df45df94f9c891dad1f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363688"
---
# <a name="unfollow-site"></a><span data-ttu-id="56d66-103">取消追随网站</span><span class="sxs-lookup"><span data-stu-id="56d66-103">Unfollow site</span></span> 

<span data-ttu-id="56d66-104">取消追随用户的[网站](../resources/site.md)或多个网站。</span><span class="sxs-lookup"><span data-stu-id="56d66-104">Unfollow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="56d66-105">权限</span><span class="sxs-lookup"><span data-stu-id="56d66-105">Permissions</span></span>

<span data-ttu-id="56d66-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56d66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="56d66-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="56d66-108">Permission type</span></span>             | <span data-ttu-id="56d66-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56d66-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="56d66-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56d66-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="56d66-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d66-111">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="56d66-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56d66-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56d66-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="56d66-113">Not supported.</span></span>                              |
| <span data-ttu-id="56d66-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="56d66-114">Application</span></span>                            | <span data-ttu-id="56d66-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d66-115">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="56d66-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56d66-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/remove
```

## <a name="request-body"></a><span data-ttu-id="56d66-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="56d66-117">Request body</span></span>

<span data-ttu-id="56d66-118">在请求正文中, 提供包含下表中所述的 id 参数的 JSON 对象的数组。</span><span class="sxs-lookup"><span data-stu-id="56d66-118">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="56d66-119">名称</span><span class="sxs-lookup"><span data-stu-id="56d66-119">Name</span></span>                 | <span data-ttu-id="56d66-120">值</span><span class="sxs-lookup"><span data-stu-id="56d66-120">Value</span></span>  | <span data-ttu-id="56d66-121">说明</span><span class="sxs-lookup"><span data-stu-id="56d66-121">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="56d66-122">id</span><span class="sxs-lookup"><span data-stu-id="56d66-122">id</span></span>                 | <span data-ttu-id="56d66-123">string</span><span class="sxs-lookup"><span data-stu-id="56d66-123">string</span></span> | <span data-ttu-id="56d66-124">项的[唯一标识符](../resources/site.md#id-property)。</span><span class="sxs-lookup"><span data-stu-id="56d66-124">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |

## <a name="response"></a><span data-ttu-id="56d66-125">响应</span><span class="sxs-lookup"><span data-stu-id="56d66-125">Response</span></span>

* <span data-ttu-id="56d66-126">如果请求成功, 此方法将返回不包含`204`任何内容的状态代码。</span><span class="sxs-lookup"><span data-stu-id="56d66-126">If the request is successful, this method returns a `204` status code with no content.</span></span>  
* <span data-ttu-id="56d66-127">如果在 unfollowing 任何指定的网站时发生错误, 此方法将返回一个`207`状态代码, 并且响应正文将包含一个包含[Error](/graph/errors)对象和 siteIds 的条目的数组, 这些条目指示哪些网站无法未点击。</span><span class="sxs-lookup"><span data-stu-id="56d66-127">If an error occured while unfollowing any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites unable to be unfollowed.</span></span>

## <a name="example"></a><span data-ttu-id="56d66-128">示例</span><span class="sxs-lookup"><span data-stu-id="56d66-128">Example</span></span>

<span data-ttu-id="56d66-129">下面的示例演示如何取消追随多个网站。</span><span class="sxs-lookup"><span data-stu-id="56d66-129">The following example shows how to unfollow multiple sites.</span></span>

### <a name="request"></a><span data-ttu-id="56d66-130">请求</span><span class="sxs-lookup"><span data-stu-id="56d66-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="56d66-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="56d66-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-site", "scopes": "sites.readwrite.all" } -->

```http
POST /users/{user-id}/followedSites/remove
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="56d66-132">C#</span><span class="sxs-lookup"><span data-stu-id="56d66-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56d66-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56d66-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="56d66-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="56d66-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="56d66-135">Java</span><span class="sxs-lookup"><span data-stu-id="56d66-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unfollow-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="56d66-136">响应</span><span class="sxs-lookup"><span data-stu-id="56d66-136">Response</span></span>

<span data-ttu-id="56d66-137">如果成功, 它将返回以下 JSON 响应。</span><span class="sxs-lookup"><span data-stu-id="56d66-137">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 204 No Content
```

<span data-ttu-id="56d66-138">如果发生错误, 它将返回以下 JSON 响应</span><span class="sxs-lookup"><span data-stu-id="56d66-138">If an error occured, it returns the following JSON response</span></span> 

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
        }
    ]
}
```  

<!-- {
  "type": "#page.annotation",
  "description": "Unfollow sharepoint site/sites for a user.",
  "keywords": "unfollow site",
  "section": "documentation",
  "tocPath": "Sites/Unfollow site",
  "suppressions": [
  ]
} -->
