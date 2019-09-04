---
title: 列出帖子
description: '获取指定线程的帖子。 您可以同时指定父对话和线程, 或者 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d351a0b5063f4e2fe2ed8140c5f8f38c8cb5b625
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719673"
---
# <a name="list-posts"></a><span data-ttu-id="81094-104">列出帖子</span><span class="sxs-lookup"><span data-stu-id="81094-104">List posts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81094-p102">获取指定线程的帖子。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="81094-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="81094-107">权限</span><span class="sxs-lookup"><span data-stu-id="81094-107">Permissions</span></span>
<span data-ttu-id="81094-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81094-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81094-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="81094-110">Permission type</span></span>      | <span data-ttu-id="81094-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="81094-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81094-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81094-112">Delegated (work or school account)</span></span> | <span data-ttu-id="81094-113">Group. 全部, Group。 Read. All</span><span class="sxs-lookup"><span data-stu-id="81094-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="81094-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81094-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81094-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="81094-115">Not supported.</span></span>    |
|<span data-ttu-id="81094-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="81094-116">Application</span></span> | <span data-ttu-id="81094-117">Group. 全部, Group。 Read. All</span><span class="sxs-lookup"><span data-stu-id="81094-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81094-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81094-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="81094-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="81094-119">Optional query parameters</span></span>
<span data-ttu-id="81094-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="81094-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="81094-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="81094-121">Request headers</span></span>
| <span data-ttu-id="81094-122">标头</span><span class="sxs-lookup"><span data-stu-id="81094-122">Header</span></span>       | <span data-ttu-id="81094-123">值</span><span class="sxs-lookup"><span data-stu-id="81094-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="81094-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="81094-124">Authorization</span></span>  | <span data-ttu-id="81094-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="81094-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="81094-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="81094-127">Request body</span></span>
<span data-ttu-id="81094-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="81094-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81094-129">响应</span><span class="sxs-lookup"><span data-stu-id="81094-129">Response</span></span>

<span data-ttu-id="81094-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Post](../resources/post.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="81094-130">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="81094-131">示例</span><span class="sxs-lookup"><span data-stu-id="81094-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81094-132">请求</span><span class="sxs-lookup"><span data-stu-id="81094-132">Request</span></span>
<span data-ttu-id="81094-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="81094-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="81094-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="81094-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="81094-135">C#</span><span class="sxs-lookup"><span data-stu-id="81094-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-posts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81094-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81094-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-posts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="81094-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="81094-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-posts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="81094-138">响应</span><span class="sxs-lookup"><span data-stu-id="81094-138">Response</span></span>
<span data-ttu-id="81094-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="81094-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts",
    "value":[
        {
            "@odata.etag":"W/\"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK\"",
            "id":"AQMkADgAAAIJbQAAAA==",
            "createdDateTime":"2018-01-11T17:36:17Z",
            "lastModifiedDateTime":"2018-01-11T17:36:17Z",
            "importance": "normal",
            "changeKey":"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK",
            "categories":[

            ],
            "receivedDateTime":"2018-01-11T17:36:17Z",
            "hasAttachments":false,
            "body":{
                "contentType":"html",
                "content":"<html><body></body></html>"
            },
            "from":{
                "emailAddress":{
                    "name":"Marketing",
                    "address":"Marketing@M365B489948.onmicrosoft.com"
                }
            },
            "sender":{
                "emailAddress":{
                    "name":"Marketing",
                    "address":"Marketing@M365B489948.onmicrosoft.com"
                }
            }
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
