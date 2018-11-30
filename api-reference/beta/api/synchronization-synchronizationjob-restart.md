---
title: 重新启动 synchronizationJob
description: 重新启动同步作业，并强制对它对目录中的所有对象。 （可选） 将清除现有的同步状态和以前的错误。
ms.openlocfilehash: 0b7ebfcd7b13400225d9ea149442207ecd994a8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047716"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="430c2-104">重新启动 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="430c2-104">Restart synchronizationJob</span></span>

> <span data-ttu-id="430c2-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="430c2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="430c2-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="430c2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="430c2-107">重新启动同步作业，并强制对它对目录中的所有对象。</span><span class="sxs-lookup"><span data-stu-id="430c2-107">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="430c2-108">（可选） 将清除现有的同步状态和以前的错误。</span><span class="sxs-lookup"><span data-stu-id="430c2-108">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="430c2-109">权限</span><span class="sxs-lookup"><span data-stu-id="430c2-109">Permissions</span></span>
<span data-ttu-id="430c2-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="430c2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="430c2-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="430c2-112">Permission type</span></span>                        | <span data-ttu-id="430c2-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="430c2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="430c2-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="430c2-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="430c2-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="430c2-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="430c2-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="430c2-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="430c2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="430c2-117">Not supported.</span></span> |
|<span data-ttu-id="430c2-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="430c2-118">Application</span></span>                            |<span data-ttu-id="430c2-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="430c2-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="430c2-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="430c2-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="430c2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="430c2-121">Request headers</span></span>

| <span data-ttu-id="430c2-122">名称</span><span class="sxs-lookup"><span data-stu-id="430c2-122">Name</span></span>           | <span data-ttu-id="430c2-123">类型</span><span class="sxs-lookup"><span data-stu-id="430c2-123">Type</span></span>    | <span data-ttu-id="430c2-124">说明</span><span class="sxs-lookup"><span data-stu-id="430c2-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="430c2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="430c2-125">Authorization</span></span>  | <span data-ttu-id="430c2-126">string</span><span class="sxs-lookup"><span data-stu-id="430c2-126">string</span></span>  | <span data-ttu-id="430c2-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="430c2-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="430c2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="430c2-129">Request body</span></span>

<span data-ttu-id="430c2-130">在请求正文中，将一个 JSON 对象，提供以下参数。</span><span class="sxs-lookup"><span data-stu-id="430c2-130">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="430c2-131">参数</span><span class="sxs-lookup"><span data-stu-id="430c2-131">Parameter</span></span>     | <span data-ttu-id="430c2-132">类型</span><span class="sxs-lookup"><span data-stu-id="430c2-132">Type</span></span>      | <span data-ttu-id="430c2-133">说明</span><span class="sxs-lookup"><span data-stu-id="430c2-133">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="430c2-134">条件</span><span class="sxs-lookup"><span data-stu-id="430c2-134">criteria</span></span>       |[<span data-ttu-id="430c2-135">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="430c2-135">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="430c2-136">重新启动条件</span><span class="sxs-lookup"><span data-stu-id="430c2-136">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="430c2-137">响应</span><span class="sxs-lookup"><span data-stu-id="430c2-137">Response</span></span>

<span data-ttu-id="430c2-138">如果成功，返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="430c2-138">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="430c2-139">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="430c2-139">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="430c2-140">示例</span><span class="sxs-lookup"><span data-stu-id="430c2-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="430c2-141">请求</span><span class="sxs-lookup"><span data-stu-id="430c2-141">Request</span></span>
<span data-ttu-id="430c2-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="430c2-142">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="430c2-143">响应</span><span class="sxs-lookup"><span data-stu-id="430c2-143">Response</span></span>
<span data-ttu-id="430c2-144">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="430c2-144">The following is an example of a response.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob: restart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
