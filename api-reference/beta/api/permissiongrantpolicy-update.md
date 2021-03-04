---
title: 更新 permissionGrantPolicy
description: 更新 permissionGrantPolicy 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 28e8fdd96bcbdc5b9542d42d8a24d8f5cf4e4da3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433857"
---
# <a name="update-permissiongrantpolicy"></a><span data-ttu-id="0ae45-103">更新 permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="0ae45-103">Update permissionGrantPolicy</span></span>

<span data-ttu-id="0ae45-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ae45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ae45-105">更新  [permissionGrantPolicy 的属性](../resources/permissiongrantpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="0ae45-105">Update properties of a  [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ae45-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0ae45-106">Permissions</span></span>

<span data-ttu-id="0ae45-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ae45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ae45-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ae45-109">Permission type</span></span>                        | <span data-ttu-id="0ae45-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ae45-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0ae45-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ae45-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ae45-112">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="0ae45-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="0ae45-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ae45-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ae45-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ae45-114">Not supported.</span></span> |
| <span data-ttu-id="0ae45-115">Application</span><span class="sxs-lookup"><span data-stu-id="0ae45-115">Application</span></span>                            | <span data-ttu-id="0ae45-116">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="0ae45-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ae45-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ae45-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0ae45-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ae45-118">Request headers</span></span>

| <span data-ttu-id="0ae45-119">名称</span><span class="sxs-lookup"><span data-stu-id="0ae45-119">Name</span></span>           | <span data-ttu-id="0ae45-120">说明</span><span class="sxs-lookup"><span data-stu-id="0ae45-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="0ae45-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ae45-121">Authorization</span></span>  | <span data-ttu-id="0ae45-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ae45-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0ae45-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ae45-124">Request body</span></span>

<span data-ttu-id="0ae45-125">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="0ae45-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0ae45-126">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="0ae45-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0ae45-127">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0ae45-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0ae45-128">属性</span><span class="sxs-lookup"><span data-stu-id="0ae45-128">Property</span></span>     | <span data-ttu-id="0ae45-129">类型</span><span class="sxs-lookup"><span data-stu-id="0ae45-129">Type</span></span> |<span data-ttu-id="0ae45-130">说明</span><span class="sxs-lookup"><span data-stu-id="0ae45-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0ae45-131">displayName</span><span class="sxs-lookup"><span data-stu-id="0ae45-131">displayName</span></span> | <span data-ttu-id="0ae45-132">String</span><span class="sxs-lookup"><span data-stu-id="0ae45-132">String</span></span> |<span data-ttu-id="0ae45-133">权限显示名称策略的权限。</span><span class="sxs-lookup"><span data-stu-id="0ae45-133">The display name for the permission grant policy.</span></span>|
| <span data-ttu-id="0ae45-134">说明</span><span class="sxs-lookup"><span data-stu-id="0ae45-134">description</span></span> |<span data-ttu-id="0ae45-135">String</span><span class="sxs-lookup"><span data-stu-id="0ae45-135">String</span></span>| <span data-ttu-id="0ae45-136">权限授予策略的说明。</span><span class="sxs-lookup"><span data-stu-id="0ae45-136">The description for the permission grant policy.</span></span>|

## <a name="response"></a><span data-ttu-id="0ae45-137">响应</span><span class="sxs-lookup"><span data-stu-id="0ae45-137">Response</span></span>

<span data-ttu-id="0ae45-138">如果成功，此方法将返回 `204 No Content` 响应代码，并且不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0ae45-138">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ae45-139">示例</span><span class="sxs-lookup"><span data-stu-id="0ae45-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ae45-140">请求</span><span class="sxs-lookup"><span data-stu-id="0ae45-140">Request</span></span>

<span data-ttu-id="0ae45-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0ae45-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0ae45-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ae45-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_permissiongrantpolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy
Content-Type: application/json

{
  "displayName": "Custom permission grant policy"
}
```
# <a name="c"></a>[<span data-ttu-id="0ae45-143">C#</span><span class="sxs-lookup"><span data-stu-id="0ae45-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ae45-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ae45-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ae45-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ae45-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ae45-146">Java</span><span class="sxs-lookup"><span data-stu-id="0ae45-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0ae45-147">响应</span><span class="sxs-lookup"><span data-stu-id="0ae45-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": false
} -->

```http
HTTP/1.1 204 No Content
```
