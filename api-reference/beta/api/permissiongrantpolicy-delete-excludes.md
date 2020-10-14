---
title: 删除 permissionGrantPolicy 的排除集合中的 permissionGrantConditionSet
description: 从权限授予策略中删除已排除的条件集。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 84a0b1eae5d4800a50ddc9e258690228f971fad4
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460328"
---
# <a name="delete-permissiongrantconditionset-from-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="1c815-103">删除 permissionGrantPolicy 的排除集合中的 permissionGrantConditionSet</span><span class="sxs-lookup"><span data-stu-id="1c815-103">Delete permissionGrantConditionSet from excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="1c815-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c815-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c815-105">从[permissionGrantPolicy](../resources/permissiongrantpolicy.md)的 "**排除**" 集合中删除[permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 。</span><span class="sxs-lookup"><span data-stu-id="1c815-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **excludes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c815-106">权限</span><span class="sxs-lookup"><span data-stu-id="1c815-106">Permissions</span></span>

<span data-ttu-id="1c815-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c815-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c815-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c815-109">Permission type</span></span>      | <span data-ttu-id="1c815-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c815-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="1c815-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c815-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1c815-112">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="1c815-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="1c815-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c815-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c815-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c815-114">Not supported.</span></span>    |
| <span data-ttu-id="1c815-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c815-115">Application</span></span> | <span data-ttu-id="1c815-116">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="1c815-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c815-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c815-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/excludes/{exclude-id}
```

## <a name="request-headers"></a><span data-ttu-id="1c815-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c815-118">Request headers</span></span>

| <span data-ttu-id="1c815-119">名称</span><span class="sxs-lookup"><span data-stu-id="1c815-119">Name</span></span>       | <span data-ttu-id="1c815-120">类型</span><span class="sxs-lookup"><span data-stu-id="1c815-120">Type</span></span> | <span data-ttu-id="1c815-121">说明</span><span class="sxs-lookup"><span data-stu-id="1c815-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1c815-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c815-122">Authorization</span></span>  | <span data-ttu-id="1c815-123">string</span><span class="sxs-lookup"><span data-stu-id="1c815-123">string</span></span>  | <span data-ttu-id="1c815-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c815-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c815-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c815-126">Request body</span></span>

<span data-ttu-id="1c815-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1c815-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c815-128">响应</span><span class="sxs-lookup"><span data-stu-id="1c815-128">Response</span></span>

<span data-ttu-id="1c815-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1c815-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c815-131">示例</span><span class="sxs-lookup"><span data-stu-id="1c815-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1c815-132">请求</span><span class="sxs-lookup"><span data-stu-id="1c815-132">Request</span></span>

<span data-ttu-id="1c815-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1c815-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1c815-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c815-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_excludes"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy/excludes/6a846635-3e70-4a10-821e-512a0db93cbd
```
# <a name="c"></a>[<span data-ttu-id="1c815-135">C#</span><span class="sxs-lookup"><span data-stu-id="1c815-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-delete-excludes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c815-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c815-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-delete-excludes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c815-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c815-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-delete-excludes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1c815-138">响应</span><span class="sxs-lookup"><span data-stu-id="1c815-138">Response</span></span>

<span data-ttu-id="1c815-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1c815-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
