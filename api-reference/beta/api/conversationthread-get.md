---
title: 获取 conversationThread
description: '获取属于某个组的特定线程。 您可以同时指定父对话和线程, 或者 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: e78629921a9c3d596ea7f9bdbe8b9948e4fc74cb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437401"
---
# <a name="get-conversationthread"></a><span data-ttu-id="9b9cf-104">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="9b9cf-104">Get conversationThread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b9cf-p102">获取属于某个组的特定线程。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="9b9cf-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="9b9cf-107">权限</span><span class="sxs-lookup"><span data-stu-id="9b9cf-107">Permissions</span></span>
<span data-ttu-id="9b9cf-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b9cf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b9cf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b9cf-110">Permission type</span></span>      | <span data-ttu-id="9b9cf-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b9cf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b9cf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b9cf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9b9cf-113">Group. 全部, Group。 Read. All</span><span class="sxs-lookup"><span data-stu-id="9b9cf-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="9b9cf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b9cf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b9cf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b9cf-115">Not supported.</span></span>    |
|<span data-ttu-id="9b9cf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b9cf-116">Application</span></span> | <span data-ttu-id="9b9cf-117">Group. 全部, Group。 Read. All</span><span class="sxs-lookup"><span data-stu-id="9b9cf-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b9cf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b9cf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="9b9cf-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9b9cf-119">Optional query parameters</span></span>
<span data-ttu-id="9b9cf-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9b9cf-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9b9cf-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b9cf-121">Request headers</span></span>
| <span data-ttu-id="9b9cf-122">标头</span><span class="sxs-lookup"><span data-stu-id="9b9cf-122">Header</span></span>       | <span data-ttu-id="9b9cf-123">值</span><span class="sxs-lookup"><span data-stu-id="9b9cf-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9b9cf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b9cf-124">Authorization</span></span>  | <span data-ttu-id="9b9cf-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b9cf-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9b9cf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b9cf-127">Request body</span></span>
<span data-ttu-id="9b9cf-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9b9cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b9cf-129">响应</span><span class="sxs-lookup"><span data-stu-id="9b9cf-129">Response</span></span>

<span data-ttu-id="9b9cf-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9b9cf-130">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9b9cf-131">示例</span><span class="sxs-lookup"><span data-stu-id="9b9cf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b9cf-132">请求</span><span class="sxs-lookup"><span data-stu-id="9b9cf-132">Request</span></span>
<span data-ttu-id="9b9cf-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9b9cf-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9b9cf-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9b9cf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9b9cf-135">C#</span><span class="sxs-lookup"><span data-stu-id="9b9cf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b9cf-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="9b9cf-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9b9cf-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="9b9cf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9b9cf-138">响应</span><span class="sxs-lookup"><span data-stu-id="9b9cf-138">Response</span></span>
<span data-ttu-id="9b9cf-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9b9cf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
