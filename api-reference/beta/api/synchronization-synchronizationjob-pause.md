---
title: synchronizationJob： 暂停
description: 暂时停止同步。 所有的进度，包括作业状态保持不变，且该作业将继续从停止时开始调用的地方。
ms.openlocfilehash: dd46f5760d7ddcfff1e254d7c000e1cd80304f07
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043979"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="78635-104">synchronizationJob： 暂停</span><span class="sxs-lookup"><span data-stu-id="78635-104">synchronizationJob: pause</span></span>

> <span data-ttu-id="78635-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="78635-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78635-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="78635-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78635-107">暂时停止同步。</span><span class="sxs-lookup"><span data-stu-id="78635-107">Temporarily stop synchronization.</span></span> <span data-ttu-id="78635-108">所有的进度，包括作业状态保持不变，且该作业将继续从停止时[启动](../api/synchronization-synchronizationjob-start.md)调用的地方。</span><span class="sxs-lookup"><span data-stu-id="78635-108">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="78635-109">权限</span><span class="sxs-lookup"><span data-stu-id="78635-109">Permissions</span></span>
<span data-ttu-id="78635-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78635-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78635-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="78635-112">Permission type</span></span>                        | <span data-ttu-id="78635-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78635-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="78635-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78635-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="78635-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78635-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="78635-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78635-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="78635-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="78635-117">Not supported.</span></span>  |
|<span data-ttu-id="78635-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="78635-118">Application</span></span>                            |<span data-ttu-id="78635-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="78635-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="78635-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78635-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="78635-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="78635-121">Request headers</span></span>

| <span data-ttu-id="78635-122">名称</span><span class="sxs-lookup"><span data-stu-id="78635-122">Name</span></span>           | <span data-ttu-id="78635-123">类型</span><span class="sxs-lookup"><span data-stu-id="78635-123">Type</span></span>    | <span data-ttu-id="78635-124">说明</span><span class="sxs-lookup"><span data-stu-id="78635-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="78635-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="78635-125">Authorization</span></span>  | <span data-ttu-id="78635-126">string</span><span class="sxs-lookup"><span data-stu-id="78635-126">string</span></span>  | <span data-ttu-id="78635-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78635-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78635-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="78635-129">Request body</span></span>

<span data-ttu-id="78635-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="78635-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78635-131">响应</span><span class="sxs-lookup"><span data-stu-id="78635-131">Response</span></span>

<span data-ttu-id="78635-132">如果成功，返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="78635-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="78635-133">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="78635-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78635-134">示例</span><span class="sxs-lookup"><span data-stu-id="78635-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="78635-135">请求</span><span class="sxs-lookup"><span data-stu-id="78635-135">Request</span></span>
<span data-ttu-id="78635-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78635-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="78635-137">响应</span><span class="sxs-lookup"><span data-stu-id="78635-137">Response</span></span>
<span data-ttu-id="78635-138">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="78635-138">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: pause",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->