---
title: 删除 synchronizationJob
description: 停止同步作业，并永久删除与之关联的所有状态。 同步帐户保留为。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2c346b1020250cb1e46aa9f3c2b57f9fd5b1f1ae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453021"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="3cb4d-104">删除 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="3cb4d-104">Delete synchronizationJob</span></span>

<span data-ttu-id="3cb4d-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3cb4d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cb4d-106">停止同步作业，并永久删除与之关联的所有状态。</span><span class="sxs-lookup"><span data-stu-id="3cb4d-106">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="3cb4d-107">同步帐户保留为。</span><span class="sxs-lookup"><span data-stu-id="3cb4d-107">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cb4d-108">权限</span><span class="sxs-lookup"><span data-stu-id="3cb4d-108">Permissions</span></span>
<span data-ttu-id="3cb4d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cb4d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cb4d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cb4d-111">Permission type</span></span>                        | <span data-ttu-id="3cb4d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cb4d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cb4d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cb4d-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="3cb4d-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cb4d-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3cb4d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cb4d-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3cb4d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cb4d-116">Not supported.</span></span>  |
|<span data-ttu-id="3cb4d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cb4d-117">Application</span></span>                            |<span data-ttu-id="3cb4d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cb4d-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3cb4d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cb4d-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="3cb4d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cb4d-120">Request headers</span></span>

| <span data-ttu-id="3cb4d-121">名称</span><span class="sxs-lookup"><span data-stu-id="3cb4d-121">Name</span></span>           | <span data-ttu-id="3cb4d-122">类型</span><span class="sxs-lookup"><span data-stu-id="3cb4d-122">Type</span></span>    | <span data-ttu-id="3cb4d-123">说明</span><span class="sxs-lookup"><span data-stu-id="3cb4d-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="3cb4d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cb4d-124">Authorization</span></span>  | <span data-ttu-id="3cb4d-125">string</span><span class="sxs-lookup"><span data-stu-id="3cb4d-125">string</span></span>  | <span data-ttu-id="3cb4d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3cb4d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cb4d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cb4d-128">Request body</span></span>

<span data-ttu-id="3cb4d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3cb4d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cb4d-130">响应</span><span class="sxs-lookup"><span data-stu-id="3cb4d-130">Response</span></span>

<span data-ttu-id="3cb4d-131">如果成功，则返回`204 No Content`响应。</span><span class="sxs-lookup"><span data-stu-id="3cb4d-131">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="3cb4d-132">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3cb4d-132">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cb4d-133">示例</span><span class="sxs-lookup"><span data-stu-id="3cb4d-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3cb4d-134">请求</span><span class="sxs-lookup"><span data-stu-id="3cb4d-134">Request</span></span>
<span data-ttu-id="3cb4d-135">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="3cb4d-135">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3cb4d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cb4d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="3cb4d-137">C#</span><span class="sxs-lookup"><span data-stu-id="3cb4d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cb4d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cb4d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cb4d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cb4d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3cb4d-140">响应</span><span class="sxs-lookup"><span data-stu-id="3cb4d-140">Response</span></span>
<span data-ttu-id="3cb4d-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3cb4d-141">The following is an example of the response.</span></span> 

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
