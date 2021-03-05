---
title: 更新 identityProvider
description: 更新现有 identityProvider 中的属性
localization_priority: Priority
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bb4695068871c2c741a1f1aa699b36a688e22b6e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441835"
---
# <a name="update-identityprovider"></a><span data-ttu-id="ff8d8-103">更新 identityProvider</span><span class="sxs-lookup"><span data-stu-id="ff8d8-103">Update identityProvider</span></span>

<span data-ttu-id="ff8d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff8d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ff8d8-105">更新现有 [identityProvider](../resources/identityprovider.md) 中的属性。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-105">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ff8d8-106">权限</span><span class="sxs-lookup"><span data-stu-id="ff8d8-106">Permissions</span></span>

<span data-ttu-id="ff8d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff8d8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff8d8-109">Permission type</span></span>      | <span data-ttu-id="ff8d8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff8d8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff8d8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff8d8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff8d8-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff8d8-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="ff8d8-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="ff8d8-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ff8d8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-114">Not supported.</span></span>|
|<span data-ttu-id="ff8d8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff8d8-115">Application</span></span>|<span data-ttu-id="ff8d8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-116">Not supported.</span></span>|

<span data-ttu-id="ff8d8-117">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="ff8d8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff8d8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ff8d8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff8d8-119">Request headers</span></span>

|<span data-ttu-id="ff8d8-120">名称</span><span class="sxs-lookup"><span data-stu-id="ff8d8-120">Name</span></span>|<span data-ttu-id="ff8d8-121">说明</span><span class="sxs-lookup"><span data-stu-id="ff8d8-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ff8d8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff8d8-122">Authorization</span></span>|<span data-ttu-id="ff8d8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ff8d8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff8d8-125">Content-Type</span></span>|<span data-ttu-id="ff8d8-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ff8d8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff8d8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff8d8-128">Request body</span></span>

<span data-ttu-id="ff8d8-129">在请求正文中，为 JSON 对象提供一个或多个需要更新的属性。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-129">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="ff8d8-130">属性</span><span class="sxs-lookup"><span data-stu-id="ff8d8-130">Property</span></span>|<span data-ttu-id="ff8d8-131">类型</span><span class="sxs-lookup"><span data-stu-id="ff8d8-131">Type</span></span>|<span data-ttu-id="ff8d8-132">说明</span><span class="sxs-lookup"><span data-stu-id="ff8d8-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff8d8-133">clientId</span><span class="sxs-lookup"><span data-stu-id="ff8d8-133">clientId</span></span>|<span data-ttu-id="ff8d8-134">字符串</span><span class="sxs-lookup"><span data-stu-id="ff8d8-134">String</span></span>|<span data-ttu-id="ff8d8-135">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-135">The client ID for the application.</span></span> <span data-ttu-id="ff8d8-136">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="ff8d8-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="ff8d8-137">clientSecret</span></span>|<span data-ttu-id="ff8d8-138">字符串</span><span class="sxs-lookup"><span data-stu-id="ff8d8-138">String</span></span>|<span data-ttu-id="ff8d8-139">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-139">The client secret for the application.</span></span> <span data-ttu-id="ff8d8-140">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="ff8d8-141">name</span><span class="sxs-lookup"><span data-stu-id="ff8d8-141">name</span></span>|<span data-ttu-id="ff8d8-142">字符串</span><span class="sxs-lookup"><span data-stu-id="ff8d8-142">String</span></span>|<span data-ttu-id="ff8d8-143">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-143">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="ff8d8-144">响应</span><span class="sxs-lookup"><span data-stu-id="ff8d8-144">Response</span></span>

<span data-ttu-id="ff8d8-145">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-145">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="ff8d8-146">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-146">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="ff8d8-147">示例</span><span class="sxs-lookup"><span data-stu-id="ff8d8-147">Example</span></span>

<span data-ttu-id="ff8d8-148">以下示例会更新令牌生命周期 **identityProvider** 的定义并将其设置为组织默认值。</span><span class="sxs-lookup"><span data-stu-id="ff8d8-148">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="ff8d8-149">请求</span><span class="sxs-lookup"><span data-stu-id="ff8d8-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ff8d8-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff8d8-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update-identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```
# <a name="c"></a>[<span data-ttu-id="ff8d8-151">C#</span><span class="sxs-lookup"><span data-stu-id="ff8d8-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff8d8-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff8d8-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff8d8-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff8d8-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff8d8-154">Java</span><span class="sxs-lookup"><span data-stu-id="ff8d8-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ff8d8-155">响应</span><span class="sxs-lookup"><span data-stu-id="ff8d8-155">Response</span></span>

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
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

