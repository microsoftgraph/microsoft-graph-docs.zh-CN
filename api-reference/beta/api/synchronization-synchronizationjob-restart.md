---
title: 重新启动 synchronizationJob
description: 重新启动同步作业, 强制它重新处理目录中的所有对象。 (可选) 清除现有同步状态和以前的错误。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 765b8801c808a71426fc6a5150229e028429436f
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621086"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="3ae67-104">重新启动 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="3ae67-104">Restart synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ae67-105">重新启动同步作业, 强制它重新处理目录中的所有对象。</span><span class="sxs-lookup"><span data-stu-id="3ae67-105">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="3ae67-106">(可选) 清除现有同步状态和以前的错误。</span><span class="sxs-lookup"><span data-stu-id="3ae67-106">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ae67-107">权限</span><span class="sxs-lookup"><span data-stu-id="3ae67-107">Permissions</span></span>
<span data-ttu-id="3ae67-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ae67-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ae67-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ae67-110">Permission type</span></span>                        | <span data-ttu-id="3ae67-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ae67-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ae67-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ae67-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="3ae67-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ae67-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3ae67-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ae67-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3ae67-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ae67-115">Not supported.</span></span> |
|<span data-ttu-id="3ae67-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ae67-116">Application</span></span>                            |<span data-ttu-id="3ae67-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ae67-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="3ae67-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ae67-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="3ae67-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ae67-119">Request headers</span></span>

| <span data-ttu-id="3ae67-120">名称</span><span class="sxs-lookup"><span data-stu-id="3ae67-120">Name</span></span>           | <span data-ttu-id="3ae67-121">类型</span><span class="sxs-lookup"><span data-stu-id="3ae67-121">Type</span></span>    | <span data-ttu-id="3ae67-122">说明</span><span class="sxs-lookup"><span data-stu-id="3ae67-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="3ae67-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ae67-123">Authorization</span></span>  | <span data-ttu-id="3ae67-124">string</span><span class="sxs-lookup"><span data-stu-id="3ae67-124">string</span></span>  | <span data-ttu-id="3ae67-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ae67-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ae67-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ae67-127">Request body</span></span>

<span data-ttu-id="3ae67-128">在请求正文中, 提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3ae67-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="3ae67-129">参数</span><span class="sxs-lookup"><span data-stu-id="3ae67-129">Parameter</span></span>     | <span data-ttu-id="3ae67-130">类型</span><span class="sxs-lookup"><span data-stu-id="3ae67-130">Type</span></span>      | <span data-ttu-id="3ae67-131">说明</span><span class="sxs-lookup"><span data-stu-id="3ae67-131">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="3ae67-132">条件</span><span class="sxs-lookup"><span data-stu-id="3ae67-132">criteria</span></span>       |[<span data-ttu-id="3ae67-133">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="3ae67-133">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="3ae67-134">重新启动条件</span><span class="sxs-lookup"><span data-stu-id="3ae67-134">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="3ae67-135">响应</span><span class="sxs-lookup"><span data-stu-id="3ae67-135">Response</span></span>

<span data-ttu-id="3ae67-136">如果成功, 则返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="3ae67-136">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="3ae67-137">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3ae67-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ae67-138">示例</span><span class="sxs-lookup"><span data-stu-id="3ae67-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3ae67-139">请求</span><span class="sxs-lookup"><span data-stu-id="3ae67-139">Request</span></span>
<span data-ttu-id="3ae67-140">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="3ae67-140">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3ae67-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3ae67-141">HTTP</span></span>](#tab/http)
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
       "resetScope": "ConnectorDataStore, Escrows, QuarantineState"
   }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3ae67-142">C#</span><span class="sxs-lookup"><span data-stu-id="3ae67-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-restart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ae67-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="3ae67-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-restart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3ae67-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="3ae67-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-restart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3ae67-145">响应</span><span class="sxs-lookup"><span data-stu-id="3ae67-145">Response</span></span>
<span data-ttu-id="3ae67-146">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="3ae67-146">The following is an example of a response.</span></span>

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
