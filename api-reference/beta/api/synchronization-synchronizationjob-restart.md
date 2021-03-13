---
title: 重新启动 synchronizationJob
description: 重新启动同步作业，强制它重新处理目录中的所有对象。 （可选）清除现有同步状态和以前的错误。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 216da34bb6900d246f990529c88bc398cc1cdcc7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50775072"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="dd35c-104">重新启动 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="dd35c-104">Restart synchronizationJob</span></span>

<span data-ttu-id="dd35c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd35c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd35c-106">重新启动同步作业，强制它重新处理目录中的所有对象。</span><span class="sxs-lookup"><span data-stu-id="dd35c-106">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="dd35c-107">（可选）清除现有同步状态和以前的错误。</span><span class="sxs-lookup"><span data-stu-id="dd35c-107">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd35c-108">权限</span><span class="sxs-lookup"><span data-stu-id="dd35c-108">Permissions</span></span>
<span data-ttu-id="dd35c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd35c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd35c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd35c-111">Permission type</span></span>                        | <span data-ttu-id="dd35c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd35c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd35c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd35c-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="dd35c-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd35c-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="dd35c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd35c-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="dd35c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd35c-116">Not supported.</span></span> |
|<span data-ttu-id="dd35c-117">Application</span><span class="sxs-lookup"><span data-stu-id="dd35c-117">Application</span></span>                            |<span data-ttu-id="dd35c-118">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd35c-118">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="dd35c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd35c-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="dd35c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd35c-120">Request headers</span></span>

| <span data-ttu-id="dd35c-121">名称</span><span class="sxs-lookup"><span data-stu-id="dd35c-121">Name</span></span>           | <span data-ttu-id="dd35c-122">类型</span><span class="sxs-lookup"><span data-stu-id="dd35c-122">Type</span></span>    | <span data-ttu-id="dd35c-123">说明</span><span class="sxs-lookup"><span data-stu-id="dd35c-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="dd35c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd35c-124">Authorization</span></span>  | <span data-ttu-id="dd35c-125">string</span><span class="sxs-lookup"><span data-stu-id="dd35c-125">string</span></span>  | <span data-ttu-id="dd35c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dd35c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd35c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd35c-128">Request body</span></span>

<span data-ttu-id="dd35c-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="dd35c-129">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="dd35c-130">参数</span><span class="sxs-lookup"><span data-stu-id="dd35c-130">Parameter</span></span>     | <span data-ttu-id="dd35c-131">类型</span><span class="sxs-lookup"><span data-stu-id="dd35c-131">Type</span></span>      | <span data-ttu-id="dd35c-132">说明</span><span class="sxs-lookup"><span data-stu-id="dd35c-132">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="dd35c-133">条件</span><span class="sxs-lookup"><span data-stu-id="dd35c-133">criteria</span></span>       |[<span data-ttu-id="dd35c-134">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="dd35c-134">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="dd35c-135">重新启动条件</span><span class="sxs-lookup"><span data-stu-id="dd35c-135">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="dd35c-136">响应</span><span class="sxs-lookup"><span data-stu-id="dd35c-136">Response</span></span>

<span data-ttu-id="dd35c-137">如果成功，则返回 `204 No Content` 响应。</span><span class="sxs-lookup"><span data-stu-id="dd35c-137">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="dd35c-138">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dd35c-138">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd35c-139">示例</span><span class="sxs-lookup"><span data-stu-id="dd35c-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dd35c-140">请求</span><span class="sxs-lookup"><span data-stu-id="dd35c-140">Request</span></span>
<span data-ttu-id="dd35c-141">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="dd35c-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd35c-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd35c-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_restart"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
Authorization: Bearer <token>
Content-type: application/json

{
   "criteria": {
       "resetScope": "Watermark, Escrows, QuarantineState"
   }
}
```
# <a name="c"></a>[<span data-ttu-id="dd35c-143">C#</span><span class="sxs-lookup"><span data-stu-id="dd35c-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-restart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd35c-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd35c-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-restart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd35c-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd35c-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-restart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd35c-146">Java</span><span class="sxs-lookup"><span data-stu-id="dd35c-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-restart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dd35c-147">响应</span><span class="sxs-lookup"><span data-stu-id="dd35c-147">Response</span></span>
<span data-ttu-id="dd35c-148">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="dd35c-148">The following is an example of a response.</span></span>

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
  "description": "synchronizationJob: restart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


