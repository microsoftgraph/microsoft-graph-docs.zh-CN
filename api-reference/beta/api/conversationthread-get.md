---
title: 获取 conversationThread
description: '获取属于某个组的特定线程。 您可以指定父对话和线程，或， '
ms.openlocfilehash: b9a99be2e44b7639fe9a44b475bdf0161efa303c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042616"
---
# <a name="get-conversationthread"></a><span data-ttu-id="bd6e1-104">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="bd6e1-104">Get conversationThread</span></span>

> <span data-ttu-id="bd6e1-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bd6e1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd6e1-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bd6e1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd6e1-p103">获取属于某个组的特定线程。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="bd6e1-p103">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="bd6e1-109">权限</span><span class="sxs-lookup"><span data-stu-id="bd6e1-109">Permissions</span></span>
<span data-ttu-id="bd6e1-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd6e1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd6e1-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd6e1-112">Permission type</span></span>      | <span data-ttu-id="bd6e1-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd6e1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd6e1-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd6e1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bd6e1-115">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd6e1-115">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="bd6e1-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd6e1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd6e1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd6e1-117">Not supported.</span></span>    |
|<span data-ttu-id="bd6e1-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd6e1-118">Application</span></span> | <span data-ttu-id="bd6e1-119">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd6e1-119">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd6e1-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd6e1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="bd6e1-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bd6e1-121">Optional query parameters</span></span>
<span data-ttu-id="bd6e1-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bd6e1-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bd6e1-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd6e1-123">Request headers</span></span>
| <span data-ttu-id="bd6e1-124">标头</span><span class="sxs-lookup"><span data-stu-id="bd6e1-124">Header</span></span>       | <span data-ttu-id="bd6e1-125">值</span><span class="sxs-lookup"><span data-stu-id="bd6e1-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bd6e1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd6e1-126">Authorization</span></span>  | <span data-ttu-id="bd6e1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bd6e1-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bd6e1-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd6e1-129">Request body</span></span>
<span data-ttu-id="bd6e1-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd6e1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd6e1-131">响应</span><span class="sxs-lookup"><span data-stu-id="bd6e1-131">Response</span></span>

<span data-ttu-id="bd6e1-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bd6e1-132">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bd6e1-133">示例</span><span class="sxs-lookup"><span data-stu-id="bd6e1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd6e1-134">请求</span><span class="sxs-lookup"><span data-stu-id="bd6e1-134">Request</span></span>
<span data-ttu-id="bd6e1-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd6e1-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="bd6e1-136">响应</span><span class="sxs-lookup"><span data-stu-id="bd6e1-136">Response</span></span>
<span data-ttu-id="bd6e1-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd6e1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
