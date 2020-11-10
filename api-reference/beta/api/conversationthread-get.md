---
title: 获取 conversationThread
description: '获取属于某个组的特定线程。 您可以同时指定父对话和线程，或者 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0a11148e2844be0bae93c86df0300b01d42322bf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956658"
---
# <a name="get-conversationthread"></a><span data-ttu-id="75f82-104">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="75f82-104">Get conversationThread</span></span>

<span data-ttu-id="75f82-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75f82-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75f82-p102">获取属于某个组的特定线程。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="75f82-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="75f82-108">权限</span><span class="sxs-lookup"><span data-stu-id="75f82-108">Permissions</span></span>
<span data-ttu-id="75f82-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75f82-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75f82-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="75f82-111">Permission type</span></span>      | <span data-ttu-id="75f82-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75f82-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75f82-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75f82-113">Delegated (work or school account)</span></span> | <span data-ttu-id="75f82-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75f82-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="75f82-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75f82-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75f82-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="75f82-116">Not supported.</span></span>    |
|<span data-ttu-id="75f82-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="75f82-117">Application</span></span> | <span data-ttu-id="75f82-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75f82-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75f82-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75f82-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="75f82-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="75f82-120">Optional query parameters</span></span>
<span data-ttu-id="75f82-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="75f82-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="75f82-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="75f82-122">Request headers</span></span>
| <span data-ttu-id="75f82-123">标头</span><span class="sxs-lookup"><span data-stu-id="75f82-123">Header</span></span>       | <span data-ttu-id="75f82-124">值</span><span class="sxs-lookup"><span data-stu-id="75f82-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="75f82-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="75f82-125">Authorization</span></span>  | <span data-ttu-id="75f82-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75f82-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75f82-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="75f82-128">Request body</span></span>
<span data-ttu-id="75f82-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="75f82-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75f82-130">响应</span><span class="sxs-lookup"><span data-stu-id="75f82-130">Response</span></span>

<span data-ttu-id="75f82-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="75f82-131">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="75f82-132">示例</span><span class="sxs-lookup"><span data-stu-id="75f82-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75f82-133">请求</span><span class="sxs-lookup"><span data-stu-id="75f82-133">Request</span></span>
<span data-ttu-id="75f82-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75f82-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="75f82-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="75f82-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
# <a name="c"></a>[<span data-ttu-id="75f82-136">C#</span><span class="sxs-lookup"><span data-stu-id="75f82-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75f82-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75f82-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75f82-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75f82-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75f82-139">Java</span><span class="sxs-lookup"><span data-stu-id="75f82-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversationthread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="75f82-140">响应</span><span class="sxs-lookup"><span data-stu-id="75f82-140">Response</span></span>
<span data-ttu-id="75f82-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="75f82-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
