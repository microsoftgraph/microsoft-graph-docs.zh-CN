---
title: 从包含 permissionGrantPolicy 的集合中删除 permissionGrantConditionSet
description: 从权限授予策略中删除包含的条件集。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 4fb9fb913698bcee6c788c3a6cbbd22eaf7db6c5
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433540"
---
# <a name="delete-permissiongrantconditionset-from-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="cf1b9-103">从包含 permissionGrantPolicy 的集合中删除 permissionGrantConditionSet</span><span class="sxs-lookup"><span data-stu-id="cf1b9-103">Delete permissionGrantConditionSet from includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="cf1b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf1b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf1b9-105">从**包含** [permissionGrantPolicy](../resources/permissiongrantpolicy.md)集合中删除一个[permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 。</span><span class="sxs-lookup"><span data-stu-id="cf1b9-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **includes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf1b9-106">权限</span><span class="sxs-lookup"><span data-stu-id="cf1b9-106">Permissions</span></span>

<span data-ttu-id="cf1b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf1b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf1b9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf1b9-109">Permission type</span></span>      | <span data-ttu-id="cf1b9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf1b9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="cf1b9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf1b9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cf1b9-112">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="cf1b9-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="cf1b9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf1b9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf1b9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf1b9-114">Not supported.</span></span>    |
| <span data-ttu-id="cf1b9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf1b9-115">Application</span></span> | <span data-ttu-id="cf1b9-116">PermissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="cf1b9-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf1b9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf1b9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/includes/{include-id}
```

## <a name="request-headers"></a><span data-ttu-id="cf1b9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf1b9-118">Request headers</span></span>

| <span data-ttu-id="cf1b9-119">名称</span><span class="sxs-lookup"><span data-stu-id="cf1b9-119">Name</span></span>       | <span data-ttu-id="cf1b9-120">类型</span><span class="sxs-lookup"><span data-stu-id="cf1b9-120">Type</span></span> | <span data-ttu-id="cf1b9-121">说明</span><span class="sxs-lookup"><span data-stu-id="cf1b9-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cf1b9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf1b9-122">Authorization</span></span>  | <span data-ttu-id="cf1b9-123">string</span><span class="sxs-lookup"><span data-stu-id="cf1b9-123">string</span></span>  | <span data-ttu-id="cf1b9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf1b9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf1b9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf1b9-126">Request body</span></span>

<span data-ttu-id="cf1b9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf1b9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf1b9-128">响应</span><span class="sxs-lookup"><span data-stu-id="cf1b9-128">Response</span></span>

<span data-ttu-id="cf1b9-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cf1b9-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cf1b9-131">示例</span><span class="sxs-lookup"><span data-stu-id="cf1b9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cf1b9-132">请求</span><span class="sxs-lookup"><span data-stu-id="cf1b9-132">Request</span></span>

<span data-ttu-id="cf1b9-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cf1b9-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_includes"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy/includes/198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5
```

### <a name="response"></a><span data-ttu-id="cf1b9-134">响应</span><span class="sxs-lookup"><span data-stu-id="cf1b9-134">Response</span></span>

<span data-ttu-id="cf1b9-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cf1b9-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
