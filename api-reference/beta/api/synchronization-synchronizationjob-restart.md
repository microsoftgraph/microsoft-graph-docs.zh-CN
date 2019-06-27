---
title: 重新启动 synchronizationJob
description: 重新启动同步作业, 强制它重新处理目录中的所有对象。 (可选) 清除现有同步状态和以前的错误。
localization_priority: Normal
ms.openlocfilehash: a97aa458bdecb9e6755add708a5e9799e1365b74
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271363"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="95452-104">重新启动 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="95452-104">Restart synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95452-105">重新启动同步作业, 强制它重新处理目录中的所有对象。</span><span class="sxs-lookup"><span data-stu-id="95452-105">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="95452-106">(可选) 清除现有同步状态和以前的错误。</span><span class="sxs-lookup"><span data-stu-id="95452-106">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="95452-107">权限</span><span class="sxs-lookup"><span data-stu-id="95452-107">Permissions</span></span>
<span data-ttu-id="95452-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95452-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95452-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="95452-110">Permission type</span></span>                        | <span data-ttu-id="95452-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="95452-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="95452-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95452-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="95452-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95452-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="95452-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95452-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="95452-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="95452-115">Not supported.</span></span> |
|<span data-ttu-id="95452-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="95452-116">Application</span></span>                            |<span data-ttu-id="95452-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="95452-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="95452-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95452-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="95452-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="95452-119">Request headers</span></span>

| <span data-ttu-id="95452-120">名称</span><span class="sxs-lookup"><span data-stu-id="95452-120">Name</span></span>           | <span data-ttu-id="95452-121">类型</span><span class="sxs-lookup"><span data-stu-id="95452-121">Type</span></span>    | <span data-ttu-id="95452-122">说明</span><span class="sxs-lookup"><span data-stu-id="95452-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="95452-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="95452-123">Authorization</span></span>  | <span data-ttu-id="95452-124">string</span><span class="sxs-lookup"><span data-stu-id="95452-124">string</span></span>  | <span data-ttu-id="95452-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="95452-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95452-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="95452-127">Request body</span></span>

<span data-ttu-id="95452-128">在请求正文中, 提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="95452-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="95452-129">参数</span><span class="sxs-lookup"><span data-stu-id="95452-129">Parameter</span></span>     | <span data-ttu-id="95452-130">类型</span><span class="sxs-lookup"><span data-stu-id="95452-130">Type</span></span>      | <span data-ttu-id="95452-131">说明</span><span class="sxs-lookup"><span data-stu-id="95452-131">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="95452-132">条件</span><span class="sxs-lookup"><span data-stu-id="95452-132">criteria</span></span>       |[<span data-ttu-id="95452-133">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="95452-133">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="95452-134">重新启动条件</span><span class="sxs-lookup"><span data-stu-id="95452-134">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="95452-135">响应</span><span class="sxs-lookup"><span data-stu-id="95452-135">Response</span></span>

<span data-ttu-id="95452-136">如果成功, 则返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="95452-136">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="95452-137">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="95452-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95452-138">示例</span><span class="sxs-lookup"><span data-stu-id="95452-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="95452-139">请求</span><span class="sxs-lookup"><span data-stu-id="95452-139">Request</span></span>
<span data-ttu-id="95452-140">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="95452-140">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="95452-141">响应</span><span class="sxs-lookup"><span data-stu-id="95452-141">Response</span></span>
<span data-ttu-id="95452-142">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="95452-142">The following is an example of a response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="95452-143">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="95452-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="95452-144">C#</span><span class="sxs-lookup"><span data-stu-id="95452-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationjob_restart-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="95452-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="95452-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationjob_restart-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="95452-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="95452-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/synchronizationjob_restart-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
