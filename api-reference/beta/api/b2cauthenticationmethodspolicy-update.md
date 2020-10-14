---
title: 更新 b2cAuthenticationMethodsPolicy
description: 更新 b2cAuthenticationMethodsPolicy 对象的属性。
localization_priority: Priority
author: namkedia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fc40a64c1af6282b0a618062cb9a0bb4cc62cc5e
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458039"
---
# <a name="update-b2cauthenticationmethodspolicy"></a><span data-ttu-id="31154-103">更新 b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="31154-103">Update b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="31154-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31154-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31154-105">更新 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="31154-105">Update the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="31154-106">权限</span><span class="sxs-lookup"><span data-stu-id="31154-106">Permissions</span></span>

<span data-ttu-id="31154-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31154-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31154-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="31154-109">Permission type</span></span>                        | <span data-ttu-id="31154-110">权限</span><span class="sxs-lookup"><span data-stu-id="31154-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="31154-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31154-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="31154-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="31154-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="31154-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31154-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31154-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="31154-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="31154-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="31154-115">Application</span></span>                            | <span data-ttu-id="31154-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="31154-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="31154-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31154-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="31154-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="31154-118">Request headers</span></span>

|<span data-ttu-id="31154-119">名称</span><span class="sxs-lookup"><span data-stu-id="31154-119">Name</span></span>|<span data-ttu-id="31154-120">说明</span><span class="sxs-lookup"><span data-stu-id="31154-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="31154-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="31154-121">Authorization</span></span>|<span data-ttu-id="31154-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31154-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="31154-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31154-124">Content-Type</span></span>|<span data-ttu-id="31154-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="31154-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="31154-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="31154-127">Request body</span></span>

<span data-ttu-id="31154-128">在请求正文中，提供 JSON 表示形式的 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31154-128">In the request body, supply a JSON representation of the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

<span data-ttu-id="31154-129">下表显示了更新 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="31154-129">The following table shows the properties that are required when you update the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span></span>

| <span data-ttu-id="31154-130">属性</span><span class="sxs-lookup"><span data-stu-id="31154-130">Property</span></span>     | <span data-ttu-id="31154-131">类型</span><span class="sxs-lookup"><span data-stu-id="31154-131">Type</span></span>        | <span data-ttu-id="31154-132">Description</span><span class="sxs-lookup"><span data-stu-id="31154-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="31154-133">isEmailPasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="31154-133">isEmailPasswordAuthenticationEnabled</span></span>|<span data-ttu-id="31154-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="31154-134">Boolean</span></span>|<span data-ttu-id="31154-135">如果启用了电子邮件和密码身份验证方法，租户管理员可以使用电子邮件配置本地帐户。</span><span class="sxs-lookup"><span data-stu-id="31154-135">The tenant admin can configure local accounts using email if the email and password authentication method is enabled.</span></span>|
|<span data-ttu-id="31154-136">isUserNameAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="31154-136">isUserNameAuthenticationEnabled</span></span>|<span data-ttu-id="31154-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="31154-137">Boolean</span></span>|<span data-ttu-id="31154-138">如果启用了用户名和密码身份验证方法，租户管理员可以使用用户名配置本地帐户。</span><span class="sxs-lookup"><span data-stu-id="31154-138">The tenant admin can configure local accounts using username if the user name and password authentication method is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="31154-139">响应</span><span class="sxs-lookup"><span data-stu-id="31154-139">Response</span></span>

<span data-ttu-id="31154-140">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="31154-140">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31154-141">示例</span><span class="sxs-lookup"><span data-stu-id="31154-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="31154-142">请求</span><span class="sxs-lookup"><span data-stu-id="31154-142">Request</span></span>

<span data-ttu-id="31154-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="31154-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="31154-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="31154-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy

{
    "isEmailPasswordAuthenticationEnabled": false,
    "isUserNameAuthenticationEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="31154-145">C#</span><span class="sxs-lookup"><span data-stu-id="31154-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-b2cauthenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31154-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31154-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-b2cauthenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31154-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31154-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-b2cauthenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="31154-148">响应</span><span class="sxs-lookup"><span data-stu-id="31154-148">Response</span></span>

<span data-ttu-id="31154-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="31154-149">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cauthenticationmethodspolicy"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update b2cauthenticationmethodspolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
