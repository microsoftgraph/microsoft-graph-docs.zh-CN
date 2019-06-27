---
title: 启动 synchronizationJob
description: 启动现有的同步作业。 如果作业处于暂停状态, 它将继续处理暂停的点处的更改。 如果作业在隔离中, 隔离状态将被清除。
localization_priority: Normal
ms.openlocfilehash: 6681096b66c5ac47cef4e18dbf606148cd637b40
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271328"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="3b78e-105">启动 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="3b78e-105">Start synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b78e-106">启动现有的同步作业。</span><span class="sxs-lookup"><span data-stu-id="3b78e-106">Start an existing synchronization job.</span></span> <span data-ttu-id="3b78e-107">如果作业处于暂停状态, 它将继续处理暂停的点处的更改。</span><span class="sxs-lookup"><span data-stu-id="3b78e-107">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="3b78e-108">如果作业在隔离中, 隔离状态将被清除。</span><span class="sxs-lookup"><span data-stu-id="3b78e-108">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b78e-109">权限</span><span class="sxs-lookup"><span data-stu-id="3b78e-109">Permissions</span></span>
<span data-ttu-id="3b78e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b78e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b78e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b78e-112">Permission type</span></span>                        | <span data-ttu-id="3b78e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b78e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b78e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b78e-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="3b78e-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b78e-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3b78e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b78e-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3b78e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b78e-117">Not supported.</span></span> |
|<span data-ttu-id="3b78e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b78e-118">Application</span></span>                            |<span data-ttu-id="3b78e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b78e-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3b78e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b78e-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="3b78e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b78e-121">Request headers</span></span>

| <span data-ttu-id="3b78e-122">名称</span><span class="sxs-lookup"><span data-stu-id="3b78e-122">Name</span></span>           | <span data-ttu-id="3b78e-123">类型</span><span class="sxs-lookup"><span data-stu-id="3b78e-123">Type</span></span>    | <span data-ttu-id="3b78e-124">说明</span><span class="sxs-lookup"><span data-stu-id="3b78e-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="3b78e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b78e-125">Authorization</span></span>  | <span data-ttu-id="3b78e-126">string</span><span class="sxs-lookup"><span data-stu-id="3b78e-126">string</span></span>  | <span data-ttu-id="3b78e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3b78e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b78e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b78e-129">Request body</span></span>

<span data-ttu-id="3b78e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3b78e-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="3b78e-131">响应</span><span class="sxs-lookup"><span data-stu-id="3b78e-131">Response</span></span>

<span data-ttu-id="3b78e-132">如果成功, 则返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="3b78e-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="3b78e-133">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3b78e-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b78e-134">示例</span><span class="sxs-lookup"><span data-stu-id="3b78e-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3b78e-135">请求</span><span class="sxs-lookup"><span data-stu-id="3b78e-135">Request</span></span>
<span data-ttu-id="3b78e-136">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="3b78e-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a><span data-ttu-id="3b78e-137">响应</span><span class="sxs-lookup"><span data-stu-id="3b78e-137">Response</span></span>
<span data-ttu-id="3b78e-138">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="3b78e-138">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3b78e-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3b78e-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3b78e-140">C#</span><span class="sxs-lookup"><span data-stu-id="3b78e-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationjob_start-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3b78e-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="3b78e-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationjob_start-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3b78e-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="3b78e-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/synchronizationjob_start-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-start.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-start.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-start.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
