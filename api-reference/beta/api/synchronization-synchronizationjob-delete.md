---
title: 删除 synchronizationJob
description: 停止同步作业, 并永久删除与之关联的所有状态。 同步帐户保留为。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a179e8b61d6cafb63b143a392c5543b566644325
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991126"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="dd868-104">删除 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="dd868-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd868-105">停止同步作业, 并永久删除与之关联的所有状态。</span><span class="sxs-lookup"><span data-stu-id="dd868-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="dd868-106">同步帐户保留为。</span><span class="sxs-lookup"><span data-stu-id="dd868-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd868-107">权限</span><span class="sxs-lookup"><span data-stu-id="dd868-107">Permissions</span></span>
<span data-ttu-id="dd868-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd868-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd868-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd868-110">Permission type</span></span>                        | <span data-ttu-id="dd868-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd868-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd868-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd868-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="dd868-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd868-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="dd868-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd868-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="dd868-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd868-115">Not supported.</span></span>  |
|<span data-ttu-id="dd868-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd868-116">Application</span></span>                            |<span data-ttu-id="dd868-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd868-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="dd868-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd868-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="dd868-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd868-119">Request headers</span></span>

| <span data-ttu-id="dd868-120">名称</span><span class="sxs-lookup"><span data-stu-id="dd868-120">Name</span></span>           | <span data-ttu-id="dd868-121">类型</span><span class="sxs-lookup"><span data-stu-id="dd868-121">Type</span></span>    | <span data-ttu-id="dd868-122">说明</span><span class="sxs-lookup"><span data-stu-id="dd868-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="dd868-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd868-123">Authorization</span></span>  | <span data-ttu-id="dd868-124">string</span><span class="sxs-lookup"><span data-stu-id="dd868-124">string</span></span>  | <span data-ttu-id="dd868-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dd868-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd868-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd868-127">Request body</span></span>

<span data-ttu-id="dd868-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dd868-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd868-129">响应</span><span class="sxs-lookup"><span data-stu-id="dd868-129">Response</span></span>

<span data-ttu-id="dd868-130">如果成功, 则返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="dd868-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="dd868-131">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dd868-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd868-132">示例</span><span class="sxs-lookup"><span data-stu-id="dd868-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dd868-133">请求</span><span class="sxs-lookup"><span data-stu-id="dd868-133">Request</span></span>
<span data-ttu-id="dd868-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="dd868-134">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dd868-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="dd868-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dd868-136">C#</span><span class="sxs-lookup"><span data-stu-id="dd868-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd868-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="dd868-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dd868-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="dd868-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dd868-139">Java</span><span class="sxs-lookup"><span data-stu-id="dd868-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-synchronizationjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dd868-140">响应</span><span class="sxs-lookup"><span data-stu-id="dd868-140">Response</span></span>
<span data-ttu-id="dd868-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dd868-141">The following is an example of the response.</span></span> 

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
