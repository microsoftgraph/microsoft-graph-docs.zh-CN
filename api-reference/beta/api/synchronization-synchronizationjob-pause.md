---
title: synchronizationJob： 暂停
description: 暂时停止同步。 所有的进度，包括作业状态保持不变，且该作业将继续从停止时开始调用的地方。
localization_priority: Normal
ms.openlocfilehash: 9f8cac05511b5efd17234ccf16b763999418bf2a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513919"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="8df83-104">synchronizationJob： 暂停</span><span class="sxs-lookup"><span data-stu-id="8df83-104">synchronizationJob: pause</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8df83-105">暂时停止同步。</span><span class="sxs-lookup"><span data-stu-id="8df83-105">Temporarily stop synchronization.</span></span> <span data-ttu-id="8df83-106">所有的进度，包括作业状态保持不变，且该作业将继续从停止时[启动](../api/synchronization-synchronizationjob-start.md)调用的地方。</span><span class="sxs-lookup"><span data-stu-id="8df83-106">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="8df83-107">权限</span><span class="sxs-lookup"><span data-stu-id="8df83-107">Permissions</span></span>
<span data-ttu-id="8df83-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8df83-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8df83-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8df83-110">Permission type</span></span>                        | <span data-ttu-id="8df83-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8df83-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8df83-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8df83-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="8df83-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8df83-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="8df83-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8df83-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="8df83-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8df83-115">Not supported.</span></span>  |
|<span data-ttu-id="8df83-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8df83-116">Application</span></span>                            |<span data-ttu-id="8df83-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8df83-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8df83-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8df83-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="8df83-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8df83-119">Request headers</span></span>

| <span data-ttu-id="8df83-120">名称</span><span class="sxs-lookup"><span data-stu-id="8df83-120">Name</span></span>           | <span data-ttu-id="8df83-121">类型</span><span class="sxs-lookup"><span data-stu-id="8df83-121">Type</span></span>    | <span data-ttu-id="8df83-122">说明</span><span class="sxs-lookup"><span data-stu-id="8df83-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="8df83-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8df83-123">Authorization</span></span>  | <span data-ttu-id="8df83-124">string</span><span class="sxs-lookup"><span data-stu-id="8df83-124">string</span></span>  | <span data-ttu-id="8df83-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8df83-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8df83-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8df83-127">Request body</span></span>

<span data-ttu-id="8df83-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8df83-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8df83-129">响应</span><span class="sxs-lookup"><span data-stu-id="8df83-129">Response</span></span>

<span data-ttu-id="8df83-130">如果成功，返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="8df83-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="8df83-131">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="8df83-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8df83-132">示例</span><span class="sxs-lookup"><span data-stu-id="8df83-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8df83-133">请求</span><span class="sxs-lookup"><span data-stu-id="8df83-133">Request</span></span>
<span data-ttu-id="8df83-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8df83-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="8df83-135">响应</span><span class="sxs-lookup"><span data-stu-id="8df83-135">Response</span></span>
<span data-ttu-id="8df83-136">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="8df83-136">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: pause",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-pause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
