---
title: 删除 synchronizationJob
description: 停止同步作业, 并永久删除与之关联的所有状态。 同步帐户保留为。
localization_priority: Normal
ms.openlocfilehash: cfcce1c3a1741625d409af22e0953df0b0ac20a9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458169"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="dc779-104">删除 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="dc779-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc779-105">停止同步作业, 并永久删除与之关联的所有状态。</span><span class="sxs-lookup"><span data-stu-id="dc779-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="dc779-106">同步帐户保留为。</span><span class="sxs-lookup"><span data-stu-id="dc779-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc779-107">权限</span><span class="sxs-lookup"><span data-stu-id="dc779-107">Permissions</span></span>
<span data-ttu-id="dc779-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc779-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc779-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc779-110">Permission type</span></span>                        | <span data-ttu-id="dc779-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc779-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc779-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc779-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="dc779-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc779-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="dc779-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc779-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="dc779-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc779-115">Not supported.</span></span>  |
|<span data-ttu-id="dc779-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc779-116">Application</span></span>                            |<span data-ttu-id="dc779-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc779-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="dc779-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc779-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="dc779-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc779-119">Request headers</span></span>

| <span data-ttu-id="dc779-120">名称</span><span class="sxs-lookup"><span data-stu-id="dc779-120">Name</span></span>           | <span data-ttu-id="dc779-121">类型</span><span class="sxs-lookup"><span data-stu-id="dc779-121">Type</span></span>    | <span data-ttu-id="dc779-122">说明</span><span class="sxs-lookup"><span data-stu-id="dc779-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="dc779-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc779-123">Authorization</span></span>  | <span data-ttu-id="dc779-124">string</span><span class="sxs-lookup"><span data-stu-id="dc779-124">string</span></span>  | <span data-ttu-id="dc779-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dc779-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc779-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc779-127">Request body</span></span>

<span data-ttu-id="dc779-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dc779-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc779-129">响应</span><span class="sxs-lookup"><span data-stu-id="dc779-129">Response</span></span>

<span data-ttu-id="dc779-130">如果成功, 则返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="dc779-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="dc779-131">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dc779-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc779-132">示例</span><span class="sxs-lookup"><span data-stu-id="dc779-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dc779-133">请求</span><span class="sxs-lookup"><span data-stu-id="dc779-133">Request</span></span>
<span data-ttu-id="dc779-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="dc779-134">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dc779-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="dc779-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc779-136">C#</span><span class="sxs-lookup"><span data-stu-id="dc779-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc779-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="dc779-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc779-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="dc779-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dc779-139">响应</span><span class="sxs-lookup"><span data-stu-id="dc779-139">Response</span></span>
<span data-ttu-id="dc779-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dc779-140">The following is an example of the response.</span></span> 

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
  ]
}
-->
