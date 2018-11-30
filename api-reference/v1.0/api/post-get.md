---
title: 获取帖子
description: '获取指定的线程中帖子的属性和关系。 您可以指定父 '
ms.openlocfilehash: d9f697ac45bf0a817334bdcfd46febc74f10e107
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007712"
---
# <a name="get-post"></a><span data-ttu-id="eb3c3-104">获取帖子</span><span class="sxs-lookup"><span data-stu-id="eb3c3-104">Get post</span></span>

<span data-ttu-id="eb3c3-p102">获取指定线程中的帖子的属性和关系。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="eb3c3-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="eb3c3-107">由于**帖子**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**帖子**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="eb3c3-107">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb3c3-108">权限</span><span class="sxs-lookup"><span data-stu-id="eb3c3-108">Permissions</span></span>
<span data-ttu-id="eb3c3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb3c3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb3c3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb3c3-111">Permission type</span></span>      | <span data-ttu-id="eb3c3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb3c3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb3c3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb3c3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="eb3c3-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb3c3-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb3c3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb3c3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb3c3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb3c3-116">Not supported.</span></span>    |
|<span data-ttu-id="eb3c3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb3c3-117">Application</span></span> | <span data-ttu-id="eb3c3-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb3c3-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb3c3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb3c3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eb3c3-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="eb3c3-120">Optional query parameters</span></span>
<span data-ttu-id="eb3c3-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="eb3c3-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="eb3c3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb3c3-122">Request headers</span></span>
| <span data-ttu-id="eb3c3-123">标头</span><span class="sxs-lookup"><span data-stu-id="eb3c3-123">Header</span></span>       | <span data-ttu-id="eb3c3-124">值</span><span class="sxs-lookup"><span data-stu-id="eb3c3-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eb3c3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb3c3-125">Authorization</span></span>  | <span data-ttu-id="eb3c3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb3c3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eb3c3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb3c3-128">Request body</span></span>
<span data-ttu-id="eb3c3-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eb3c3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb3c3-130">响应</span><span class="sxs-lookup"><span data-stu-id="eb3c3-130">Response</span></span>

<span data-ttu-id="eb3c3-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [post](../resources/post.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb3c3-131">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eb3c3-132">示例</span><span class="sxs-lookup"><span data-stu-id="eb3c3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb3c3-133">请求</span><span class="sxs-lookup"><span data-stu-id="eb3c3-133">Request</span></span>
<span data-ttu-id="eb3c3-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb3c3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
##### <a name="response"></a><span data-ttu-id="eb3c3-135">响应</span><span class="sxs-lookup"><span data-stu-id="eb3c3-135">Response</span></span>
<span data-ttu-id="eb3c3-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eb3c3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="eb3c3-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="eb3c3-139">See also</span></span>

- [<span data-ttu-id="eb3c3-140">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="eb3c3-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="eb3c3-141">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="eb3c3-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
  "tocPath": ""
}-->
