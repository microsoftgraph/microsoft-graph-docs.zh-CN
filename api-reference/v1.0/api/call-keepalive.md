---
title: call： keepAlive
description: 每15至45分钟向此 API 发出一次请求，以确保正在进行的呼叫保持活动状态。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 32de1b3a24c6b37640376cdf7b60289ced5f90f3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865856"
---
# <a name="call-keepalive"></a><span data-ttu-id="b5726-103">call： keepAlive</span><span class="sxs-lookup"><span data-stu-id="b5726-103">call: keepAlive</span></span>

<span data-ttu-id="b5726-104">每15至45分钟向此 API 发出一次请求，以确保正在进行的呼叫仍处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="b5726-104">Make a request to this API every 15 to 45 minutes to ensure that an ongoing call remains active.</span></span> <span data-ttu-id="b5726-105">在45分钟内未收到此请求的呼叫被视为非活动状态，随后将结束。</span><span class="sxs-lookup"><span data-stu-id="b5726-105">A call that does not receive this request within 45 minutes is considered inactive and will subsequently end.</span></span>

<span data-ttu-id="b5726-106">必须在前一个请求的45分钟内或开始呼叫开始时至少执行一次成功的请求。</span><span class="sxs-lookup"><span data-stu-id="b5726-106">At least one successful request must be made within 45 minutes of the previous request, or the start of the call.</span></span>

<span data-ttu-id="b5726-107">我们建议您以较短的时间间隔（每15分钟）发送请求。</span><span class="sxs-lookup"><span data-stu-id="b5726-107">We recommend that you send a request in shorter time intervals (every 15 minutes).</span></span> <span data-ttu-id="b5726-108">确保这些请求成功，以阻止调用超时和结束。</span><span class="sxs-lookup"><span data-stu-id="b5726-108">Make sure that these requests are successful to prevent the call from timing out and ending.</span></span>

<span data-ttu-id="b5726-109">尝试向已结束的呼叫发送请求将导致`404 Not-Found`错误。</span><span class="sxs-lookup"><span data-stu-id="b5726-109">Attempting to send a request to a call that has already ended will result in a `404 Not-Found` error.</span></span> <span data-ttu-id="b5726-110">应在应用程序一侧清理与此呼叫相关的资源。</span><span class="sxs-lookup"><span data-stu-id="b5726-110">The resources related to the call should be cleaned up on the application side.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5726-111">权限</span><span class="sxs-lookup"><span data-stu-id="b5726-111">Permissions</span></span>
<span data-ttu-id="b5726-112">若要调用此 API，可能需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="b5726-112">One of the following permissions may be required to call this API.</span></span> <span data-ttu-id="b5726-113">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5726-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5726-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5726-114">Permission type</span></span> | <span data-ttu-id="b5726-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5726-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="b5726-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5726-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5726-117">不支持</span><span class="sxs-lookup"><span data-stu-id="b5726-117">Not Supported</span></span>        |
| <span data-ttu-id="b5726-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5726-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5726-119">不支持</span><span class="sxs-lookup"><span data-stu-id="b5726-119">Not Supported</span></span>        |
| <span data-ttu-id="b5726-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5726-120">Application</span></span>     | <span data-ttu-id="b5726-121">无</span><span class="sxs-lookup"><span data-stu-id="b5726-121">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="b5726-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5726-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/keepAlive
```


## <a name="request-headers"></a><span data-ttu-id="b5726-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5726-123">Request headers</span></span>
| <span data-ttu-id="b5726-124">名称</span><span class="sxs-lookup"><span data-stu-id="b5726-124">Name</span></span>          | <span data-ttu-id="b5726-125">说明</span><span class="sxs-lookup"><span data-stu-id="b5726-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b5726-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5726-126">Authorization</span></span> | <span data-ttu-id="b5726-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5726-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5726-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5726-129">Request body</span></span>
<span data-ttu-id="b5726-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5726-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5726-131">响应</span><span class="sxs-lookup"><span data-stu-id="b5726-131">Response</span></span>
<span data-ttu-id="b5726-132">此方法返回`200 OK`响应代码。</span><span class="sxs-lookup"><span data-stu-id="b5726-132">This method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b5726-133">示例</span><span class="sxs-lookup"><span data-stu-id="b5726-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b5726-134">请求</span><span class="sxs-lookup"><span data-stu-id="b5726-134">Request</span></span>
<span data-ttu-id="b5726-135">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="b5726-135">The following example shows a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b5726-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5726-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "keep-alive"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5726-137">C#</span><span class="sxs-lookup"><span data-stu-id="b5726-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/keep-alive-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5726-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5726-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/keep-alive-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5726-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5726-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/keep-alive-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b5726-140">Java</span><span class="sxs-lookup"><span data-stu-id="b5726-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/keep-alive-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b5726-141">响应</span><span class="sxs-lookup"><span data-stu-id="b5726-141">Response</span></span>
<span data-ttu-id="b5726-142">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="b5726-142">The following example shows the response.</span></span>

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
