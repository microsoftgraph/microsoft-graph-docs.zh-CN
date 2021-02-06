---
title: synchronizationJob：pause
description: 暂时停止同步。 所有进度（包括作业状态）都将保持，并且作业将在启动调用时从它离开的地方继续。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: eba89e688b8dc9ea02fee633ee4beeb40bb55106
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137485"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="5ffc3-104">synchronizationJob：pause</span><span class="sxs-lookup"><span data-stu-id="5ffc3-104">synchronizationJob: pause</span></span>

<span data-ttu-id="5ffc3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ffc3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ffc3-106">暂时停止同步。</span><span class="sxs-lookup"><span data-stu-id="5ffc3-106">Temporarily stop synchronization.</span></span> <span data-ttu-id="5ffc3-107">所有进度（包括作业状态）都将保持，并且作业将在启动调用时从它离开的地方继续。 [](../api/synchronization-synchronizationjob-start.md)</span><span class="sxs-lookup"><span data-stu-id="5ffc3-107">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ffc3-108">权限</span><span class="sxs-lookup"><span data-stu-id="5ffc3-108">Permissions</span></span>
<span data-ttu-id="5ffc3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ffc3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ffc3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ffc3-111">Permission type</span></span>                        | <span data-ttu-id="5ffc3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ffc3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ffc3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ffc3-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="5ffc3-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ffc3-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="5ffc3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ffc3-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="5ffc3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ffc3-116">Not supported.</span></span>  |
|<span data-ttu-id="5ffc3-117">Application</span><span class="sxs-lookup"><span data-stu-id="5ffc3-117">Application</span></span>                            |<span data-ttu-id="5ffc3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ffc3-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5ffc3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ffc3-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="5ffc3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ffc3-120">Request headers</span></span>

| <span data-ttu-id="5ffc3-121">名称</span><span class="sxs-lookup"><span data-stu-id="5ffc3-121">Name</span></span>           | <span data-ttu-id="5ffc3-122">类型</span><span class="sxs-lookup"><span data-stu-id="5ffc3-122">Type</span></span>    | <span data-ttu-id="5ffc3-123">说明</span><span class="sxs-lookup"><span data-stu-id="5ffc3-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="5ffc3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ffc3-124">Authorization</span></span>  | <span data-ttu-id="5ffc3-125">string</span><span class="sxs-lookup"><span data-stu-id="5ffc3-125">string</span></span>  | <span data-ttu-id="5ffc3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5ffc3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ffc3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ffc3-128">Request body</span></span>

<span data-ttu-id="5ffc3-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5ffc3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ffc3-130">响应</span><span class="sxs-lookup"><span data-stu-id="5ffc3-130">Response</span></span>

<span data-ttu-id="5ffc3-131">如果成功，则返回 `204 No Content` 响应。</span><span class="sxs-lookup"><span data-stu-id="5ffc3-131">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="5ffc3-132">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5ffc3-132">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ffc3-133">示例</span><span class="sxs-lookup"><span data-stu-id="5ffc3-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5ffc3-134">请求</span><span class="sxs-lookup"><span data-stu-id="5ffc3-134">Request</span></span>
<span data-ttu-id="5ffc3-135">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="5ffc3-135">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ffc3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ffc3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```
# <a name="c"></a>[<span data-ttu-id="5ffc3-137">C#</span><span class="sxs-lookup"><span data-stu-id="5ffc3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ffc3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ffc3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ffc3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ffc3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ffc3-140">Java</span><span class="sxs-lookup"><span data-stu-id="5ffc3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-pause-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5ffc3-141">响应</span><span class="sxs-lookup"><span data-stu-id="5ffc3-141">Response</span></span>
<span data-ttu-id="5ffc3-142">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="5ffc3-142">The following is an example of a response.</span></span>
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


