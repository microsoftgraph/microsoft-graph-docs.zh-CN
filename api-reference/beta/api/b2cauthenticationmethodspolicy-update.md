---
title: 更新 b2cAuthenticationMethodsPolicy
description: 更新 b2cAuthenticationMethodsPolicy 对象的属性。
localization_priority: Priority
author: namkedia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b4f85da6545e430ee2a04fabd4e3aa16a3062457
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786837"
---
# <a name="update-b2cauthenticationmethodspolicy"></a><span data-ttu-id="e73c0-103">更新 b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="e73c0-103">Update b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="e73c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e73c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e73c0-105">更新 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e73c0-105">Update the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e73c0-106">权限</span><span class="sxs-lookup"><span data-stu-id="e73c0-106">Permissions</span></span>

<span data-ttu-id="e73c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e73c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e73c0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e73c0-109">Permission type</span></span>                        | <span data-ttu-id="e73c0-110">权限</span><span class="sxs-lookup"><span data-stu-id="e73c0-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="e73c0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e73c0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e73c0-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e73c0-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="e73c0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e73c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e73c0-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e73c0-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="e73c0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e73c0-115">Application</span></span>                            | <span data-ttu-id="e73c0-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e73c0-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="e73c0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e73c0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="e73c0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e73c0-118">Request headers</span></span>

|<span data-ttu-id="e73c0-119">名称</span><span class="sxs-lookup"><span data-stu-id="e73c0-119">Name</span></span>|<span data-ttu-id="e73c0-120">说明</span><span class="sxs-lookup"><span data-stu-id="e73c0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e73c0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e73c0-121">Authorization</span></span>|<span data-ttu-id="e73c0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e73c0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e73c0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e73c0-124">Content-Type</span></span>|<span data-ttu-id="e73c0-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e73c0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e73c0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e73c0-127">Request body</span></span>

<span data-ttu-id="e73c0-128">在请求正文中，提供 JSON 表示形式的 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e73c0-128">In the request body, supply a JSON representation of the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

<span data-ttu-id="e73c0-129">下表显示了更新 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e73c0-129">The following table shows the properties that are required when you update the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span></span>

| <span data-ttu-id="e73c0-130">属性</span><span class="sxs-lookup"><span data-stu-id="e73c0-130">Property</span></span>     | <span data-ttu-id="e73c0-131">类型</span><span class="sxs-lookup"><span data-stu-id="e73c0-131">Type</span></span>        | <span data-ttu-id="e73c0-132">Description</span><span class="sxs-lookup"><span data-stu-id="e73c0-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e73c0-133">isEmailPasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="e73c0-133">isEmailPasswordAuthenticationEnabled</span></span>|<span data-ttu-id="e73c0-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="e73c0-134">Boolean</span></span>|<span data-ttu-id="e73c0-135">如果启用了电子邮件和密码身份验证方法，租户管理员可以使用电子邮件配置本地帐户。</span><span class="sxs-lookup"><span data-stu-id="e73c0-135">The tenant admin can configure local accounts using email if the email and password authentication method is enabled.</span></span>|
|<span data-ttu-id="e73c0-136">isUserNameAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="e73c0-136">isUserNameAuthenticationEnabled</span></span>|<span data-ttu-id="e73c0-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="e73c0-137">Boolean</span></span>|<span data-ttu-id="e73c0-138">如果启用了用户名和密码身份验证方法，租户管理员可以使用用户名配置本地帐户。</span><span class="sxs-lookup"><span data-stu-id="e73c0-138">The tenant admin can configure local accounts using username if the username and password authentication method is enabled.</span></span>|
|<span data-ttu-id="e73c0-139">isPhoneOneTimePasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="e73c0-139">isPhoneOneTimePasswordAuthenticationEnabled</span></span>|<span data-ttu-id="e73c0-140">布尔值</span><span class="sxs-lookup"><span data-stu-id="e73c0-140">Boolean</span></span>|<span data-ttu-id="e73c0-141">如果已启用电话号码和一次性密码身份验证方法，则租户管理员可以使用电话号码配置本地帐户。</span><span class="sxs-lookup"><span data-stu-id="e73c0-141">The tenant admin can configure local accounts using phone number if the phone number and one-time password authentication method is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="e73c0-142">响应</span><span class="sxs-lookup"><span data-stu-id="e73c0-142">Response</span></span>

<span data-ttu-id="e73c0-143">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="e73c0-143">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e73c0-144">示例</span><span class="sxs-lookup"><span data-stu-id="e73c0-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e73c0-145">请求</span><span class="sxs-lookup"><span data-stu-id="e73c0-145">Request</span></span>

<span data-ttu-id="e73c0-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e73c0-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e73c0-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e73c0-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy

{
    "isEmailPasswordAuthenticationEnabled": false,
    "isUserNameAuthenticationEnabled": true,
    "isPhoneOneTimePasswordAuthenticationEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="e73c0-148">C#</span><span class="sxs-lookup"><span data-stu-id="e73c0-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-b2cauthenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e73c0-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e73c0-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-b2cauthenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e73c0-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e73c0-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-b2cauthenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e73c0-151">Java</span><span class="sxs-lookup"><span data-stu-id="e73c0-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-b2cauthenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e73c0-152">响应</span><span class="sxs-lookup"><span data-stu-id="e73c0-152">Response</span></span>

<span data-ttu-id="e73c0-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e73c0-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
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
