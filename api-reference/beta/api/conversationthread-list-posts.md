---
title: 列出帖子
description: '获取指定线程的帖子。 您可以同时指定父对话和线程，或者 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0c339a7ea867d68b46816728b8bb16af67b4c6c1
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48371573"
---
# <a name="list-posts"></a><span data-ttu-id="fe848-104">列出帖子</span><span class="sxs-lookup"><span data-stu-id="fe848-104">List posts</span></span>

<span data-ttu-id="fe848-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe848-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe848-p102">获取指定线程的帖子。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="fe848-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe848-108">权限</span><span class="sxs-lookup"><span data-stu-id="fe848-108">Permissions</span></span>
<span data-ttu-id="fe848-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe848-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe848-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe848-111">Permission type</span></span>      | <span data-ttu-id="fe848-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe848-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe848-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe848-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fe848-114">Group. 全部，Group。 Read. All</span><span class="sxs-lookup"><span data-stu-id="fe848-114">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="fe848-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe848-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe848-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe848-116">Not supported.</span></span>    |
|<span data-ttu-id="fe848-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe848-117">Application</span></span> | <span data-ttu-id="fe848-118">Group. 全部，Group。 Read. All</span><span class="sxs-lookup"><span data-stu-id="fe848-118">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe848-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe848-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="fe848-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fe848-120">Optional query parameters</span></span>
<span data-ttu-id="fe848-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fe848-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fe848-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe848-122">Request headers</span></span>
| <span data-ttu-id="fe848-123">标头</span><span class="sxs-lookup"><span data-stu-id="fe848-123">Header</span></span>       | <span data-ttu-id="fe848-124">值</span><span class="sxs-lookup"><span data-stu-id="fe848-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fe848-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe848-125">Authorization</span></span>  | <span data-ttu-id="fe848-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe848-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe848-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe848-128">Request body</span></span>
<span data-ttu-id="fe848-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe848-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe848-130">响应</span><span class="sxs-lookup"><span data-stu-id="fe848-130">Response</span></span>

<span data-ttu-id="fe848-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Post](../resources/post.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fe848-131">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe848-132">示例</span><span class="sxs-lookup"><span data-stu-id="fe848-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe848-133">请求</span><span class="sxs-lookup"><span data-stu-id="fe848-133">Request</span></span>
<span data-ttu-id="fe848-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe848-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fe848-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe848-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts
```
# <a name="c"></a>[<span data-ttu-id="fe848-136">C#</span><span class="sxs-lookup"><span data-stu-id="fe848-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-posts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe848-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe848-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-posts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe848-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe848-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-posts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fe848-139">响应</span><span class="sxs-lookup"><span data-stu-id="fe848-139">Response</span></span>
<span data-ttu-id="fe848-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe848-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
