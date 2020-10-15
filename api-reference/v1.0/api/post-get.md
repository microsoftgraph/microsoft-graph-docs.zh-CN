---
title: 获取帖子
description: '获取指定的线程中帖子的属性和关系。 您可以同时指定父 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2ce4db0e0cf4b17245ad7ad0e84a45e4152d567f
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458323"
---
# <a name="get-post"></a><span data-ttu-id="e73f4-104">获取帖子</span><span class="sxs-lookup"><span data-stu-id="e73f4-104">Get post</span></span>

<span data-ttu-id="e73f4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e73f4-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e73f4-p102">获取指定线程中的帖子的属性和关系。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="e73f4-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="e73f4-108">由于**帖子**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**帖子**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="e73f4-108">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="e73f4-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="e73f4-109">Permissions</span></span>
<span data-ttu-id="e73f4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e73f4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e73f4-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e73f4-112">Permission type</span></span>      | <span data-ttu-id="e73f4-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e73f4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e73f4-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e73f4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e73f4-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e73f4-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e73f4-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e73f4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e73f4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e73f4-117">Not supported.</span></span>    |
|<span data-ttu-id="e73f4-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e73f4-118">Application</span></span> | <span data-ttu-id="e73f4-119">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e73f4-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e73f4-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e73f4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e73f4-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e73f4-121">Optional query parameters</span></span>
<span data-ttu-id="e73f4-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e73f4-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e73f4-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e73f4-123">Request headers</span></span>
| <span data-ttu-id="e73f4-124">标头</span><span class="sxs-lookup"><span data-stu-id="e73f4-124">Header</span></span>       | <span data-ttu-id="e73f4-125">值</span><span class="sxs-lookup"><span data-stu-id="e73f4-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e73f4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e73f4-126">Authorization</span></span>  | <span data-ttu-id="e73f4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e73f4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e73f4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e73f4-129">Request body</span></span>
<span data-ttu-id="e73f4-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e73f4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e73f4-131">响应</span><span class="sxs-lookup"><span data-stu-id="e73f4-131">Response</span></span>

<span data-ttu-id="e73f4-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [post](../resources/post.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e73f4-132">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e73f4-133">示例</span><span class="sxs-lookup"><span data-stu-id="e73f4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e73f4-134">请求</span><span class="sxs-lookup"><span data-stu-id="e73f4-134">Request</span></span>
<span data-ttu-id="e73f4-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e73f4-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e73f4-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e73f4-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
# <a name="c"></a>[<span data-ttu-id="e73f4-137">C#</span><span class="sxs-lookup"><span data-stu-id="e73f4-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e73f4-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e73f4-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e73f4-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e73f4-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e73f4-140">Java</span><span class="sxs-lookup"><span data-stu-id="e73f4-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e73f4-141">响应</span><span class="sxs-lookup"><span data-stu-id="e73f4-141">Response</span></span>
<span data-ttu-id="e73f4-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e73f4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 414

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
  }
}
```

## <a name="see-also"></a><span data-ttu-id="e73f4-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e73f4-145">See also</span></span>

- [<span data-ttu-id="e73f4-146">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e73f4-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e73f4-147">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="e73f4-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
