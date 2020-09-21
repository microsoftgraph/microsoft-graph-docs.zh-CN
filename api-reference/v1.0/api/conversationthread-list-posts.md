---
title: 列出帖子
description: '获取指定线程的帖子。 您可以同时指定父对话和线程，或者 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c63c8ada94b8f4025aa48d949cbfb94619495b21
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009994"
---
# <a name="list-posts"></a><span data-ttu-id="503d7-104">列出帖子</span><span class="sxs-lookup"><span data-stu-id="503d7-104">List posts</span></span>

<span data-ttu-id="503d7-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="503d7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="503d7-p102">获取指定线程的帖子。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="503d7-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="503d7-108">权限</span><span class="sxs-lookup"><span data-stu-id="503d7-108">Permissions</span></span>
<span data-ttu-id="503d7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="503d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="503d7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="503d7-111">Permission type</span></span>      | <span data-ttu-id="503d7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="503d7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="503d7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="503d7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="503d7-114">Group. 全部，Group。 Read. All</span><span class="sxs-lookup"><span data-stu-id="503d7-114">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="503d7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="503d7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="503d7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="503d7-116">Not supported.</span></span>    |
|<span data-ttu-id="503d7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="503d7-117">Application</span></span> | <span data-ttu-id="503d7-118">Group. 全部，Group。 Read. All</span><span class="sxs-lookup"><span data-stu-id="503d7-118">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="503d7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="503d7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="503d7-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="503d7-120">Optional query parameters</span></span>
<span data-ttu-id="503d7-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="503d7-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="503d7-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="503d7-122">Request headers</span></span>
| <span data-ttu-id="503d7-123">标头</span><span class="sxs-lookup"><span data-stu-id="503d7-123">Header</span></span>       | <span data-ttu-id="503d7-124">值</span><span class="sxs-lookup"><span data-stu-id="503d7-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="503d7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="503d7-125">Authorization</span></span>  | <span data-ttu-id="503d7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="503d7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="503d7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="503d7-128">Request body</span></span>
<span data-ttu-id="503d7-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="503d7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="503d7-130">响应</span><span class="sxs-lookup"><span data-stu-id="503d7-130">Response</span></span>

<span data-ttu-id="503d7-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Post](../resources/post.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="503d7-131">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="503d7-132">示例</span><span class="sxs-lookup"><span data-stu-id="503d7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="503d7-133">请求</span><span class="sxs-lookup"><span data-stu-id="503d7-133">Request</span></span>
<span data-ttu-id="503d7-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="503d7-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="503d7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="503d7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
# <a name="c"></a>[<span data-ttu-id="503d7-136">C#</span><span class="sxs-lookup"><span data-stu-id="503d7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-posts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="503d7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="503d7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-posts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="503d7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="503d7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-posts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="503d7-139">Java</span><span class="sxs-lookup"><span data-stu-id="503d7-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-posts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="503d7-140">响应</span><span class="sxs-lookup"><span data-stu-id="503d7-140">Response</span></span>
<span data-ttu-id="503d7-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="503d7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 523

{
  "value": [
    {
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "receivedDateTime": "datetime-value",
      "hasAttachments": true,
      "from": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "sender": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "conversationThreadId": "conversationThreadId-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

