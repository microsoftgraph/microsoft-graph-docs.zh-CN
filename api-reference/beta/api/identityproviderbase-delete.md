---
title: 删除 identityProvider
description: 删除 identityProvider。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: d78aff8a604f42b7efbc1f87269a87acbb29656c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508806"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="41766-103">删除 identityProvider</span><span class="sxs-lookup"><span data-stu-id="41766-103">Delete identityProvider</span></span>
<span data-ttu-id="41766-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41766-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41766-105">删除 Azure AD 中的 [socialIdentityProvider](../resources/socialidentityprovider.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41766-105">Delete a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="41766-106">在 Azure AD B2C 中，删除 [socialIdentityProvider](../resources/socialidentityprovider.md) [、openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) 或 [appleIdentityProvider](../resources/appleidentityprovider.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41766-106">In Azure AD B2C, delete a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="41766-107">权限</span><span class="sxs-lookup"><span data-stu-id="41766-107">Permissions</span></span>

<span data-ttu-id="41766-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41766-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41766-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="41766-110">Permission type</span></span>      | <span data-ttu-id="41766-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41766-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41766-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41766-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41766-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41766-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="41766-114">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="41766-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="41766-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="41766-115">Not supported.</span></span>|
|<span data-ttu-id="41766-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="41766-116">Application</span></span>|<span data-ttu-id="41766-117">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41766-117">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="41766-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="41766-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="41766-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="41766-119">Global Administrator</span></span>
* <span data-ttu-id="41766-120">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="41766-120">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="41766-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41766-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="41766-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="41766-122">Request headers</span></span>

|<span data-ttu-id="41766-123">名称</span><span class="sxs-lookup"><span data-stu-id="41766-123">Name</span></span>|<span data-ttu-id="41766-124">说明</span><span class="sxs-lookup"><span data-stu-id="41766-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="41766-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="41766-125">Authorization</span></span>|<span data-ttu-id="41766-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="41766-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="41766-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="41766-128">Request body</span></span>

<span data-ttu-id="41766-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41766-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41766-130">响应</span><span class="sxs-lookup"><span data-stu-id="41766-130">Response</span></span>

<span data-ttu-id="41766-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="41766-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="41766-132">示例</span><span class="sxs-lookup"><span data-stu-id="41766-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="41766-133">请求</span><span class="sxs-lookup"><span data-stu-id="41766-133">Request</span></span>

<span data-ttu-id="41766-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="41766-134">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="41766-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="41766-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="41766-136">C#</span><span class="sxs-lookup"><span data-stu-id="41766-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41766-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41766-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41766-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41766-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41766-139">Java</span><span class="sxs-lookup"><span data-stu-id="41766-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="41766-140">响应</span><span class="sxs-lookup"><span data-stu-id="41766-140">Response</span></span>

<span data-ttu-id="41766-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="41766-141">The following is an example of the response.</span></span>

<span data-ttu-id="41766-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="41766-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
