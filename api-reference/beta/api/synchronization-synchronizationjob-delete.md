---
title: 删除 synchronizationJob
description: 停止同步作业，并永久删除所有与之关联的状态。 同步的帐户保留为-是。
localization_priority: Normal
ms.openlocfilehash: 95a7d52e9e6fba9bc3f528aedfc5a082d459a003
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835684"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="2ffdd-104">删除 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="2ffdd-104">Delete synchronizationJob</span></span>

> <span data-ttu-id="2ffdd-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2ffdd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ffdd-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2ffdd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2ffdd-107">停止同步作业，并永久删除所有与之关联的状态。</span><span class="sxs-lookup"><span data-stu-id="2ffdd-107">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="2ffdd-108">同步的帐户保留为-是。</span><span class="sxs-lookup"><span data-stu-id="2ffdd-108">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ffdd-109">权限</span><span class="sxs-lookup"><span data-stu-id="2ffdd-109">Permissions</span></span>
<span data-ttu-id="2ffdd-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ffdd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ffdd-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ffdd-112">Permission type</span></span>                        | <span data-ttu-id="2ffdd-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ffdd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ffdd-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ffdd-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="2ffdd-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ffdd-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="2ffdd-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ffdd-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="2ffdd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ffdd-117">Not supported.</span></span>  |
|<span data-ttu-id="2ffdd-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ffdd-118">Application</span></span>                            |<span data-ttu-id="2ffdd-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ffdd-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2ffdd-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ffdd-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="2ffdd-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ffdd-121">Request headers</span></span>

| <span data-ttu-id="2ffdd-122">名称</span><span class="sxs-lookup"><span data-stu-id="2ffdd-122">Name</span></span>           | <span data-ttu-id="2ffdd-123">类型</span><span class="sxs-lookup"><span data-stu-id="2ffdd-123">Type</span></span>    | <span data-ttu-id="2ffdd-124">说明</span><span class="sxs-lookup"><span data-stu-id="2ffdd-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="2ffdd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ffdd-125">Authorization</span></span>  | <span data-ttu-id="2ffdd-126">string</span><span class="sxs-lookup"><span data-stu-id="2ffdd-126">string</span></span>  | <span data-ttu-id="2ffdd-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ffdd-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ffdd-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ffdd-129">Request body</span></span>

<span data-ttu-id="2ffdd-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ffdd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ffdd-131">响应</span><span class="sxs-lookup"><span data-stu-id="2ffdd-131">Response</span></span>

<span data-ttu-id="2ffdd-132">如果成功，返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="2ffdd-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="2ffdd-133">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="2ffdd-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ffdd-134">示例</span><span class="sxs-lookup"><span data-stu-id="2ffdd-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2ffdd-135">请求</span><span class="sxs-lookup"><span data-stu-id="2ffdd-135">Request</span></span>
<span data-ttu-id="2ffdd-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ffdd-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="2ffdd-137">响应</span><span class="sxs-lookup"><span data-stu-id="2ffdd-137">Response</span></span>
<span data-ttu-id="2ffdd-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2ffdd-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
