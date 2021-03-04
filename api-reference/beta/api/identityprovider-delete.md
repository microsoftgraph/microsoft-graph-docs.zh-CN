---
title: 删除 identityProvider
description: 删除 identityProvider。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: f09503674cf3f340ef6b7ebe7a918c7c061368c9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435488"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="5fb85-103">删除 identityProvider</span><span class="sxs-lookup"><span data-stu-id="5fb85-103">Delete identityProvider</span></span>

<span data-ttu-id="5fb85-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fb85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fb85-105">删除 [identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="5fb85-105">Delete an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5fb85-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="5fb85-106">Permissions</span></span>

<span data-ttu-id="5fb85-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5fb85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fb85-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5fb85-109">Permission type</span></span>      | <span data-ttu-id="5fb85-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5fb85-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5fb85-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5fb85-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5fb85-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fb85-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="5fb85-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="5fb85-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5fb85-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fb85-114">Not supported.</span></span>|
|<span data-ttu-id="5fb85-115">Application</span><span class="sxs-lookup"><span data-stu-id="5fb85-115">Application</span></span>|<span data-ttu-id="5fb85-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fb85-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="5fb85-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="5fb85-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="5fb85-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="5fb85-118">Global administrator</span></span>
* <span data-ttu-id="5fb85-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="5fb85-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="5fb85-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5fb85-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5fb85-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5fb85-121">Request headers</span></span>

|<span data-ttu-id="5fb85-122">名称</span><span class="sxs-lookup"><span data-stu-id="5fb85-122">Name</span></span>|<span data-ttu-id="5fb85-123">说明</span><span class="sxs-lookup"><span data-stu-id="5fb85-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="5fb85-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fb85-124">Authorization</span></span>|<span data-ttu-id="5fb85-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5fb85-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fb85-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5fb85-127">Request body</span></span>

<span data-ttu-id="5fb85-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5fb85-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fb85-129">响应</span><span class="sxs-lookup"><span data-stu-id="5fb85-129">Response</span></span>

<span data-ttu-id="5fb85-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5fb85-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5fb85-131">示例</span><span class="sxs-lookup"><span data-stu-id="5fb85-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fb85-132">请求</span><span class="sxs-lookup"><span data-stu-id="5fb85-132">Request</span></span>

<span data-ttu-id="5fb85-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5fb85-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5fb85-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5fb85-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="5fb85-135">C#</span><span class="sxs-lookup"><span data-stu-id="5fb85-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5fb85-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5fb85-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5fb85-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5fb85-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5fb85-138">Java</span><span class="sxs-lookup"><span data-stu-id="5fb85-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5fb85-139">响应</span><span class="sxs-lookup"><span data-stu-id="5fb85-139">Response</span></span>

<span data-ttu-id="5fb85-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5fb85-140">The following is an example of the response.</span></span>

<span data-ttu-id="5fb85-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5fb85-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


