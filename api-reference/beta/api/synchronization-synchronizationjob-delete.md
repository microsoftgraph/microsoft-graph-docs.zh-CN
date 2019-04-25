---
title: 删除 synchronizationJob
description: 停止同步作业, 并永久删除与之关联的所有状态。 同步帐户保留为。
localization_priority: Normal
ms.openlocfilehash: 29083413c5b24a5ed07b671adfa048f58d437f0d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545212"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="418eb-104">删除 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="418eb-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="418eb-105">停止同步作业, 并永久删除与之关联的所有状态。</span><span class="sxs-lookup"><span data-stu-id="418eb-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="418eb-106">同步帐户保留为。</span><span class="sxs-lookup"><span data-stu-id="418eb-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="418eb-107">权限</span><span class="sxs-lookup"><span data-stu-id="418eb-107">Permissions</span></span>
<span data-ttu-id="418eb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="418eb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="418eb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="418eb-110">Permission type</span></span>                        | <span data-ttu-id="418eb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="418eb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="418eb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="418eb-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="418eb-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="418eb-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="418eb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="418eb-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="418eb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="418eb-115">Not supported.</span></span>  |
|<span data-ttu-id="418eb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="418eb-116">Application</span></span>                            |<span data-ttu-id="418eb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="418eb-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="418eb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="418eb-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="418eb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="418eb-119">Request headers</span></span>

| <span data-ttu-id="418eb-120">名称</span><span class="sxs-lookup"><span data-stu-id="418eb-120">Name</span></span>           | <span data-ttu-id="418eb-121">类型</span><span class="sxs-lookup"><span data-stu-id="418eb-121">Type</span></span>    | <span data-ttu-id="418eb-122">说明</span><span class="sxs-lookup"><span data-stu-id="418eb-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="418eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="418eb-123">Authorization</span></span>  | <span data-ttu-id="418eb-124">string</span><span class="sxs-lookup"><span data-stu-id="418eb-124">string</span></span>  | <span data-ttu-id="418eb-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="418eb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="418eb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="418eb-127">Request body</span></span>

<span data-ttu-id="418eb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="418eb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="418eb-129">响应</span><span class="sxs-lookup"><span data-stu-id="418eb-129">Response</span></span>

<span data-ttu-id="418eb-130">如果成功, 则返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="418eb-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="418eb-131">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="418eb-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="418eb-132">示例</span><span class="sxs-lookup"><span data-stu-id="418eb-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="418eb-133">请求</span><span class="sxs-lookup"><span data-stu-id="418eb-133">Request</span></span>
<span data-ttu-id="418eb-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="418eb-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="418eb-135">响应</span><span class="sxs-lookup"><span data-stu-id="418eb-135">Response</span></span>
<span data-ttu-id="418eb-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="418eb-136">The following is an example of the response.</span></span> 

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
