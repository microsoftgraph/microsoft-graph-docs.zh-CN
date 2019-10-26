---
title: 更新 identityProvider
description: 更新现有 Identityprovider.read.all 中的属性。
localization_priority: Normal
doc_type: apiPageType
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cbbac43b7c47ee7aa160bf1e66a94e1afdb0c60
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734428"
---
# <a name="update-identityprovider"></a><span data-ttu-id="18b98-103">更新 identityProvider</span><span class="sxs-lookup"><span data-stu-id="18b98-103">Update identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18b98-104">更新现有 [identityProvider](../resources/identityprovider.md) 中的属性。</span><span class="sxs-lookup"><span data-stu-id="18b98-104">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="18b98-105">权限</span><span class="sxs-lookup"><span data-stu-id="18b98-105">Permissions</span></span>

<span data-ttu-id="18b98-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18b98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18b98-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="18b98-108">Permission type</span></span>      | <span data-ttu-id="18b98-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18b98-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18b98-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18b98-110">Delegated (work or school account)</span></span>|<span data-ttu-id="18b98-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18b98-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="18b98-112">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="18b98-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="18b98-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="18b98-113">Not supported.</span></span>|
|<span data-ttu-id="18b98-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="18b98-114">Application</span></span>| <span data-ttu-id="18b98-115">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18b98-115">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="18b98-116">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="18b98-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="18b98-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18b98-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="18b98-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="18b98-118">Request headers</span></span>

|<span data-ttu-id="18b98-119">名称</span><span class="sxs-lookup"><span data-stu-id="18b98-119">Name</span></span>|<span data-ttu-id="18b98-120">说明</span><span class="sxs-lookup"><span data-stu-id="18b98-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="18b98-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="18b98-121">Authorization</span></span>|<span data-ttu-id="18b98-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18b98-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="18b98-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18b98-124">Content-Type</span></span>|<span data-ttu-id="18b98-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="18b98-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="18b98-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="18b98-127">Request body</span></span>

<span data-ttu-id="18b98-128">在请求正文中，为 JSON 对象提供一个或多个需要更新的属性。</span><span class="sxs-lookup"><span data-stu-id="18b98-128">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="18b98-129">属性</span><span class="sxs-lookup"><span data-stu-id="18b98-129">Property</span></span>|<span data-ttu-id="18b98-130">类型</span><span class="sxs-lookup"><span data-stu-id="18b98-130">Type</span></span>|<span data-ttu-id="18b98-131">说明</span><span class="sxs-lookup"><span data-stu-id="18b98-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18b98-132">clientId</span><span class="sxs-lookup"><span data-stu-id="18b98-132">clientId</span></span>|<span data-ttu-id="18b98-133">字符串</span><span class="sxs-lookup"><span data-stu-id="18b98-133">String</span></span>|<span data-ttu-id="18b98-134">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="18b98-134">The client ID for the application.</span></span> <span data-ttu-id="18b98-135">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="18b98-135">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="18b98-136">clientSecret</span><span class="sxs-lookup"><span data-stu-id="18b98-136">clientSecret</span></span>|<span data-ttu-id="18b98-137">字符串</span><span class="sxs-lookup"><span data-stu-id="18b98-137">String</span></span>|<span data-ttu-id="18b98-138">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="18b98-138">The client secret for the application.</span></span> <span data-ttu-id="18b98-139">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="18b98-139">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="18b98-140">name</span><span class="sxs-lookup"><span data-stu-id="18b98-140">name</span></span>|<span data-ttu-id="18b98-141">字符串</span><span class="sxs-lookup"><span data-stu-id="18b98-141">String</span></span>|<span data-ttu-id="18b98-142">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="18b98-142">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="18b98-143">响应</span><span class="sxs-lookup"><span data-stu-id="18b98-143">Response</span></span>

<span data-ttu-id="18b98-144">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="18b98-144">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="18b98-145">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="18b98-145">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="18b98-146">示例</span><span class="sxs-lookup"><span data-stu-id="18b98-146">Example</span></span>

<span data-ttu-id="18b98-147">以下示例会更新令牌生命周期 **identityProvider** 的定义并将其设置为组织默认值。</span><span class="sxs-lookup"><span data-stu-id="18b98-147">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="18b98-148">请求</span><span class="sxs-lookup"><span data-stu-id="18b98-148">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="18b98-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="18b98-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="18b98-150">C#</span><span class="sxs-lookup"><span data-stu-id="18b98-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18b98-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18b98-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="18b98-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18b98-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="18b98-153">响应</span><span class="sxs-lookup"><span data-stu-id="18b98-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
