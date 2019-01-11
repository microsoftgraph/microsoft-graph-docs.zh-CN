---
title: 创建 synchronizationJob
description: 使用默认同步架构创建新的同步作业。 作业创建处于禁用状态。 呼叫开始作业启动同步。
localization_priority: Normal
ms.openlocfilehash: 04b8e383c923968b150067c9d2c3a65ce32bd9c0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842222"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="304b0-105">创建 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="304b0-105">Create synchronizationJob</span></span>

> <span data-ttu-id="304b0-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="304b0-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="304b0-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="304b0-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="304b0-108">使用默认同步架构创建新的同步作业。</span><span class="sxs-lookup"><span data-stu-id="304b0-108">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="304b0-109">作业创建处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="304b0-109">The job is created in a disabled state.</span></span> <span data-ttu-id="304b0-110">调用[启动作业](synchronization-synchronizationjob-start.md)启动同步。</span><span class="sxs-lookup"><span data-stu-id="304b0-110">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="304b0-111">权限</span><span class="sxs-lookup"><span data-stu-id="304b0-111">Permissions</span></span>
<span data-ttu-id="304b0-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="304b0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="304b0-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="304b0-114">Permission type</span></span>                        | <span data-ttu-id="304b0-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="304b0-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="304b0-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="304b0-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="304b0-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="304b0-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="304b0-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="304b0-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="304b0-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="304b0-119">Not supported.</span></span>|
|<span data-ttu-id="304b0-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="304b0-120">Application</span></span>                            |<span data-ttu-id="304b0-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="304b0-121">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="304b0-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="304b0-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="304b0-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="304b0-123">Request headers</span></span>

| <span data-ttu-id="304b0-124">名称</span><span class="sxs-lookup"><span data-stu-id="304b0-124">Name</span></span>           | <span data-ttu-id="304b0-125">类型</span><span class="sxs-lookup"><span data-stu-id="304b0-125">Type</span></span>    | <span data-ttu-id="304b0-126">说明</span><span class="sxs-lookup"><span data-stu-id="304b0-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="304b0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="304b0-127">Authorization</span></span>  | <span data-ttu-id="304b0-128">string</span><span class="sxs-lookup"><span data-stu-id="304b0-128">string</span></span>  | <span data-ttu-id="304b0-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="304b0-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="304b0-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="304b0-131">Request body</span></span>

<span data-ttu-id="304b0-132">在请求正文中，提供要创建的[synchronizationJob](../resources/synchronization-synchronizationjob.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="304b0-132">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="304b0-133">仅 required 的属性是`templateId`。</span><span class="sxs-lookup"><span data-stu-id="304b0-133">The only required property is `templateId`.</span></span> <span data-ttu-id="304b0-134">`templateId`属性必须匹配的模板创建的此应用程序/服务主体之一。</span><span class="sxs-lookup"><span data-stu-id="304b0-134">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="304b0-135">若要查找可用的模板，请使用[列表模板](synchronization-synchronizationtemplate-list.md)。</span><span class="sxs-lookup"><span data-stu-id="304b0-135">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="304b0-136">响应</span><span class="sxs-lookup"><span data-stu-id="304b0-136">Response</span></span>

<span data-ttu-id="304b0-137">如果成功，返回`201 Created`响应代码和响应正文中的[synchronizationJob](../resources/synchronization-synchronizationjob.md)对象。</span><span class="sxs-lookup"><span data-stu-id="304b0-137">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="304b0-138">示例</span><span class="sxs-lookup"><span data-stu-id="304b0-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="304b0-139">请求</span><span class="sxs-lookup"><span data-stu-id="304b0-139">Request</span></span>
<span data-ttu-id="304b0-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="304b0-140">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_synchronizationjob_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
Content-type: application/json

{ 
    "templateId": "BoxOutDelta"
}
```

##### <a name="response"></a><span data-ttu-id="304b0-141">响应</span><span class="sxs-lookup"><span data-stu-id="304b0-141">Response</span></span>
<span data-ttu-id="304b0-142">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="304b0-142">The following is an example of a response.</span></span> 

><span data-ttu-id="304b0-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="304b0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "{jobId}",
    "templateId": "BoxOutDelta",
    "schedule": {
        "expiration": null,
        "interval": "P10675199DT2H48M5.4775807S",
        "state": "Disabled"
    },
    "status": {
        "countSuccessiveCompleteFailures": 0,
        "escrowsPruned": false,
        "synchronizedEntryCountByType": [],
        "code": "NotConfigured",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
        "lastSuccessfulExecutionWithExports": null,
        "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
        "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
        "quarantine": null,
        "troubleshootingUrl": null
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
