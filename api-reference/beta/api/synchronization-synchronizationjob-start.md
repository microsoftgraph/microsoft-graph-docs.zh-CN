---
title: 启动 synchronizationJob
description: 启动现有的同步作业。 如果作业处于暂停状态, 它将继续处理暂停的点处的更改。 如果作业在隔离中, 隔离状态将被清除。
localization_priority: Normal
ms.openlocfilehash: 4648d9d3d889adf2cd7ec06e4fcf79b761c77132
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545264"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="c5044-105">启动 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="c5044-105">Start synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5044-106">启动现有的同步作业。</span><span class="sxs-lookup"><span data-stu-id="c5044-106">Start an existing synchronization job.</span></span> <span data-ttu-id="c5044-107">如果作业处于暂停状态, 它将继续处理暂停的点处的更改。</span><span class="sxs-lookup"><span data-stu-id="c5044-107">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="c5044-108">如果作业在隔离中, 隔离状态将被清除。</span><span class="sxs-lookup"><span data-stu-id="c5044-108">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5044-109">权限</span><span class="sxs-lookup"><span data-stu-id="c5044-109">Permissions</span></span>
<span data-ttu-id="c5044-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5044-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5044-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5044-112">Permission type</span></span>                        | <span data-ttu-id="c5044-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5044-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5044-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5044-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="c5044-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5044-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c5044-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5044-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c5044-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5044-117">Not supported.</span></span> |
|<span data-ttu-id="c5044-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5044-118">Application</span></span>                            |<span data-ttu-id="c5044-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5044-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c5044-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5044-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="c5044-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5044-121">Request headers</span></span>

| <span data-ttu-id="c5044-122">名称</span><span class="sxs-lookup"><span data-stu-id="c5044-122">Name</span></span>           | <span data-ttu-id="c5044-123">类型</span><span class="sxs-lookup"><span data-stu-id="c5044-123">Type</span></span>    | <span data-ttu-id="c5044-124">说明</span><span class="sxs-lookup"><span data-stu-id="c5044-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c5044-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5044-125">Authorization</span></span>  | <span data-ttu-id="c5044-126">string</span><span class="sxs-lookup"><span data-stu-id="c5044-126">string</span></span>  | <span data-ttu-id="c5044-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5044-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5044-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5044-129">Request body</span></span>

<span data-ttu-id="c5044-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5044-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="c5044-131">响应</span><span class="sxs-lookup"><span data-stu-id="c5044-131">Response</span></span>

<span data-ttu-id="c5044-132">如果成功, 则返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="c5044-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="c5044-133">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c5044-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5044-134">示例</span><span class="sxs-lookup"><span data-stu-id="c5044-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c5044-135">请求</span><span class="sxs-lookup"><span data-stu-id="c5044-135">Request</span></span>
<span data-ttu-id="c5044-136">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="c5044-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a><span data-ttu-id="c5044-137">响应</span><span class="sxs-lookup"><span data-stu-id="c5044-137">Response</span></span>
<span data-ttu-id="c5044-138">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="c5044-138">The following is an example of a response.</span></span>
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
