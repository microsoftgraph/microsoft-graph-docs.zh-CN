---
title: 列出帖子
description: '获取指定线程的帖子。 您可以指定父对话和线程，或， '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: aa411939f9e8040b127a8821c23b557defffbaec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961517"
---
# <a name="list-posts"></a><span data-ttu-id="03cae-104">列出帖子</span><span class="sxs-lookup"><span data-stu-id="03cae-104">List posts</span></span>

<span data-ttu-id="03cae-p102">获取指定线程的帖子。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="03cae-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="03cae-107">权限</span><span class="sxs-lookup"><span data-stu-id="03cae-107">Permissions</span></span>
<span data-ttu-id="03cae-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03cae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03cae-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="03cae-110">Permission type</span></span>      | <span data-ttu-id="03cae-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03cae-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03cae-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03cae-112">Delegated (work or school account)</span></span> | <span data-ttu-id="03cae-113">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="03cae-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="03cae-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03cae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03cae-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="03cae-115">Not supported.</span></span>    |
|<span data-ttu-id="03cae-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="03cae-116">Application</span></span> | <span data-ttu-id="03cae-117">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="03cae-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03cae-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03cae-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="03cae-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="03cae-119">Optional query parameters</span></span>
<span data-ttu-id="03cae-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="03cae-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="03cae-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="03cae-121">Request headers</span></span>
| <span data-ttu-id="03cae-122">标头</span><span class="sxs-lookup"><span data-stu-id="03cae-122">Header</span></span>       | <span data-ttu-id="03cae-123">值</span><span class="sxs-lookup"><span data-stu-id="03cae-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="03cae-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="03cae-124">Authorization</span></span>  | <span data-ttu-id="03cae-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="03cae-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="03cae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="03cae-127">Request body</span></span>
<span data-ttu-id="03cae-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="03cae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03cae-129">响应</span><span class="sxs-lookup"><span data-stu-id="03cae-129">Response</span></span>

<span data-ttu-id="03cae-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Post](../resources/post.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="03cae-130">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="03cae-131">示例</span><span class="sxs-lookup"><span data-stu-id="03cae-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03cae-132">请求</span><span class="sxs-lookup"><span data-stu-id="03cae-132">Request</span></span>
<span data-ttu-id="03cae-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03cae-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
##### <a name="response"></a><span data-ttu-id="03cae-134">响应</span><span class="sxs-lookup"><span data-stu-id="03cae-134">Response</span></span>
<span data-ttu-id="03cae-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03cae-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
