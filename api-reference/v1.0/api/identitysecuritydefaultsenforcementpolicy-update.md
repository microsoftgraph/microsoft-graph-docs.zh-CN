---
title: 更新 identitySecurityDefaultsEnforcementPolicy
description: 更新 identitySecurityDefaultsEnforcementPolicy 对象的属性。
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 95d18774bbed04a8559c5c607f76233e12c5afd5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033396"
---
# <a name="update-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="80b8f-103">更新 identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="80b8f-103">Update identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="80b8f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80b8f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="80b8f-105">更新 [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="80b8f-105">Update the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="80b8f-106">权限</span><span class="sxs-lookup"><span data-stu-id="80b8f-106">Permissions</span></span>

<span data-ttu-id="80b8f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80b8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="80b8f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="80b8f-109">Permission type</span></span>                        | <span data-ttu-id="80b8f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80b8f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="80b8f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80b8f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="80b8f-112">Policy。 Read. All 和 ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="80b8f-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="80b8f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80b8f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80b8f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="80b8f-114">Not supported.</span></span> |
| <span data-ttu-id="80b8f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="80b8f-115">Application</span></span>                            | <span data-ttu-id="80b8f-116">Policy。 Read. All 和 ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="80b8f-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="80b8f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80b8f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="request-headers"></a><span data-ttu-id="80b8f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="80b8f-118">Request headers</span></span>

| <span data-ttu-id="80b8f-119">名称</span><span class="sxs-lookup"><span data-stu-id="80b8f-119">Name</span></span>       | <span data-ttu-id="80b8f-120">说明</span><span class="sxs-lookup"><span data-stu-id="80b8f-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="80b8f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="80b8f-121">Authorization</span></span> | <span data-ttu-id="80b8f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80b8f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="80b8f-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="80b8f-124">Content-type</span></span> | <span data-ttu-id="80b8f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="80b8f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80b8f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="80b8f-127">Request body</span></span>

<span data-ttu-id="80b8f-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="80b8f-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="80b8f-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="80b8f-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="80b8f-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="80b8f-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="80b8f-131">属性</span><span class="sxs-lookup"><span data-stu-id="80b8f-131">Property</span></span>     | <span data-ttu-id="80b8f-132">类型</span><span class="sxs-lookup"><span data-stu-id="80b8f-132">Type</span></span>        | <span data-ttu-id="80b8f-133">说明</span><span class="sxs-lookup"><span data-stu-id="80b8f-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="80b8f-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="80b8f-134">isEnabled</span></span>|<span data-ttu-id="80b8f-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="80b8f-135">Boolean</span></span>|<span data-ttu-id="80b8f-136">如果设置为 true，则会为租户启用 Azure Active Directory 安全性默认设置。</span><span class="sxs-lookup"><span data-stu-id="80b8f-136">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="response"></a><span data-ttu-id="80b8f-137">响应</span><span class="sxs-lookup"><span data-stu-id="80b8f-137">Response</span></span>

<span data-ttu-id="80b8f-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="80b8f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="80b8f-140">示例</span><span class="sxs-lookup"><span data-stu-id="80b8f-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="80b8f-141">请求</span><span class="sxs-lookup"><span data-stu-id="80b8f-141">Request</span></span>

<span data-ttu-id="80b8f-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="80b8f-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="80b8f-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="80b8f-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identitysecuritydefaultsenforcementpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/identitySecurityDefaultsEnforcementPolicy
Content-type: application/json

{
  "isEnabled": false
}
```
# <a name="c"></a>[<span data-ttu-id="80b8f-144">C#</span><span class="sxs-lookup"><span data-stu-id="80b8f-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identitysecuritydefaultsenforcementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80b8f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80b8f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identitysecuritydefaultsenforcementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80b8f-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80b8f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identitysecuritydefaultsenforcementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80b8f-147">Java</span><span class="sxs-lookup"><span data-stu-id="80b8f-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identitysecuritydefaultsenforcementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="80b8f-148">响应</span><span class="sxs-lookup"><span data-stu-id="80b8f-148">Response</span></span>

<span data-ttu-id="80b8f-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="80b8f-149">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update identitysecuritydefaultsenforcementpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

