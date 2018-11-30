---
title: 获取 conversationThread
description: '获取属于某个组的特定线程。 您可以指定父对话和线程，或， '
ms.openlocfilehash: 1c4e0da5a85464c07844c976140425a70fd48b76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009303"
---
# <a name="get-conversationthread"></a><span data-ttu-id="28869-104">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="28869-104">Get conversationThread</span></span>

<span data-ttu-id="28869-p102">获取属于某个组的特定线程。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="28869-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="28869-107">权限</span><span class="sxs-lookup"><span data-stu-id="28869-107">Permissions</span></span>
<span data-ttu-id="28869-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28869-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28869-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="28869-110">Permission type</span></span>      | <span data-ttu-id="28869-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28869-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28869-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28869-112">Delegated (work or school account)</span></span> | <span data-ttu-id="28869-113">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="28869-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="28869-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28869-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28869-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="28869-115">Not supported.</span></span>    |
|<span data-ttu-id="28869-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="28869-116">Application</span></span> | <span data-ttu-id="28869-117">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="28869-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28869-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28869-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="28869-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="28869-119">Optional query parameters</span></span>
<span data-ttu-id="28869-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="28869-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="28869-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="28869-121">Request headers</span></span>
| <span data-ttu-id="28869-122">标头</span><span class="sxs-lookup"><span data-stu-id="28869-122">Header</span></span>       | <span data-ttu-id="28869-123">值</span><span class="sxs-lookup"><span data-stu-id="28869-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="28869-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="28869-124">Authorization</span></span>  | <span data-ttu-id="28869-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="28869-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="28869-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="28869-127">Request body</span></span>
<span data-ttu-id="28869-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="28869-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28869-129">响应</span><span class="sxs-lookup"><span data-stu-id="28869-129">Response</span></span>

<span data-ttu-id="28869-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="28869-130">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="28869-131">示例</span><span class="sxs-lookup"><span data-stu-id="28869-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28869-132">请求</span><span class="sxs-lookup"><span data-stu-id="28869-132">Request</span></span>
<span data-ttu-id="28869-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="28869-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="28869-134">响应</span><span class="sxs-lookup"><span data-stu-id="28869-134">Response</span></span>
<span data-ttu-id="28869-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="28869-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
