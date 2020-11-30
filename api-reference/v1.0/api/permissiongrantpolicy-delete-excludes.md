---
title: 删除 permissionGrantPolicy 的排除集合中的 permissionGrantConditionSet
description: 从权限授予策略中删除已排除的条件集。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 981693c50cfc2784cdb48a6eeecf00cab1910123
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377203"
---
# <a name="delete-permissiongrantconditionset-from-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="d9a88-103">删除 permissionGrantPolicy 的排除集合中的 permissionGrantConditionSet</span><span class="sxs-lookup"><span data-stu-id="d9a88-103">Delete permissionGrantConditionSet from excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="d9a88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9a88-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9a88-105">从 [permissionGrantPolicy](../resources/permissiongrantpolicy.md)的 "**排除**" 集合中删除 [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 。</span><span class="sxs-lookup"><span data-stu-id="d9a88-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **excludes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d9a88-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d9a88-106">Permissions</span></span>

<span data-ttu-id="d9a88-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9a88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9a88-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9a88-109">Permission type</span></span>      | <span data-ttu-id="d9a88-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9a88-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="d9a88-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9a88-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d9a88-112">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="d9a88-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="d9a88-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9a88-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9a88-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9a88-114">Not supported.</span></span>    |
| <span data-ttu-id="d9a88-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9a88-115">Application</span></span> | <span data-ttu-id="d9a88-116">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="d9a88-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9a88-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9a88-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/excludes/{exclude-id}
```

## <a name="request-headers"></a><span data-ttu-id="d9a88-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9a88-118">Request headers</span></span>

| <span data-ttu-id="d9a88-119">名称</span><span class="sxs-lookup"><span data-stu-id="d9a88-119">Name</span></span>       | <span data-ttu-id="d9a88-120">类型</span><span class="sxs-lookup"><span data-stu-id="d9a88-120">Type</span></span> | <span data-ttu-id="d9a88-121">说明</span><span class="sxs-lookup"><span data-stu-id="d9a88-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d9a88-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9a88-122">Authorization</span></span>  | <span data-ttu-id="d9a88-123">string</span><span class="sxs-lookup"><span data-stu-id="d9a88-123">string</span></span>  | <span data-ttu-id="d9a88-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d9a88-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9a88-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9a88-126">Request body</span></span>

<span data-ttu-id="d9a88-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d9a88-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9a88-128">响应</span><span class="sxs-lookup"><span data-stu-id="d9a88-128">Response</span></span>

<span data-ttu-id="d9a88-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d9a88-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9a88-131">示例</span><span class="sxs-lookup"><span data-stu-id="d9a88-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9a88-132">请求</span><span class="sxs-lookup"><span data-stu-id="d9a88-132">Request</span></span>

<span data-ttu-id="d9a88-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d9a88-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_excludes"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy/excludes/6a846635-3e70-4a10-821e-512a0db93cbd
```

### <a name="response"></a><span data-ttu-id="d9a88-134">响应</span><span class="sxs-lookup"><span data-stu-id="d9a88-134">Response</span></span>

<span data-ttu-id="d9a88-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d9a88-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
