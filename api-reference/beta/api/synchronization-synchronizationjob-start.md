---
title: 启动 synchronizationJob
description: 启动现有同步作业。 如果作业已暂停，它将从暂停点开始继续处理更改。 如果作业位于隔离中，则清除隔离状态。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: fc70f816dfc1e564d27fe5c9be60580eded415e6
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626249"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="8a392-105">启动 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="8a392-105">Start synchronizationJob</span></span>

<span data-ttu-id="8a392-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a392-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a392-107">启动现有同步作业。</span><span class="sxs-lookup"><span data-stu-id="8a392-107">Start an existing synchronization job.</span></span> <span data-ttu-id="8a392-108">如果作业已暂停，它将从暂停点开始继续处理更改。</span><span class="sxs-lookup"><span data-stu-id="8a392-108">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="8a392-109">如果作业位于隔离中，则清除隔离状态。</span><span class="sxs-lookup"><span data-stu-id="8a392-109">If the job is in quarantine, the quarantine status will be cleared.</span></span> <span data-ttu-id="8a392-110">请勿创建脚本以在启动作业运行时持续调用它，因为这可能会导致服务停止运行。</span><span class="sxs-lookup"><span data-stu-id="8a392-110">Do not create scripts to call the start job continuously while it's running because that can cause the service to stop running.</span></span> <span data-ttu-id="8a392-111">仅在作业当前暂停或隔离时，才使用启动作业。</span><span class="sxs-lookup"><span data-stu-id="8a392-111">Use the start job only when the job is currently paused or in quarantine.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8a392-112">权限</span><span class="sxs-lookup"><span data-stu-id="8a392-112">Permissions</span></span>
<span data-ttu-id="8a392-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a392-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a392-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a392-115">Permission type</span></span>                        | <span data-ttu-id="8a392-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a392-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a392-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a392-117">Delegated (work or school account)</span></span>     |<span data-ttu-id="8a392-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a392-118">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="8a392-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a392-119">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="8a392-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a392-120">Not supported.</span></span> |
|<span data-ttu-id="8a392-121">Application</span><span class="sxs-lookup"><span data-stu-id="8a392-121">Application</span></span>                            |<span data-ttu-id="8a392-122">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a392-122">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8a392-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a392-123">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="8a392-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a392-124">Request headers</span></span>

| <span data-ttu-id="8a392-125">名称</span><span class="sxs-lookup"><span data-stu-id="8a392-125">Name</span></span>           | <span data-ttu-id="8a392-126">类型</span><span class="sxs-lookup"><span data-stu-id="8a392-126">Type</span></span>    | <span data-ttu-id="8a392-127">说明</span><span class="sxs-lookup"><span data-stu-id="8a392-127">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="8a392-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a392-128">Authorization</span></span>  | <span data-ttu-id="8a392-129">string</span><span class="sxs-lookup"><span data-stu-id="8a392-129">string</span></span>  | <span data-ttu-id="8a392-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a392-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a392-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a392-132">Request body</span></span>

<span data-ttu-id="8a392-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8a392-133">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="8a392-134">响应</span><span class="sxs-lookup"><span data-stu-id="8a392-134">Response</span></span>

<span data-ttu-id="8a392-135">如果成功，则返回 `204 No Content` 响应。</span><span class="sxs-lookup"><span data-stu-id="8a392-135">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="8a392-136">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8a392-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a392-137">示例</span><span class="sxs-lookup"><span data-stu-id="8a392-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8a392-138">请求</span><span class="sxs-lookup"><span data-stu-id="8a392-138">Request</span></span>
<span data-ttu-id="8a392-139">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="8a392-139">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8a392-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a392-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="c"></a>[<span data-ttu-id="8a392-141">C#</span><span class="sxs-lookup"><span data-stu-id="8a392-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a392-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a392-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a392-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a392-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a392-144">Java</span><span class="sxs-lookup"><span data-stu-id="8a392-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8a392-145">响应</span><span class="sxs-lookup"><span data-stu-id="8a392-145">Response</span></span>
<span data-ttu-id="8a392-146">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="8a392-146">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


