---
title: 获取帖子
description: '获取指定的线程中帖子的属性和关系。 您可以同时指定父 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 8e724a664e708503daf5b30afdec04cccbb2fee4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576302"
---
# <a name="get-post"></a><span data-ttu-id="54d46-104">获取帖子</span><span class="sxs-lookup"><span data-stu-id="54d46-104">Get post</span></span>

<span data-ttu-id="54d46-p102">获取指定线程中的帖子的属性和关系。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="54d46-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="54d46-107">由于**帖子**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**帖子**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="54d46-107">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="54d46-108">权限</span><span class="sxs-lookup"><span data-stu-id="54d46-108">Permissions</span></span>
<span data-ttu-id="54d46-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54d46-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54d46-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="54d46-111">Permission type</span></span>      | <span data-ttu-id="54d46-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54d46-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54d46-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54d46-113">Delegated (work or school account)</span></span> | <span data-ttu-id="54d46-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54d46-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="54d46-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54d46-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54d46-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="54d46-116">Not supported.</span></span>    |
|<span data-ttu-id="54d46-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="54d46-117">Application</span></span> | <span data-ttu-id="54d46-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54d46-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54d46-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54d46-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="54d46-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="54d46-120">Optional query parameters</span></span>
<span data-ttu-id="54d46-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="54d46-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="54d46-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="54d46-122">Request headers</span></span>
| <span data-ttu-id="54d46-123">标头</span><span class="sxs-lookup"><span data-stu-id="54d46-123">Header</span></span>       | <span data-ttu-id="54d46-124">值</span><span class="sxs-lookup"><span data-stu-id="54d46-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="54d46-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="54d46-125">Authorization</span></span>  | <span data-ttu-id="54d46-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="54d46-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="54d46-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="54d46-128">Request body</span></span>
<span data-ttu-id="54d46-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="54d46-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54d46-130">响应</span><span class="sxs-lookup"><span data-stu-id="54d46-130">Response</span></span>

<span data-ttu-id="54d46-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [post](../resources/post.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="54d46-131">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="54d46-132">示例</span><span class="sxs-lookup"><span data-stu-id="54d46-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54d46-133">请求</span><span class="sxs-lookup"><span data-stu-id="54d46-133">Request</span></span>
<span data-ttu-id="54d46-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="54d46-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
##### <a name="response"></a><span data-ttu-id="54d46-135">响应</span><span class="sxs-lookup"><span data-stu-id="54d46-135">Response</span></span>
<span data-ttu-id="54d46-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="54d46-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="54d46-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="54d46-139">See also</span></span>

- [<span data-ttu-id="54d46-140">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="54d46-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="54d46-141">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="54d46-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
