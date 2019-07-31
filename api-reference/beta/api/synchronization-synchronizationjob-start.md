---
title: 启动 synchronizationJob
description: 启动现有的同步作业。 如果作业处于暂停状态, 它将继续处理暂停的点处的更改。 如果作业在隔离中, 隔离状态将被清除。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3d65c4c80f2369c5668d890517106b6b53c40b4a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977792"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="51274-105">启动 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="51274-105">Start synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51274-106">启动现有的同步作业。</span><span class="sxs-lookup"><span data-stu-id="51274-106">Start an existing synchronization job.</span></span> <span data-ttu-id="51274-107">如果作业处于暂停状态, 它将继续处理暂停的点处的更改。</span><span class="sxs-lookup"><span data-stu-id="51274-107">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="51274-108">如果作业在隔离中, 隔离状态将被清除。</span><span class="sxs-lookup"><span data-stu-id="51274-108">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="51274-109">权限</span><span class="sxs-lookup"><span data-stu-id="51274-109">Permissions</span></span>
<span data-ttu-id="51274-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51274-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51274-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="51274-112">Permission type</span></span>                        | <span data-ttu-id="51274-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="51274-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="51274-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51274-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="51274-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51274-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="51274-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51274-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="51274-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="51274-117">Not supported.</span></span> |
|<span data-ttu-id="51274-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="51274-118">Application</span></span>                            |<span data-ttu-id="51274-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="51274-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="51274-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51274-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="51274-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="51274-121">Request headers</span></span>

| <span data-ttu-id="51274-122">名称</span><span class="sxs-lookup"><span data-stu-id="51274-122">Name</span></span>           | <span data-ttu-id="51274-123">类型</span><span class="sxs-lookup"><span data-stu-id="51274-123">Type</span></span>    | <span data-ttu-id="51274-124">说明</span><span class="sxs-lookup"><span data-stu-id="51274-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="51274-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="51274-125">Authorization</span></span>  | <span data-ttu-id="51274-126">string</span><span class="sxs-lookup"><span data-stu-id="51274-126">string</span></span>  | <span data-ttu-id="51274-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="51274-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51274-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="51274-129">Request body</span></span>

<span data-ttu-id="51274-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="51274-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="51274-131">响应</span><span class="sxs-lookup"><span data-stu-id="51274-131">Response</span></span>

<span data-ttu-id="51274-132">如果成功, 则返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="51274-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="51274-133">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="51274-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51274-134">示例</span><span class="sxs-lookup"><span data-stu-id="51274-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="51274-135">请求</span><span class="sxs-lookup"><span data-stu-id="51274-135">Request</span></span>
<span data-ttu-id="51274-136">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="51274-136">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="51274-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="51274-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="51274-138">C#</span><span class="sxs-lookup"><span data-stu-id="51274-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51274-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="51274-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="51274-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="51274-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="51274-141">Java</span><span class="sxs-lookup"><span data-stu-id="51274-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="51274-142">响应</span><span class="sxs-lookup"><span data-stu-id="51274-142">Response</span></span>
<span data-ttu-id="51274-143">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="51274-143">The following is an example of a response.</span></span>
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
  ]
}
-->
