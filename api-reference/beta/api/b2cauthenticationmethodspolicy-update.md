---
title: 更新 b2cAuthenticationMethodsPolicy
description: 更新 b2cAuthenticationMethodsPolicy 对象的属性。
localization_priority: Priority
author: namkedia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 61c3bfa7d3fef328ed3c06d51f8c1db4ae552405
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406282"
---
# <a name="update-b2cauthenticationmethodspolicy"></a><span data-ttu-id="0748f-103">更新 b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="0748f-103">Update b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="0748f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0748f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0748f-105">更新 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0748f-105">Update the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0748f-106">权限</span><span class="sxs-lookup"><span data-stu-id="0748f-106">Permissions</span></span>

<span data-ttu-id="0748f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0748f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0748f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0748f-109">Permission type</span></span>                        | <span data-ttu-id="0748f-110">权限</span><span class="sxs-lookup"><span data-stu-id="0748f-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="0748f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0748f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0748f-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0748f-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="0748f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0748f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0748f-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0748f-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="0748f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0748f-115">Application</span></span>                            | <span data-ttu-id="0748f-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0748f-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="0748f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0748f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="0748f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0748f-118">Request headers</span></span>

|<span data-ttu-id="0748f-119">名称</span><span class="sxs-lookup"><span data-stu-id="0748f-119">Name</span></span>|<span data-ttu-id="0748f-120">说明</span><span class="sxs-lookup"><span data-stu-id="0748f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0748f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0748f-121">Authorization</span></span>|<span data-ttu-id="0748f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0748f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0748f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0748f-124">Content-Type</span></span>|<span data-ttu-id="0748f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0748f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0748f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0748f-127">Request body</span></span>

<span data-ttu-id="0748f-128">在请求正文中，提供 JSON 表示形式的 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0748f-128">In the request body, supply a JSON representation of the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

<span data-ttu-id="0748f-129">下表显示了更新 [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0748f-129">The following table shows the properties that are required when you update the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span></span>

| <span data-ttu-id="0748f-130">属性</span><span class="sxs-lookup"><span data-stu-id="0748f-130">Property</span></span>     | <span data-ttu-id="0748f-131">类型</span><span class="sxs-lookup"><span data-stu-id="0748f-131">Type</span></span>        | <span data-ttu-id="0748f-132">Description</span><span class="sxs-lookup"><span data-stu-id="0748f-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0748f-133">isEmailPasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="0748f-133">isEmailPasswordAuthenticationEnabled</span></span>|<span data-ttu-id="0748f-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="0748f-134">Boolean</span></span>|<span data-ttu-id="0748f-135">如果启用了电子邮件和密码身份验证方法，租户管理员可以使用电子邮件配置本地帐户。</span><span class="sxs-lookup"><span data-stu-id="0748f-135">The tenant admin can configure local accounts using email if the email and password authentication method is enabled.</span></span>|
|<span data-ttu-id="0748f-136">isUserNameAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="0748f-136">isUserNameAuthenticationEnabled</span></span>|<span data-ttu-id="0748f-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="0748f-137">Boolean</span></span>|<span data-ttu-id="0748f-138">如果启用了用户名和密码身份验证方法，租户管理员可以使用用户名配置本地帐户。</span><span class="sxs-lookup"><span data-stu-id="0748f-138">The tenant admin can configure local accounts using username if the user name and password authentication method is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="0748f-139">响应</span><span class="sxs-lookup"><span data-stu-id="0748f-139">Response</span></span>

<span data-ttu-id="0748f-140">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="0748f-140">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0748f-141">示例</span><span class="sxs-lookup"><span data-stu-id="0748f-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0748f-142">请求</span><span class="sxs-lookup"><span data-stu-id="0748f-142">Request</span></span>

<span data-ttu-id="0748f-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0748f-143">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="0748f-144">响应</span><span class="sxs-lookup"><span data-stu-id="0748f-144">Response</span></span>

<span data-ttu-id="0748f-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0748f-145">The following is an example of the response.</span></span>

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
