---
title: call： keepAlive
description: 每15至45分钟向此 API 发出一次请求，以确保正在进行的呼叫保持活动状态。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 37af131e5e51f1bb0388bc002465aef71a8059a0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518712"
---
# <a name="call-keepalive"></a><span data-ttu-id="f1bd3-103">call： keepAlive</span><span class="sxs-lookup"><span data-stu-id="f1bd3-103">call: keepAlive</span></span>

<span data-ttu-id="f1bd3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1bd3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1bd3-105">每15至45分钟向此 API 发出一次请求，以确保正在进行的呼叫仍处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="f1bd3-105">Make a request to this API every 15 to 45 minutes to ensure that an ongoing call remains active.</span></span> <span data-ttu-id="f1bd3-106">在45分钟内未收到此请求的呼叫被视为非活动状态，随后将结束。</span><span class="sxs-lookup"><span data-stu-id="f1bd3-106">A call that does not receive this request within 45 minutes is considered inactive and will subsequently end.</span></span>

<span data-ttu-id="f1bd3-107">必须在前一个请求的45分钟内或开始呼叫开始时至少执行一次成功的请求。</span><span class="sxs-lookup"><span data-stu-id="f1bd3-107">At least one successful request must be made within 45 minutes of the previous request, or the start of the call.</span></span>

<span data-ttu-id="f1bd3-108">我们建议您以较短的时间间隔（每15分钟）发送请求。</span><span class="sxs-lookup"><span data-stu-id="f1bd3-108">We recommend that you send a request in shorter time intervals (every 15 minutes).</span></span> <span data-ttu-id="f1bd3-109">确保这些请求成功，以阻止调用超时和结束。</span><span class="sxs-lookup"><span data-stu-id="f1bd3-109">Make sure that these requests are successful to prevent the call from timing out and ending.</span></span>

<span data-ttu-id="f1bd3-110">尝试向已结束的呼叫发送请求将导致`404 Not-Found`错误。</span><span class="sxs-lookup"><span data-stu-id="f1bd3-110">Attempting to send a request to a call that has already ended will result in a `404 Not-Found` error.</span></span> <span data-ttu-id="f1bd3-111">应在应用程序一侧清理与此呼叫相关的资源。</span><span class="sxs-lookup"><span data-stu-id="f1bd3-111">The resources related to the call should be cleaned up on the application side.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1bd3-112">权限</span><span class="sxs-lookup"><span data-stu-id="f1bd3-112">Permissions</span></span>
<span data-ttu-id="f1bd3-113">若要调用此 API，可能需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="f1bd3-113">One of the following permissions may be required to call this API.</span></span> <span data-ttu-id="f1bd3-114">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1bd3-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1bd3-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1bd3-115">Permission type</span></span> | <span data-ttu-id="f1bd3-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1bd3-116">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="f1bd3-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1bd3-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1bd3-118">不支持</span><span class="sxs-lookup"><span data-stu-id="f1bd3-118">Not Supported</span></span>        |
| <span data-ttu-id="f1bd3-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1bd3-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1bd3-120">不支持</span><span class="sxs-lookup"><span data-stu-id="f1bd3-120">Not Supported</span></span>        |
| <span data-ttu-id="f1bd3-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1bd3-121">Application</span></span>     | <span data-ttu-id="f1bd3-122">无</span><span class="sxs-lookup"><span data-stu-id="f1bd3-122">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="f1bd3-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1bd3-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/keepAlive
```


## <a name="request-headers"></a><span data-ttu-id="f1bd3-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1bd3-124">Request headers</span></span>
| <span data-ttu-id="f1bd3-125">名称</span><span class="sxs-lookup"><span data-stu-id="f1bd3-125">Name</span></span>          | <span data-ttu-id="f1bd3-126">说明</span><span class="sxs-lookup"><span data-stu-id="f1bd3-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f1bd3-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1bd3-127">Authorization</span></span> | <span data-ttu-id="f1bd3-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f1bd3-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1bd3-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1bd3-130">Request body</span></span>
<span data-ttu-id="f1bd3-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f1bd3-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1bd3-132">响应</span><span class="sxs-lookup"><span data-stu-id="f1bd3-132">Response</span></span>
<span data-ttu-id="f1bd3-133">此方法返回`200 OK`响应代码。</span><span class="sxs-lookup"><span data-stu-id="f1bd3-133">This method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f1bd3-134">示例</span><span class="sxs-lookup"><span data-stu-id="f1bd3-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1bd3-135">请求</span><span class="sxs-lookup"><span data-stu-id="f1bd3-135">Request</span></span>
<span data-ttu-id="f1bd3-136">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="f1bd3-136">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1bd3-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1bd3-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "keep-alive"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive
```
# <a name="c"></a>[<span data-ttu-id="f1bd3-138">C#</span><span class="sxs-lookup"><span data-stu-id="f1bd3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/keep-alive-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1bd3-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1bd3-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/keep-alive-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1bd3-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1bd3-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/keep-alive-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1bd3-141">Java</span><span class="sxs-lookup"><span data-stu-id="f1bd3-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/keep-alive-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f1bd3-142">响应</span><span class="sxs-lookup"><span data-stu-id="f1bd3-142">Response</span></span>
<span data-ttu-id="f1bd3-143">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="f1bd3-143">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "keep-alive",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 200 OK
```


<!--
{
  "type": "#page.annotation",
  "description": "call: keepAlive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
