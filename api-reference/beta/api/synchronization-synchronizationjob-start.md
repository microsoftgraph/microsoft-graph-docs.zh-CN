---
title: 启动 synchronizationJob
description: 启动现有同步作业。 如果该作业暂停状态，它将继续处理更改从暂停的位置的点。 如果该作业在隔离，将被清除隔离状态。
localization_priority: Normal
ms.openlocfilehash: 478f29d1c49cf6cc820fcc52393f4721ff94caac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826213"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="71797-105">启动 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="71797-105">Start synchronizationJob</span></span>

> <span data-ttu-id="71797-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="71797-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71797-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="71797-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71797-108">启动现有同步作业。</span><span class="sxs-lookup"><span data-stu-id="71797-108">Start an existing synchronization job.</span></span> <span data-ttu-id="71797-109">如果该作业暂停状态，它将继续处理更改从暂停的位置的点。</span><span class="sxs-lookup"><span data-stu-id="71797-109">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="71797-110">如果该作业在隔离，将被清除隔离状态。</span><span class="sxs-lookup"><span data-stu-id="71797-110">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="71797-111">权限</span><span class="sxs-lookup"><span data-stu-id="71797-111">Permissions</span></span>
<span data-ttu-id="71797-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71797-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71797-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="71797-114">Permission type</span></span>                        | <span data-ttu-id="71797-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71797-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="71797-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71797-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="71797-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71797-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="71797-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71797-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="71797-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="71797-119">Not supported.</span></span> |
|<span data-ttu-id="71797-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="71797-120">Application</span></span>                            |<span data-ttu-id="71797-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="71797-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="71797-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71797-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="71797-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="71797-123">Request headers</span></span>

| <span data-ttu-id="71797-124">名称</span><span class="sxs-lookup"><span data-stu-id="71797-124">Name</span></span>           | <span data-ttu-id="71797-125">类型</span><span class="sxs-lookup"><span data-stu-id="71797-125">Type</span></span>    | <span data-ttu-id="71797-126">说明</span><span class="sxs-lookup"><span data-stu-id="71797-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="71797-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="71797-127">Authorization</span></span>  | <span data-ttu-id="71797-128">string</span><span class="sxs-lookup"><span data-stu-id="71797-128">string</span></span>  | <span data-ttu-id="71797-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71797-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71797-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="71797-131">Request body</span></span>

<span data-ttu-id="71797-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71797-132">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="71797-133">响应</span><span class="sxs-lookup"><span data-stu-id="71797-133">Response</span></span>

<span data-ttu-id="71797-134">如果成功，返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="71797-134">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="71797-135">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="71797-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71797-136">示例</span><span class="sxs-lookup"><span data-stu-id="71797-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="71797-137">请求</span><span class="sxs-lookup"><span data-stu-id="71797-137">Request</span></span>
<span data-ttu-id="71797-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71797-138">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a><span data-ttu-id="71797-139">响应</span><span class="sxs-lookup"><span data-stu-id="71797-139">Response</span></span>
<span data-ttu-id="71797-140">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="71797-140">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
