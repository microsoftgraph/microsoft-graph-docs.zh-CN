---
title: 删除 synchronizationJob
description: 停止同步作业，并永久删除与之关联的所有状态。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd732200b8ab02be3bffc443272a45f2da8a9a77
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466432"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="b5c88-103">删除 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="b5c88-103">Delete synchronizationJob</span></span>

<span data-ttu-id="b5c88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5c88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5c88-105">停止同步作业，并永久删除与之关联的所有状态。</span><span class="sxs-lookup"><span data-stu-id="b5c88-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="b5c88-106">同步帐户保留为。</span><span class="sxs-lookup"><span data-stu-id="b5c88-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5c88-107">权限</span><span class="sxs-lookup"><span data-stu-id="b5c88-107">Permissions</span></span>
<span data-ttu-id="b5c88-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5c88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5c88-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5c88-110">Permission type</span></span>                        | <span data-ttu-id="b5c88-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5c88-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5c88-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5c88-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="b5c88-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5c88-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b5c88-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5c88-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b5c88-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5c88-115">Not supported.</span></span>  |
|<span data-ttu-id="b5c88-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5c88-116">Application</span></span>                            |<span data-ttu-id="b5c88-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5c88-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b5c88-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5c88-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="b5c88-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5c88-119">Request headers</span></span>

| <span data-ttu-id="b5c88-120">名称</span><span class="sxs-lookup"><span data-stu-id="b5c88-120">Name</span></span>           | <span data-ttu-id="b5c88-121">类型</span><span class="sxs-lookup"><span data-stu-id="b5c88-121">Type</span></span>    | <span data-ttu-id="b5c88-122">说明</span><span class="sxs-lookup"><span data-stu-id="b5c88-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b5c88-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5c88-123">Authorization</span></span>  | <span data-ttu-id="b5c88-124">string</span><span class="sxs-lookup"><span data-stu-id="b5c88-124">string</span></span>  | <span data-ttu-id="b5c88-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5c88-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5c88-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5c88-127">Request body</span></span>

<span data-ttu-id="b5c88-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5c88-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5c88-129">响应</span><span class="sxs-lookup"><span data-stu-id="b5c88-129">Response</span></span>

<span data-ttu-id="b5c88-130">如果成功，则返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="b5c88-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="b5c88-131">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b5c88-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5c88-132">示例</span><span class="sxs-lookup"><span data-stu-id="b5c88-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b5c88-133">请求</span><span class="sxs-lookup"><span data-stu-id="b5c88-133">Request</span></span>
<span data-ttu-id="b5c88-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="b5c88-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5c88-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5c88-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="b5c88-136">C#</span><span class="sxs-lookup"><span data-stu-id="b5c88-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5c88-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5c88-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5c88-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5c88-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b5c88-139">响应</span><span class="sxs-lookup"><span data-stu-id="b5c88-139">Response</span></span>
<span data-ttu-id="b5c88-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b5c88-140">The following is an example of the response.</span></span> 

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
