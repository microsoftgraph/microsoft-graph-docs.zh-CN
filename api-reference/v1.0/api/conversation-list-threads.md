---
title: 列出线程
description: 获取组对话中的所有线程。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 80dceb9cc85d9a9e17761ab8197d94df7b675161
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035657"
---
# <a name="list-threads"></a><span data-ttu-id="4228d-103">列出线程</span><span class="sxs-lookup"><span data-stu-id="4228d-103">List threads</span></span>

<span data-ttu-id="4228d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4228d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4228d-105">获取组对话中的所有线程。</span><span class="sxs-lookup"><span data-stu-id="4228d-105">Get all the threads in a group conversation.</span></span>

<span data-ttu-id="4228d-106">注意：还可以 [获取组的所有线程](group-list-threads.md)。</span><span class="sxs-lookup"><span data-stu-id="4228d-106">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4228d-107">权限</span><span class="sxs-lookup"><span data-stu-id="4228d-107">Permissions</span></span>
<span data-ttu-id="4228d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4228d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4228d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4228d-110">Permission type</span></span>      | <span data-ttu-id="4228d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4228d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4228d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4228d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4228d-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4228d-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4228d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4228d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4228d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4228d-115">Not supported.</span></span>    |
|<span data-ttu-id="4228d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4228d-116">Application</span></span> | <span data-ttu-id="4228d-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4228d-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4228d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4228d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4228d-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4228d-119">Optional query parameters</span></span>
<span data-ttu-id="4228d-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4228d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4228d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4228d-121">Request headers</span></span>
| <span data-ttu-id="4228d-122">标头</span><span class="sxs-lookup"><span data-stu-id="4228d-122">Header</span></span>       | <span data-ttu-id="4228d-123">值</span><span class="sxs-lookup"><span data-stu-id="4228d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4228d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4228d-124">Authorization</span></span>  | <span data-ttu-id="4228d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4228d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4228d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4228d-127">Request body</span></span>
<span data-ttu-id="4228d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4228d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4228d-129">响应</span><span class="sxs-lookup"><span data-stu-id="4228d-129">Response</span></span>

<span data-ttu-id="4228d-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4228d-130">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4228d-131">示例</span><span class="sxs-lookup"><span data-stu-id="4228d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4228d-132">请求</span><span class="sxs-lookup"><span data-stu-id="4228d-132">Request</span></span>
<span data-ttu-id="4228d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4228d-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4228d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4228d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
```
# <a name="c"></a>[<span data-ttu-id="4228d-135">C#</span><span class="sxs-lookup"><span data-stu-id="4228d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4228d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4228d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4228d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4228d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4228d-138">Java</span><span class="sxs-lookup"><span data-stu-id="4228d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threads-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4228d-139">响应</span><span class="sxs-lookup"><span data-stu-id="4228d-139">Response</span></span>
<span data-ttu-id="4228d-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4228d-140">Here is an example of the response.</span></span> <span data-ttu-id="4228d-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4228d-141">Note: The response object shown here might be shortened for readability.</span></span>
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
