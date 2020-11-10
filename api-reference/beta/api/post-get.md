---
title: 获取帖子
description: '获取指定的线程中帖子的属性和关系。 您可以同时指定父 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4001b298983668ebf0ebf213fd8e36fa3168a5e7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982260"
---
# <a name="get-post"></a><span data-ttu-id="5173a-104">获取帖子</span><span class="sxs-lookup"><span data-stu-id="5173a-104">Get post</span></span>

<span data-ttu-id="5173a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5173a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5173a-p102">获取指定线程中的帖子的属性和关系。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="5173a-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="5173a-108">由于 **帖子** 资源支持 [扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取 **帖子** 实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="5173a-108">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="5173a-109">权限</span><span class="sxs-lookup"><span data-stu-id="5173a-109">Permissions</span></span>
<span data-ttu-id="5173a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5173a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5173a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5173a-112">Permission type</span></span>      | <span data-ttu-id="5173a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5173a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5173a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5173a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5173a-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5173a-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5173a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5173a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5173a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5173a-117">Not supported.</span></span>    |
|<span data-ttu-id="5173a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5173a-118">Application</span></span> | <span data-ttu-id="5173a-119">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5173a-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5173a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5173a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5173a-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5173a-121">Optional query parameters</span></span>
<span data-ttu-id="5173a-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5173a-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5173a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5173a-123">Request headers</span></span>
| <span data-ttu-id="5173a-124">标头</span><span class="sxs-lookup"><span data-stu-id="5173a-124">Header</span></span>       | <span data-ttu-id="5173a-125">值</span><span class="sxs-lookup"><span data-stu-id="5173a-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5173a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5173a-126">Authorization</span></span>  | <span data-ttu-id="5173a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5173a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5173a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5173a-129">Request body</span></span>
<span data-ttu-id="5173a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5173a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5173a-131">响应</span><span class="sxs-lookup"><span data-stu-id="5173a-131">Response</span></span>

<span data-ttu-id="5173a-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [post](../resources/post.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5173a-132">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5173a-133">示例</span><span class="sxs-lookup"><span data-stu-id="5173a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5173a-134">请求</span><span class="sxs-lookup"><span data-stu-id="5173a-134">Request</span></span>
<span data-ttu-id="5173a-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5173a-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5173a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5173a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts/AQMkADgAAAIJbQAAAA==
```
# <a name="c"></a>[<span data-ttu-id="5173a-137">C#</span><span class="sxs-lookup"><span data-stu-id="5173a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5173a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5173a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5173a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5173a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5173a-140">Java</span><span class="sxs-lookup"><span data-stu-id="5173a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5173a-141">响应</span><span class="sxs-lookup"><span data-stu-id="5173a-141">Response</span></span>
<span data-ttu-id="5173a-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5173a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts/$entity",
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
```

## <a name="see-also"></a><span data-ttu-id="5173a-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5173a-145">See also</span></span>

- [<span data-ttu-id="5173a-146">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="5173a-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5173a-147">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="5173a-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="5173a-148">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="5173a-148">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
