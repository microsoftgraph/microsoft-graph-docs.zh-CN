---
title: 'synchronizationJob: pause'
description: 临时停止同步。 所有进度 (包括作业状态) 均保持不变, 作业将从开始调用时停止的位置继续。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6af366251f54c9964d4bedf41286ed15aef34297
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363534"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="ac53b-104">synchronizationJob: pause</span><span class="sxs-lookup"><span data-stu-id="ac53b-104">synchronizationJob: pause</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac53b-105">临时停止同步。</span><span class="sxs-lookup"><span data-stu-id="ac53b-105">Temporarily stop synchronization.</span></span> <span data-ttu-id="ac53b-106">所有进度 (包括作业状态) 均保持不变, 作业将从[开始](../api/synchronization-synchronizationjob-start.md)调用时停止的位置继续。</span><span class="sxs-lookup"><span data-stu-id="ac53b-106">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac53b-107">权限</span><span class="sxs-lookup"><span data-stu-id="ac53b-107">Permissions</span></span>
<span data-ttu-id="ac53b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac53b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac53b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac53b-110">Permission type</span></span>                        | <span data-ttu-id="ac53b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac53b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac53b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac53b-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="ac53b-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac53b-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ac53b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac53b-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ac53b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac53b-115">Not supported.</span></span>  |
|<span data-ttu-id="ac53b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac53b-116">Application</span></span>                            |<span data-ttu-id="ac53b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac53b-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ac53b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac53b-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="ac53b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac53b-119">Request headers</span></span>

| <span data-ttu-id="ac53b-120">名称</span><span class="sxs-lookup"><span data-stu-id="ac53b-120">Name</span></span>           | <span data-ttu-id="ac53b-121">类型</span><span class="sxs-lookup"><span data-stu-id="ac53b-121">Type</span></span>    | <span data-ttu-id="ac53b-122">说明</span><span class="sxs-lookup"><span data-stu-id="ac53b-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ac53b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac53b-123">Authorization</span></span>  | <span data-ttu-id="ac53b-124">string</span><span class="sxs-lookup"><span data-stu-id="ac53b-124">string</span></span>  | <span data-ttu-id="ac53b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac53b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac53b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac53b-127">Request body</span></span>

<span data-ttu-id="ac53b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ac53b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac53b-129">响应</span><span class="sxs-lookup"><span data-stu-id="ac53b-129">Response</span></span>

<span data-ttu-id="ac53b-130">如果成功, 则返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="ac53b-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="ac53b-131">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ac53b-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac53b-132">示例</span><span class="sxs-lookup"><span data-stu-id="ac53b-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ac53b-133">请求</span><span class="sxs-lookup"><span data-stu-id="ac53b-133">Request</span></span>
<span data-ttu-id="ac53b-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="ac53b-134">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ac53b-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ac53b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ac53b-136">C#</span><span class="sxs-lookup"><span data-stu-id="ac53b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ac53b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac53b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ac53b-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="ac53b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ac53b-139">Java</span><span class="sxs-lookup"><span data-stu-id="ac53b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-pause-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ac53b-140">响应</span><span class="sxs-lookup"><span data-stu-id="ac53b-140">Response</span></span>
<span data-ttu-id="ac53b-141">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="ac53b-141">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: pause",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
