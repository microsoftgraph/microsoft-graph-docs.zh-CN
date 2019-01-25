---
title: 删除 synchronizationJob
description: 停止同步作业，并永久删除所有与之关联的状态。 同步的帐户保留为-是。
localization_priority: Normal
ms.openlocfilehash: 29083413c5b24a5ed07b671adfa048f58d437f0d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521682"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="16a90-104">删除 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="16a90-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16a90-105">停止同步作业，并永久删除所有与之关联的状态。</span><span class="sxs-lookup"><span data-stu-id="16a90-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="16a90-106">同步的帐户保留为-是。</span><span class="sxs-lookup"><span data-stu-id="16a90-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="16a90-107">权限</span><span class="sxs-lookup"><span data-stu-id="16a90-107">Permissions</span></span>
<span data-ttu-id="16a90-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16a90-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16a90-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="16a90-110">Permission type</span></span>                        | <span data-ttu-id="16a90-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16a90-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="16a90-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16a90-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="16a90-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16a90-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="16a90-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16a90-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="16a90-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="16a90-115">Not supported.</span></span>  |
|<span data-ttu-id="16a90-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="16a90-116">Application</span></span>                            |<span data-ttu-id="16a90-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="16a90-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="16a90-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16a90-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="16a90-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="16a90-119">Request headers</span></span>

| <span data-ttu-id="16a90-120">名称</span><span class="sxs-lookup"><span data-stu-id="16a90-120">Name</span></span>           | <span data-ttu-id="16a90-121">类型</span><span class="sxs-lookup"><span data-stu-id="16a90-121">Type</span></span>    | <span data-ttu-id="16a90-122">说明</span><span class="sxs-lookup"><span data-stu-id="16a90-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="16a90-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16a90-123">Authorization</span></span>  | <span data-ttu-id="16a90-124">string</span><span class="sxs-lookup"><span data-stu-id="16a90-124">string</span></span>  | <span data-ttu-id="16a90-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16a90-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16a90-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="16a90-127">Request body</span></span>

<span data-ttu-id="16a90-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16a90-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16a90-129">响应</span><span class="sxs-lookup"><span data-stu-id="16a90-129">Response</span></span>

<span data-ttu-id="16a90-130">如果成功，返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="16a90-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="16a90-131">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="16a90-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16a90-132">示例</span><span class="sxs-lookup"><span data-stu-id="16a90-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="16a90-133">请求</span><span class="sxs-lookup"><span data-stu-id="16a90-133">Request</span></span>
<span data-ttu-id="16a90-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16a90-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="16a90-135">响应</span><span class="sxs-lookup"><span data-stu-id="16a90-135">Response</span></span>
<span data-ttu-id="16a90-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="16a90-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
