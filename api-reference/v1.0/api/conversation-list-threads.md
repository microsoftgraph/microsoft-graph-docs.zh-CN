---
title: 列出线程
description: 获取组对话中的所有线程。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 69d1179dc74b275f8f9cf74b515ff2ebf9dc5349
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2020
ms.locfileid: "44743779"
---
# <a name="list-threads"></a><span data-ttu-id="93f46-103">列出线程</span><span class="sxs-lookup"><span data-stu-id="93f46-103">List threads</span></span>

<span data-ttu-id="93f46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93f46-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93f46-105">获取组对话中的所有线程。</span><span class="sxs-lookup"><span data-stu-id="93f46-105">Get all the threads in a group conversation.</span></span>

<span data-ttu-id="93f46-106">注意：还可以 [获取组的所有线程](group-list-threads.md)。</span><span class="sxs-lookup"><span data-stu-id="93f46-106">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="93f46-107">权限</span><span class="sxs-lookup"><span data-stu-id="93f46-107">Permissions</span></span>
<span data-ttu-id="93f46-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="93f46-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="93f46-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93f46-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93f46-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="93f46-110">Permission type</span></span>      | <span data-ttu-id="93f46-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="93f46-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93f46-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93f46-112">Delegated (work or school account)</span></span> | <span data-ttu-id="93f46-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93f46-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="93f46-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93f46-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93f46-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="93f46-115">Not supported.</span></span>    |
|<span data-ttu-id="93f46-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="93f46-116">Application</span></span> | <span data-ttu-id="93f46-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93f46-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93f46-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93f46-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="93f46-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="93f46-119">Optional query parameters</span></span>
<span data-ttu-id="93f46-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="93f46-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="93f46-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="93f46-121">Request headers</span></span>
| <span data-ttu-id="93f46-122">标头</span><span class="sxs-lookup"><span data-stu-id="93f46-122">Header</span></span>       | <span data-ttu-id="93f46-123">值</span><span class="sxs-lookup"><span data-stu-id="93f46-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93f46-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="93f46-124">Authorization</span></span>  | <span data-ttu-id="93f46-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="93f46-125">Bearer {token}.</span></span> <span data-ttu-id="93f46-126">Required.</span><span class="sxs-lookup"><span data-stu-id="93f46-126">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93f46-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="93f46-127">Request body</span></span>
<span data-ttu-id="93f46-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="93f46-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93f46-129">响应</span><span class="sxs-lookup"><span data-stu-id="93f46-129">Response</span></span>

<span data-ttu-id="93f46-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="93f46-130">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93f46-131">示例</span><span class="sxs-lookup"><span data-stu-id="93f46-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93f46-132">请求</span><span class="sxs-lookup"><span data-stu-id="93f46-132">Request</span></span>
<span data-ttu-id="93f46-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="93f46-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93f46-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="93f46-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
```
# <a name="c"></a>[<span data-ttu-id="93f46-135">C#</span><span class="sxs-lookup"><span data-stu-id="93f46-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93f46-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93f46-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93f46-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93f46-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93f46-138">Java</span><span class="sxs-lookup"><span data-stu-id="93f46-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threads-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="93f46-139">响应</span><span class="sxs-lookup"><span data-stu-id="93f46-139">Response</span></span>
<span data-ttu-id="93f46-140">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="93f46-140">Here is an example of the response.</span></span> <span data-ttu-id="93f46-141">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="93f46-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="93f46-142">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="93f46-142">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
