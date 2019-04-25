---
title: 'synchronizationJob: pause'
description: 临时停止同步。 所有进度 (包括作业状态) 均保持不变, 作业将从开始调用时停止的位置继续。
localization_priority: Normal
ms.openlocfilehash: 9f8cac05511b5efd17234ccf16b763999418bf2a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537168"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="46216-104">synchronizationJob: pause</span><span class="sxs-lookup"><span data-stu-id="46216-104">synchronizationJob: pause</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46216-105">临时停止同步。</span><span class="sxs-lookup"><span data-stu-id="46216-105">Temporarily stop synchronization.</span></span> <span data-ttu-id="46216-106">所有进度 (包括作业状态) 均保持不变, 作业将从[开始](../api/synchronization-synchronizationjob-start.md)调用时停止的位置继续。</span><span class="sxs-lookup"><span data-stu-id="46216-106">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="46216-107">权限</span><span class="sxs-lookup"><span data-stu-id="46216-107">Permissions</span></span>
<span data-ttu-id="46216-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46216-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46216-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="46216-110">Permission type</span></span>                        | <span data-ttu-id="46216-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46216-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="46216-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46216-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="46216-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46216-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="46216-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46216-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="46216-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="46216-115">Not supported.</span></span>  |
|<span data-ttu-id="46216-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="46216-116">Application</span></span>                            |<span data-ttu-id="46216-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="46216-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="46216-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46216-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="46216-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="46216-119">Request headers</span></span>

| <span data-ttu-id="46216-120">名称</span><span class="sxs-lookup"><span data-stu-id="46216-120">Name</span></span>           | <span data-ttu-id="46216-121">类型</span><span class="sxs-lookup"><span data-stu-id="46216-121">Type</span></span>    | <span data-ttu-id="46216-122">说明</span><span class="sxs-lookup"><span data-stu-id="46216-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="46216-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="46216-123">Authorization</span></span>  | <span data-ttu-id="46216-124">string</span><span class="sxs-lookup"><span data-stu-id="46216-124">string</span></span>  | <span data-ttu-id="46216-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46216-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46216-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="46216-127">Request body</span></span>

<span data-ttu-id="46216-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="46216-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46216-129">响应</span><span class="sxs-lookup"><span data-stu-id="46216-129">Response</span></span>

<span data-ttu-id="46216-130">如果成功, 则返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="46216-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="46216-131">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="46216-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46216-132">示例</span><span class="sxs-lookup"><span data-stu-id="46216-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="46216-133">请求</span><span class="sxs-lookup"><span data-stu-id="46216-133">Request</span></span>
<span data-ttu-id="46216-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="46216-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="46216-135">响应</span><span class="sxs-lookup"><span data-stu-id="46216-135">Response</span></span>
<span data-ttu-id="46216-136">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="46216-136">The following is an example of a response.</span></span>
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
