---
title: 重新启动 synchronizationJob
description: 重新启动同步作业，并强制对它对目录中的所有对象。 （可选） 将清除现有的同步状态和以前的错误。
localization_priority: Normal
ms.openlocfilehash: 169f95c3662fd774207584b54fcf27fb2548c795
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526723"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="2d94e-104">重新启动 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="2d94e-104">Restart synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d94e-105">重新启动同步作业，并强制对它对目录中的所有对象。</span><span class="sxs-lookup"><span data-stu-id="2d94e-105">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="2d94e-106">（可选） 将清除现有的同步状态和以前的错误。</span><span class="sxs-lookup"><span data-stu-id="2d94e-106">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d94e-107">权限</span><span class="sxs-lookup"><span data-stu-id="2d94e-107">Permissions</span></span>
<span data-ttu-id="2d94e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d94e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d94e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d94e-110">Permission type</span></span>                        | <span data-ttu-id="2d94e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d94e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d94e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d94e-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="2d94e-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d94e-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="2d94e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d94e-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="2d94e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d94e-115">Not supported.</span></span> |
|<span data-ttu-id="2d94e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d94e-116">Application</span></span>                            |<span data-ttu-id="2d94e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d94e-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="2d94e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d94e-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="2d94e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d94e-119">Request headers</span></span>

| <span data-ttu-id="2d94e-120">名称</span><span class="sxs-lookup"><span data-stu-id="2d94e-120">Name</span></span>           | <span data-ttu-id="2d94e-121">类型</span><span class="sxs-lookup"><span data-stu-id="2d94e-121">Type</span></span>    | <span data-ttu-id="2d94e-122">说明</span><span class="sxs-lookup"><span data-stu-id="2d94e-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="2d94e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d94e-123">Authorization</span></span>  | <span data-ttu-id="2d94e-124">string</span><span class="sxs-lookup"><span data-stu-id="2d94e-124">string</span></span>  | <span data-ttu-id="2d94e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d94e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d94e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d94e-127">Request body</span></span>

<span data-ttu-id="2d94e-128">在请求正文中，将一个 JSON 对象，提供以下参数。</span><span class="sxs-lookup"><span data-stu-id="2d94e-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="2d94e-129">参数</span><span class="sxs-lookup"><span data-stu-id="2d94e-129">Parameter</span></span>     | <span data-ttu-id="2d94e-130">类型</span><span class="sxs-lookup"><span data-stu-id="2d94e-130">Type</span></span>      | <span data-ttu-id="2d94e-131">说明</span><span class="sxs-lookup"><span data-stu-id="2d94e-131">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="2d94e-132">条件</span><span class="sxs-lookup"><span data-stu-id="2d94e-132">criteria</span></span>       |[<span data-ttu-id="2d94e-133">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="2d94e-133">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="2d94e-134">重新启动条件</span><span class="sxs-lookup"><span data-stu-id="2d94e-134">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="2d94e-135">响应</span><span class="sxs-lookup"><span data-stu-id="2d94e-135">Response</span></span>

<span data-ttu-id="2d94e-136">如果成功，返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="2d94e-136">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="2d94e-137">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="2d94e-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d94e-138">示例</span><span class="sxs-lookup"><span data-stu-id="2d94e-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2d94e-139">请求</span><span class="sxs-lookup"><span data-stu-id="2d94e-139">Request</span></span>
<span data-ttu-id="2d94e-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d94e-140">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2d94e-141">响应</span><span class="sxs-lookup"><span data-stu-id="2d94e-141">Response</span></span>
<span data-ttu-id="2d94e-142">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="2d94e-142">The following is an example of a response.</span></span>

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
