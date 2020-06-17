---
title: 获取 conversationThread
description: '获取属于某个组的特定线程。 您可以同时指定父对话和线程，或者 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 56a49586fcab45f325441593137e578ae0a3145a
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2020
ms.locfileid: "44743790"
---
# <a name="get-conversationthread"></a><span data-ttu-id="91de7-104">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="91de7-104">Get conversationThread</span></span>

<span data-ttu-id="91de7-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91de7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="91de7-106">Get a specific thread that belongs to a group.</span><span class="sxs-lookup"><span data-stu-id="91de7-106">Get a specific thread that belongs to a group.</span></span> <span data-ttu-id="91de7-107">You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span><span class="sxs-lookup"><span data-stu-id="91de7-107">You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="91de7-108">权限</span><span class="sxs-lookup"><span data-stu-id="91de7-108">Permissions</span></span>
<span data-ttu-id="91de7-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="91de7-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="91de7-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91de7-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91de7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="91de7-111">Permission type</span></span>      | <span data-ttu-id="91de7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91de7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91de7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91de7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="91de7-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91de7-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="91de7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91de7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91de7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="91de7-116">Not supported.</span></span>    |
|<span data-ttu-id="91de7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="91de7-117">Application</span></span> | <span data-ttu-id="91de7-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91de7-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91de7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91de7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="91de7-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="91de7-120">Optional query parameters</span></span>
<span data-ttu-id="91de7-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="91de7-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="91de7-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="91de7-122">Request headers</span></span>
| <span data-ttu-id="91de7-123">标头</span><span class="sxs-lookup"><span data-stu-id="91de7-123">Header</span></span>       | <span data-ttu-id="91de7-124">值</span><span class="sxs-lookup"><span data-stu-id="91de7-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91de7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="91de7-125">Authorization</span></span>  | <span data-ttu-id="91de7-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="91de7-126">Bearer {token}.</span></span> <span data-ttu-id="91de7-127">Required.</span><span class="sxs-lookup"><span data-stu-id="91de7-127">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91de7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="91de7-128">Request body</span></span>
<span data-ttu-id="91de7-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="91de7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91de7-130">响应</span><span class="sxs-lookup"><span data-stu-id="91de7-130">Response</span></span>

<span data-ttu-id="91de7-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="91de7-131">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91de7-132">示例</span><span class="sxs-lookup"><span data-stu-id="91de7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91de7-133">请求</span><span class="sxs-lookup"><span data-stu-id="91de7-133">Request</span></span>
<span data-ttu-id="91de7-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="91de7-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91de7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="91de7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
# <a name="c"></a>[<span data-ttu-id="91de7-136">C#</span><span class="sxs-lookup"><span data-stu-id="91de7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91de7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91de7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91de7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91de7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91de7-139">Java</span><span class="sxs-lookup"><span data-stu-id="91de7-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversationthread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="91de7-140">响应</span><span class="sxs-lookup"><span data-stu-id="91de7-140">Response</span></span>
<span data-ttu-id="91de7-141">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="91de7-141">Here is an example of the response.</span></span> <span data-ttu-id="91de7-142">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="91de7-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="91de7-143">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="91de7-143">All of the properties will be returned from an actual call.</span></span>
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
