---
title: 获取 conversationThread
description: '获取属于某个组的特定线程。 你可以同时指定父会话和线程，或者， '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: da9e54b919a046e826ec892cbeaf210d9add82fb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053235"
---
# <a name="get-conversationthread"></a><span data-ttu-id="8603e-104">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="8603e-104">Get conversationThread</span></span>

<span data-ttu-id="8603e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8603e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8603e-p102">获取属于某个组的特定线程。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="8603e-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="8603e-108">权限</span><span class="sxs-lookup"><span data-stu-id="8603e-108">Permissions</span></span>
<span data-ttu-id="8603e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8603e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8603e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8603e-111">Permission type</span></span>      | <span data-ttu-id="8603e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8603e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8603e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8603e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8603e-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8603e-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8603e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8603e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8603e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8603e-116">Not supported.</span></span>    |
|<span data-ttu-id="8603e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8603e-117">Application</span></span> | <span data-ttu-id="8603e-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8603e-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8603e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8603e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="8603e-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8603e-120">Optional query parameters</span></span>
<span data-ttu-id="8603e-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8603e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8603e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="8603e-122">Request headers</span></span>
| <span data-ttu-id="8603e-123">标头</span><span class="sxs-lookup"><span data-stu-id="8603e-123">Header</span></span>       | <span data-ttu-id="8603e-124">值</span><span class="sxs-lookup"><span data-stu-id="8603e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8603e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8603e-125">Authorization</span></span>  | <span data-ttu-id="8603e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8603e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8603e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8603e-128">Request body</span></span>
<span data-ttu-id="8603e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8603e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8603e-130">响应</span><span class="sxs-lookup"><span data-stu-id="8603e-130">Response</span></span>

<span data-ttu-id="8603e-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8603e-131">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8603e-132">示例</span><span class="sxs-lookup"><span data-stu-id="8603e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8603e-133">请求</span><span class="sxs-lookup"><span data-stu-id="8603e-133">Request</span></span>
<span data-ttu-id="8603e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8603e-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8603e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8603e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
# <a name="c"></a>[<span data-ttu-id="8603e-136">C#</span><span class="sxs-lookup"><span data-stu-id="8603e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8603e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8603e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8603e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8603e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8603e-139">Java</span><span class="sxs-lookup"><span data-stu-id="8603e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversationthread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8603e-140">响应</span><span class="sxs-lookup"><span data-stu-id="8603e-140">Response</span></span>
<span data-ttu-id="8603e-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8603e-141">Here is an example of the response.</span></span> <span data-ttu-id="8603e-142">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8603e-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
