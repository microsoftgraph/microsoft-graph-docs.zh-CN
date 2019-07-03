---
title: 删除 identityProvider
description: 删除现有的 identityProvider
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 464ae5b8490a1cd5f9762dd4c1443c4d74a8acd0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447360"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="77551-103">删除 identityProvider</span><span class="sxs-lookup"><span data-stu-id="77551-103">Delete identityProvider</span></span>

<span data-ttu-id="77551-104">删除现有的 [identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="77551-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="77551-105">权限</span><span class="sxs-lookup"><span data-stu-id="77551-105">Permissions</span></span>

<span data-ttu-id="77551-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77551-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77551-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="77551-108">Permission type</span></span>      | <span data-ttu-id="77551-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77551-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77551-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77551-110">Delegated (work or school account)</span></span>|<span data-ttu-id="77551-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77551-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="77551-112">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="77551-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="77551-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="77551-113">Not supported.</span></span>|
|<span data-ttu-id="77551-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="77551-114">Application</span></span>|<span data-ttu-id="77551-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="77551-115">Not supported.</span></span>|

<span data-ttu-id="77551-116">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="77551-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="77551-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77551-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="77551-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="77551-118">Request headers</span></span>

|<span data-ttu-id="77551-119">名称</span><span class="sxs-lookup"><span data-stu-id="77551-119">Name</span></span>|<span data-ttu-id="77551-120">说明</span><span class="sxs-lookup"><span data-stu-id="77551-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="77551-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="77551-121">Authorization</span></span>|<span data-ttu-id="77551-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77551-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77551-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="77551-124">Request body</span></span>

<span data-ttu-id="77551-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77551-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77551-126">响应</span><span class="sxs-lookup"><span data-stu-id="77551-126">Response</span></span>

<span data-ttu-id="77551-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="77551-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="77551-128">示例</span><span class="sxs-lookup"><span data-stu-id="77551-128">Example</span></span>

<span data-ttu-id="77551-129">以下示例会删除 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="77551-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="77551-130">请求</span><span class="sxs-lookup"><span data-stu-id="77551-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="77551-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="77551-131">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="77551-132">C#</span><span class="sxs-lookup"><span data-stu-id="77551-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77551-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="77551-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77551-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77551-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="77551-135">响应</span><span class="sxs-lookup"><span data-stu-id="77551-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
