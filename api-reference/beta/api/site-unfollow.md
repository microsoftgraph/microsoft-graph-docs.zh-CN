---
author: learafa
title: 取消关注网站
description: 取消关注用户的网站
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 6d938fc0c02cfc876449edd5bf656770df9190c4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475750"
---
# <a name="unfollow-site"></a><span data-ttu-id="cb84a-103">取消关注网站</span><span class="sxs-lookup"><span data-stu-id="cb84a-103">Unfollow site</span></span> 

<span data-ttu-id="cb84a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb84a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb84a-105">取消关注用户 [网站或](../resources/site.md) 多个网站。</span><span class="sxs-lookup"><span data-stu-id="cb84a-105">Unfollow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb84a-106">权限</span><span class="sxs-lookup"><span data-stu-id="cb84a-106">Permissions</span></span>

<span data-ttu-id="cb84a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb84a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="cb84a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb84a-109">Permission type</span></span>             | <span data-ttu-id="cb84a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb84a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="cb84a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb84a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb84a-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb84a-112">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="cb84a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb84a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb84a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb84a-114">Not supported.</span></span>                              |
| <span data-ttu-id="cb84a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb84a-115">Application</span></span>                            | <span data-ttu-id="cb84a-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb84a-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cb84a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb84a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/remove
```

## <a name="request-body"></a><span data-ttu-id="cb84a-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb84a-118">Request body</span></span>

<span data-ttu-id="cb84a-119">在请求正文中，提供包含下表中提到的 id 参数的 JSON 对象的数组。</span><span class="sxs-lookup"><span data-stu-id="cb84a-119">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="cb84a-120">名称</span><span class="sxs-lookup"><span data-stu-id="cb84a-120">Name</span></span>                 | <span data-ttu-id="cb84a-121">值</span><span class="sxs-lookup"><span data-stu-id="cb84a-121">Value</span></span>  | <span data-ttu-id="cb84a-122">说明</span><span class="sxs-lookup"><span data-stu-id="cb84a-122">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="cb84a-123">id</span><span class="sxs-lookup"><span data-stu-id="cb84a-123">id</span></span>                 | <span data-ttu-id="cb84a-124">string</span><span class="sxs-lookup"><span data-stu-id="cb84a-124">string</span></span> | <span data-ttu-id="cb84a-125">项的[唯一标识符](../resources/site.md#id-property)。</span><span class="sxs-lookup"><span data-stu-id="cb84a-125">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |

## <a name="response"></a><span data-ttu-id="cb84a-126">响应</span><span class="sxs-lookup"><span data-stu-id="cb84a-126">Response</span></span>

* <span data-ttu-id="cb84a-127">如果请求成功，此方法将返回 `204` 无内容的状态代码。</span><span class="sxs-lookup"><span data-stu-id="cb84a-127">If the request is successful, this method returns a `204` status code with no content.</span></span>  
* <span data-ttu-id="cb84a-128">如果在取消关注任何指定网站时发生错误，此方法将返回状态代码，响应正文将包含一组包含错误对象和 siteId 的条目，这些条目指示哪些网站无法取消安装。 `207` [](/graph/errors)</span><span class="sxs-lookup"><span data-stu-id="cb84a-128">If an error occured while unfollowing any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites unable to be unfollowed.</span></span>

## <a name="example"></a><span data-ttu-id="cb84a-129">示例</span><span class="sxs-lookup"><span data-stu-id="cb84a-129">Example</span></span>

<span data-ttu-id="cb84a-130">以下示例演示如何取消关注多个网站。</span><span class="sxs-lookup"><span data-stu-id="cb84a-130">The following example shows how to unfollow multiple sites.</span></span>

### <a name="request"></a><span data-ttu-id="cb84a-131">请求</span><span class="sxs-lookup"><span data-stu-id="cb84a-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cb84a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb84a-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cb84a-133">C#</span><span class="sxs-lookup"><span data-stu-id="cb84a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb84a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb84a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb84a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb84a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb84a-136">Java</span><span class="sxs-lookup"><span data-stu-id="cb84a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unfollow-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="cb84a-137">响应</span><span class="sxs-lookup"><span data-stu-id="cb84a-137">Response</span></span>

<span data-ttu-id="cb84a-138">如果成功，它将返回以下 JSON 响应。</span><span class="sxs-lookup"><span data-stu-id="cb84a-138">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="cb84a-139">如果发生错误，它将返回以下 JSON 响应</span><span class="sxs-lookup"><span data-stu-id="cb84a-139">If an error occured, it returns the following JSON response</span></span> 

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


