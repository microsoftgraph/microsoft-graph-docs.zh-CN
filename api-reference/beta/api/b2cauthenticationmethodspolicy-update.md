---
title: 更新 b2cAuthenticationMethodsPolicy
description: 更新 b2cAuthenticationMethodsPolicy 对象的属性。
localization_priority: Priority
author: namkedia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aed20c26bab07cb6778b80d10e3becf33e998409
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961267"
---
# <a name="update-b2cauthenticationmethodspolicy"></a><span data-ttu-id="86ed2-103">更新 b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="86ed2-103">Update b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="86ed2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86ed2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86ed2-105">更新 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="86ed2-105">Update the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="86ed2-106">权限</span><span class="sxs-lookup"><span data-stu-id="86ed2-106">Permissions</span></span>

<span data-ttu-id="86ed2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86ed2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86ed2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="86ed2-109">Permission type</span></span>                        | <span data-ttu-id="86ed2-110">权限</span><span class="sxs-lookup"><span data-stu-id="86ed2-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="86ed2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86ed2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="86ed2-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="86ed2-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="86ed2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86ed2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86ed2-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="86ed2-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="86ed2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="86ed2-115">Application</span></span>                            | <span data-ttu-id="86ed2-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="86ed2-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="86ed2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86ed2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="86ed2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="86ed2-118">Request headers</span></span>

|<span data-ttu-id="86ed2-119">名称</span><span class="sxs-lookup"><span data-stu-id="86ed2-119">Name</span></span>|<span data-ttu-id="86ed2-120">说明</span><span class="sxs-lookup"><span data-stu-id="86ed2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="86ed2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="86ed2-121">Authorization</span></span>|<span data-ttu-id="86ed2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="86ed2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="86ed2-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86ed2-124">Content-Type</span></span>|<span data-ttu-id="86ed2-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="86ed2-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86ed2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="86ed2-127">Request body</span></span>

<span data-ttu-id="86ed2-128">在请求正文中，提供 JSON 表示形式的 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86ed2-128">In the request body, supply a JSON representation of the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

<span data-ttu-id="86ed2-129">下表显示了更新 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="86ed2-129">The following table shows the properties that are required when you update the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span></span>

| <span data-ttu-id="86ed2-130">属性</span><span class="sxs-lookup"><span data-stu-id="86ed2-130">Property</span></span>     | <span data-ttu-id="86ed2-131">类型</span><span class="sxs-lookup"><span data-stu-id="86ed2-131">Type</span></span>        | <span data-ttu-id="86ed2-132">Description</span><span class="sxs-lookup"><span data-stu-id="86ed2-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="86ed2-133">isEmailPasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="86ed2-133">isEmailPasswordAuthenticationEnabled</span></span>|<span data-ttu-id="86ed2-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="86ed2-134">Boolean</span></span>|<span data-ttu-id="86ed2-135">如果启用了电子邮件和密码身份验证方法，租户管理员可以使用电子邮件配置本地帐户。</span><span class="sxs-lookup"><span data-stu-id="86ed2-135">The tenant admin can configure local accounts using email if the email and password authentication method is enabled.</span></span>|
|<span data-ttu-id="86ed2-136">isUserNameAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="86ed2-136">isUserNameAuthenticationEnabled</span></span>|<span data-ttu-id="86ed2-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="86ed2-137">Boolean</span></span>|<span data-ttu-id="86ed2-138">如果启用了用户名和密码身份验证方法，租户管理员可以使用用户名配置本地帐户。</span><span class="sxs-lookup"><span data-stu-id="86ed2-138">The tenant admin can configure local accounts using username if the username and password authentication method is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="86ed2-139">响应</span><span class="sxs-lookup"><span data-stu-id="86ed2-139">Response</span></span>

<span data-ttu-id="86ed2-140">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="86ed2-140">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86ed2-141">示例</span><span class="sxs-lookup"><span data-stu-id="86ed2-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86ed2-142">请求</span><span class="sxs-lookup"><span data-stu-id="86ed2-142">Request</span></span>

<span data-ttu-id="86ed2-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="86ed2-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="86ed2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="86ed2-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="86ed2-145">C#</span><span class="sxs-lookup"><span data-stu-id="86ed2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-b2cauthenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86ed2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86ed2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-b2cauthenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86ed2-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86ed2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-b2cauthenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86ed2-148">Java</span><span class="sxs-lookup"><span data-stu-id="86ed2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-b2cauthenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="86ed2-149">响应</span><span class="sxs-lookup"><span data-stu-id="86ed2-149">Response</span></span>

<span data-ttu-id="86ed2-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="86ed2-150">The following is an example of the response.</span></span>

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
