---
title: 启动 synchronizationJob
description: 启动现有同步作业。 如果该作业暂停状态，它将继续处理更改从暂停的位置的点。 如果该作业在隔离，将被清除隔离状态。
localization_priority: Normal
ms.openlocfilehash: 4648d9d3d889adf2cd7ec06e4fcf79b761c77132
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515368"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="25164-105">启动 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="25164-105">Start synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25164-106">启动现有同步作业。</span><span class="sxs-lookup"><span data-stu-id="25164-106">Start an existing synchronization job.</span></span> <span data-ttu-id="25164-107">如果该作业暂停状态，它将继续处理更改从暂停的位置的点。</span><span class="sxs-lookup"><span data-stu-id="25164-107">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="25164-108">如果该作业在隔离，将被清除隔离状态。</span><span class="sxs-lookup"><span data-stu-id="25164-108">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="25164-109">权限</span><span class="sxs-lookup"><span data-stu-id="25164-109">Permissions</span></span>
<span data-ttu-id="25164-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25164-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25164-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="25164-112">Permission type</span></span>                        | <span data-ttu-id="25164-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25164-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="25164-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25164-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="25164-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25164-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="25164-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25164-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="25164-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="25164-117">Not supported.</span></span> |
|<span data-ttu-id="25164-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="25164-118">Application</span></span>                            |<span data-ttu-id="25164-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="25164-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="25164-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25164-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="25164-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="25164-121">Request headers</span></span>

| <span data-ttu-id="25164-122">名称</span><span class="sxs-lookup"><span data-stu-id="25164-122">Name</span></span>           | <span data-ttu-id="25164-123">类型</span><span class="sxs-lookup"><span data-stu-id="25164-123">Type</span></span>    | <span data-ttu-id="25164-124">说明</span><span class="sxs-lookup"><span data-stu-id="25164-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="25164-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="25164-125">Authorization</span></span>  | <span data-ttu-id="25164-126">string</span><span class="sxs-lookup"><span data-stu-id="25164-126">string</span></span>  | <span data-ttu-id="25164-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25164-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25164-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="25164-129">Request body</span></span>

<span data-ttu-id="25164-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="25164-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="25164-131">响应</span><span class="sxs-lookup"><span data-stu-id="25164-131">Response</span></span>

<span data-ttu-id="25164-132">如果成功，返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="25164-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="25164-133">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="25164-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25164-134">示例</span><span class="sxs-lookup"><span data-stu-id="25164-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="25164-135">请求</span><span class="sxs-lookup"><span data-stu-id="25164-135">Request</span></span>
<span data-ttu-id="25164-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="25164-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a><span data-ttu-id="25164-137">响应</span><span class="sxs-lookup"><span data-stu-id="25164-137">Response</span></span>
<span data-ttu-id="25164-138">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="25164-138">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-start.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
