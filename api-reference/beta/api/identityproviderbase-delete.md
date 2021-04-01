---
title: 删除 identityProvider
description: 删除 identityProvider。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: cdacaf4495d6856bc39465d4bed990a20cd264e7
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491060"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="9d24b-103">删除 identityProvider</span><span class="sxs-lookup"><span data-stu-id="9d24b-103">Delete identityProvider</span></span>
<span data-ttu-id="9d24b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d24b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d24b-105">删除 Azure AD 中的 [socialIdentityProvider](../resources/socialidentityprovider.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d24b-105">Delete a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="9d24b-106">在 Azure AD B2C 中，删除 [socialIdentityProvider](../resources/socialidentityprovider.md) [、openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) 或 [appleIdentityProvider](../resources/appleidentityprovider.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d24b-106">In Azure AD B2C, delete a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d24b-107">权限</span><span class="sxs-lookup"><span data-stu-id="9d24b-107">Permissions</span></span>

<span data-ttu-id="9d24b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d24b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d24b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d24b-110">Permission type</span></span>      | <span data-ttu-id="9d24b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d24b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d24b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d24b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9d24b-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d24b-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="9d24b-114">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="9d24b-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9d24b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d24b-115">Not supported.</span></span>|
|<span data-ttu-id="9d24b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d24b-116">Application</span></span>|<span data-ttu-id="9d24b-117">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d24b-117">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="9d24b-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="9d24b-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="9d24b-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="9d24b-119">Global Administrator</span></span>
* <span data-ttu-id="9d24b-120">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="9d24b-120">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9d24b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d24b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9d24b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d24b-122">Request headers</span></span>

|<span data-ttu-id="9d24b-123">名称</span><span class="sxs-lookup"><span data-stu-id="9d24b-123">Name</span></span>|<span data-ttu-id="9d24b-124">说明</span><span class="sxs-lookup"><span data-stu-id="9d24b-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9d24b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d24b-125">Authorization</span></span>|<span data-ttu-id="9d24b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9d24b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d24b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d24b-128">Request body</span></span>

<span data-ttu-id="9d24b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9d24b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d24b-130">响应</span><span class="sxs-lookup"><span data-stu-id="9d24b-130">Response</span></span>

<span data-ttu-id="9d24b-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9d24b-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9d24b-132">示例</span><span class="sxs-lookup"><span data-stu-id="9d24b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d24b-133">请求</span><span class="sxs-lookup"><span data-stu-id="9d24b-133">Request</span></span>

<span data-ttu-id="9d24b-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9d24b-134">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/identityProviders/{id}
```

### <a name="response"></a><span data-ttu-id="9d24b-135">响应</span><span class="sxs-lookup"><span data-stu-id="9d24b-135">Response</span></span>

<span data-ttu-id="9d24b-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9d24b-136">The following is an example of the response.</span></span>

<span data-ttu-id="9d24b-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9d24b-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
