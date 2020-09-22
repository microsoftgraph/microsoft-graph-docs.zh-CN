---
title: 启动 synchronizationJob
description: 启动现有的同步作业。 如果作业处于暂停状态，它将继续处理暂停的点处的更改。 如果作业在隔离中，隔离状态将被清除。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8135c81c0046dfd67b830e0c8c8a075e4550ef74
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044289"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="c19b2-105">启动 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="c19b2-105">Start synchronizationJob</span></span>

<span data-ttu-id="c19b2-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c19b2-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c19b2-107">启动现有的同步作业。</span><span class="sxs-lookup"><span data-stu-id="c19b2-107">Start an existing synchronization job.</span></span> <span data-ttu-id="c19b2-108">如果作业处于暂停状态，它将继续处理暂停的点处的更改。</span><span class="sxs-lookup"><span data-stu-id="c19b2-108">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="c19b2-109">如果作业在隔离中，隔离状态将被清除。</span><span class="sxs-lookup"><span data-stu-id="c19b2-109">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="c19b2-110">权限</span><span class="sxs-lookup"><span data-stu-id="c19b2-110">Permissions</span></span>
<span data-ttu-id="c19b2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c19b2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c19b2-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c19b2-113">Permission type</span></span>                        | <span data-ttu-id="c19b2-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c19b2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c19b2-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c19b2-115">Delegated (work or school account)</span></span>     |<span data-ttu-id="c19b2-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c19b2-116">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c19b2-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c19b2-117">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c19b2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c19b2-118">Not supported.</span></span> |
|<span data-ttu-id="c19b2-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c19b2-119">Application</span></span>                            |<span data-ttu-id="c19b2-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="c19b2-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c19b2-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c19b2-121">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="c19b2-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c19b2-122">Request headers</span></span>

| <span data-ttu-id="c19b2-123">名称</span><span class="sxs-lookup"><span data-stu-id="c19b2-123">Name</span></span>           | <span data-ttu-id="c19b2-124">类型</span><span class="sxs-lookup"><span data-stu-id="c19b2-124">Type</span></span>    | <span data-ttu-id="c19b2-125">说明</span><span class="sxs-lookup"><span data-stu-id="c19b2-125">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c19b2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c19b2-126">Authorization</span></span>  | <span data-ttu-id="c19b2-127">string</span><span class="sxs-lookup"><span data-stu-id="c19b2-127">string</span></span>  | <span data-ttu-id="c19b2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c19b2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c19b2-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c19b2-130">Request body</span></span>

<span data-ttu-id="c19b2-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c19b2-131">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="c19b2-132">响应</span><span class="sxs-lookup"><span data-stu-id="c19b2-132">Response</span></span>

<span data-ttu-id="c19b2-133">如果成功，则返回 `204 No Content` 响应。</span><span class="sxs-lookup"><span data-stu-id="c19b2-133">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="c19b2-134">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c19b2-134">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c19b2-135">示例</span><span class="sxs-lookup"><span data-stu-id="c19b2-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c19b2-136">请求</span><span class="sxs-lookup"><span data-stu-id="c19b2-136">Request</span></span>
<span data-ttu-id="c19b2-137">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="c19b2-137">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c19b2-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c19b2-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="c"></a>[<span data-ttu-id="c19b2-139">C#</span><span class="sxs-lookup"><span data-stu-id="c19b2-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c19b2-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c19b2-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c19b2-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c19b2-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c19b2-142">响应</span><span class="sxs-lookup"><span data-stu-id="c19b2-142">Response</span></span>
<span data-ttu-id="c19b2-143">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="c19b2-143">The following is an example of a response.</span></span>
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


