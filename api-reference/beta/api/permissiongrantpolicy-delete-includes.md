---
title: 从包含 permissionGrantPolicy 的集合中删除 permissionGrantConditionSet
description: 从权限授予策略中删除包含的条件集。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 803890aaee2e8ad12bee88fb844f3529fce258e6
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460288"
---
# <a name="delete-permissiongrantconditionset-from-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="fbf0e-103">从包含 permissionGrantPolicy 的集合中删除 permissionGrantConditionSet</span><span class="sxs-lookup"><span data-stu-id="fbf0e-103">Delete permissionGrantConditionSet from includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="fbf0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbf0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbf0e-105">从**包含** [permissionGrantPolicy](../resources/permissiongrantpolicy.md)集合中删除一个[permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 。</span><span class="sxs-lookup"><span data-stu-id="fbf0e-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **includes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fbf0e-106">权限</span><span class="sxs-lookup"><span data-stu-id="fbf0e-106">Permissions</span></span>

<span data-ttu-id="fbf0e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fbf0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fbf0e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fbf0e-109">Permission type</span></span>      | <span data-ttu-id="fbf0e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fbf0e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="fbf0e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fbf0e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fbf0e-112">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="fbf0e-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="fbf0e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fbf0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbf0e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbf0e-114">Not supported.</span></span>    |
| <span data-ttu-id="fbf0e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fbf0e-115">Application</span></span> | <span data-ttu-id="fbf0e-116">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="fbf0e-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbf0e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fbf0e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/includes/{include-id}
```

## <a name="request-headers"></a><span data-ttu-id="fbf0e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fbf0e-118">Request headers</span></span>

| <span data-ttu-id="fbf0e-119">名称</span><span class="sxs-lookup"><span data-stu-id="fbf0e-119">Name</span></span>       | <span data-ttu-id="fbf0e-120">类型</span><span class="sxs-lookup"><span data-stu-id="fbf0e-120">Type</span></span> | <span data-ttu-id="fbf0e-121">说明</span><span class="sxs-lookup"><span data-stu-id="fbf0e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fbf0e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbf0e-122">Authorization</span></span>  | <span data-ttu-id="fbf0e-123">string</span><span class="sxs-lookup"><span data-stu-id="fbf0e-123">string</span></span>  | <span data-ttu-id="fbf0e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fbf0e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbf0e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fbf0e-126">Request body</span></span>

<span data-ttu-id="fbf0e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fbf0e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbf0e-128">响应</span><span class="sxs-lookup"><span data-stu-id="fbf0e-128">Response</span></span>

<span data-ttu-id="fbf0e-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fbf0e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fbf0e-131">示例</span><span class="sxs-lookup"><span data-stu-id="fbf0e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fbf0e-132">请求</span><span class="sxs-lookup"><span data-stu-id="fbf0e-132">Request</span></span>

<span data-ttu-id="fbf0e-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fbf0e-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fbf0e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbf0e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_includes"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy/includes/198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5
```
# <a name="c"></a>[<span data-ttu-id="fbf0e-135">C#</span><span class="sxs-lookup"><span data-stu-id="fbf0e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-delete-includes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fbf0e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbf0e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-delete-includes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fbf0e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbf0e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-delete-includes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fbf0e-138">响应</span><span class="sxs-lookup"><span data-stu-id="fbf0e-138">Response</span></span>

<span data-ttu-id="fbf0e-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fbf0e-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
