---
title: 从包含 permissionGrantPolicy 的集合中删除 permissionGrantConditionSet
description: 从权限授予策略中删除包含的条件集。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 077d501146efd7325dc6e543ffd718bec81680f8
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522193"
---
# <a name="delete-permissiongrantconditionset-from-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="bfe43-103">从包含 permissionGrantPolicy 的集合中删除 permissionGrantConditionSet</span><span class="sxs-lookup"><span data-stu-id="bfe43-103">Delete permissionGrantConditionSet from includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="bfe43-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfe43-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bfe43-105">从 **包含** [permissionGrantPolicy](../resources/permissiongrantpolicy.md)集合中删除一个 [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 。</span><span class="sxs-lookup"><span data-stu-id="bfe43-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **includes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bfe43-106">权限</span><span class="sxs-lookup"><span data-stu-id="bfe43-106">Permissions</span></span>

<span data-ttu-id="bfe43-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bfe43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bfe43-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfe43-109">Permission type</span></span>      | <span data-ttu-id="bfe43-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bfe43-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="bfe43-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfe43-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bfe43-112">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="bfe43-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="bfe43-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfe43-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfe43-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfe43-114">Not supported.</span></span>    |
| <span data-ttu-id="bfe43-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfe43-115">Application</span></span> | <span data-ttu-id="bfe43-116">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="bfe43-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfe43-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfe43-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/includes/{include-id}
```

## <a name="request-headers"></a><span data-ttu-id="bfe43-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfe43-118">Request headers</span></span>

| <span data-ttu-id="bfe43-119">名称</span><span class="sxs-lookup"><span data-stu-id="bfe43-119">Name</span></span>       | <span data-ttu-id="bfe43-120">类型</span><span class="sxs-lookup"><span data-stu-id="bfe43-120">Type</span></span> | <span data-ttu-id="bfe43-121">说明</span><span class="sxs-lookup"><span data-stu-id="bfe43-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bfe43-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfe43-122">Authorization</span></span>  | <span data-ttu-id="bfe43-123">string</span><span class="sxs-lookup"><span data-stu-id="bfe43-123">string</span></span>  | <span data-ttu-id="bfe43-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bfe43-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfe43-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfe43-126">Request body</span></span>

<span data-ttu-id="bfe43-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bfe43-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfe43-128">响应</span><span class="sxs-lookup"><span data-stu-id="bfe43-128">Response</span></span>

<span data-ttu-id="bfe43-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bfe43-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bfe43-131">示例</span><span class="sxs-lookup"><span data-stu-id="bfe43-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bfe43-132">请求</span><span class="sxs-lookup"><span data-stu-id="bfe43-132">Request</span></span>

<span data-ttu-id="bfe43-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bfe43-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bfe43-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfe43-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_includes"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy/includes/198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5
```
# <a name="c"></a>[<span data-ttu-id="bfe43-135">C#</span><span class="sxs-lookup"><span data-stu-id="bfe43-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-delete-includes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfe43-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfe43-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-delete-includes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfe43-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfe43-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-delete-includes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfe43-138">Java</span><span class="sxs-lookup"><span data-stu-id="bfe43-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-delete-includes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bfe43-139">响应</span><span class="sxs-lookup"><span data-stu-id="bfe43-139">Response</span></span>

<span data-ttu-id="bfe43-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bfe43-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
