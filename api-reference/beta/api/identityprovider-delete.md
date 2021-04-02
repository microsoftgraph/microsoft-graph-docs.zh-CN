---
title: 删除 identityProvider
description: 删除 identityProvider。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 2924b7b4174f1457d212f4905dd829a23d636296
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508856"
---
# <a name="delete-identityprovider-deprecated"></a><span data-ttu-id="d54a2-103">删除 identityProvider (已弃) </span><span class="sxs-lookup"><span data-stu-id="d54a2-103">Delete identityProvider (deprecated)</span></span>
<span data-ttu-id="d54a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d54a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="d54a2-105">删除 [identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="d54a2-105">Delete an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d54a2-106">权限</span><span class="sxs-lookup"><span data-stu-id="d54a2-106">Permissions</span></span>

<span data-ttu-id="d54a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d54a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d54a2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d54a2-109">Permission type</span></span>      | <span data-ttu-id="d54a2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d54a2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d54a2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d54a2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d54a2-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d54a2-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="d54a2-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="d54a2-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d54a2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d54a2-114">Not supported.</span></span>|
|<span data-ttu-id="d54a2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d54a2-115">Application</span></span>|<span data-ttu-id="d54a2-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d54a2-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="d54a2-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="d54a2-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d54a2-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="d54a2-118">Global Administrator</span></span>
* <span data-ttu-id="d54a2-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="d54a2-119">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d54a2-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d54a2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d54a2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d54a2-121">Request headers</span></span>

|<span data-ttu-id="d54a2-122">名称</span><span class="sxs-lookup"><span data-stu-id="d54a2-122">Name</span></span>|<span data-ttu-id="d54a2-123">说明</span><span class="sxs-lookup"><span data-stu-id="d54a2-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d54a2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d54a2-124">Authorization</span></span>|<span data-ttu-id="d54a2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d54a2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d54a2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d54a2-127">Request body</span></span>

<span data-ttu-id="d54a2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d54a2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d54a2-129">响应</span><span class="sxs-lookup"><span data-stu-id="d54a2-129">Response</span></span>

<span data-ttu-id="d54a2-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d54a2-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d54a2-131">示例</span><span class="sxs-lookup"><span data-stu-id="d54a2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d54a2-132">请求</span><span class="sxs-lookup"><span data-stu-id="d54a2-132">Request</span></span>

<span data-ttu-id="d54a2-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d54a2-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identityProviders/{id}
```

# <a name="java"></a>[<span data-ttu-id="d54a2-134">Java</span><span class="sxs-lookup"><span data-stu-id="d54a2-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="d54a2-135">C#</span><span class="sxs-lookup"><span data-stu-id="d54a2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d54a2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d54a2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d54a2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d54a2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d54a2-138">响应</span><span class="sxs-lookup"><span data-stu-id="d54a2-138">Response</span></span>

<span data-ttu-id="d54a2-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d54a2-139">The following is an example of the response.</span></span>

<span data-ttu-id="d54a2-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d54a2-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
