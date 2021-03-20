---
title: 删除 temporaryAccessPassAuthenticationMethodConfiguration
description: 删除对 temporaryAccessPassAuthenticationMethodConfiguration 对象所做的更改。
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4512b4127a9c1fe1bab4c9e7bc0645d39f79c3b1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953993"
---
# <a name="delete-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="e195d-103">删除 temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="e195d-103">Delete temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="e195d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e195d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e195d-105">将策略还原为默认配置，删除 [对 temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) 对象所做的更改。</span><span class="sxs-lookup"><span data-stu-id="e195d-105">Remove changes made to the [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="e195d-106">权限</span><span class="sxs-lookup"><span data-stu-id="e195d-106">Permissions</span></span>
<span data-ttu-id="e195d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e195d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e195d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e195d-109">Permission type</span></span>|<span data-ttu-id="e195d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e195d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e195d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e195d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e195d-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e195d-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="e195d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e195d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e195d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e195d-114">Not supported.</span></span>|
|<span data-ttu-id="e195d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e195d-115">Application</span></span>|<span data-ttu-id="e195d-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e195d-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="e195d-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="e195d-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="e195d-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="e195d-118">For more information, see [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="e195d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e195d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```


## <a name="request-headers"></a><span data-ttu-id="e195d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e195d-120">Request headers</span></span>
|<span data-ttu-id="e195d-121">名称</span><span class="sxs-lookup"><span data-stu-id="e195d-121">Name</span></span>|<span data-ttu-id="e195d-122">说明</span><span class="sxs-lookup"><span data-stu-id="e195d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e195d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e195d-123">Authorization</span></span>|<span data-ttu-id="e195d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e195d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e195d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e195d-126">Request body</span></span>
<span data-ttu-id="e195d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e195d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e195d-128">响应</span><span class="sxs-lookup"><span data-stu-id="e195d-128">Response</span></span>

<span data-ttu-id="e195d-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e195d-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e195d-130">示例</span><span class="sxs-lookup"><span data-stu-id="e195d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e195d-131">请求</span><span class="sxs-lookup"><span data-stu-id="e195d-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e195d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e195d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration_2"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```
# <a name="c"></a>[<span data-ttu-id="e195d-133">C#</span><span class="sxs-lookup"><span data-stu-id="e195d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethodconfiguration-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e195d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e195d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethodconfiguration-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e195d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e195d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethodconfiguration-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e195d-136">Java</span><span class="sxs-lookup"><span data-stu-id="e195d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethodconfiguration-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e195d-137">响应</span><span class="sxs-lookup"><span data-stu-id="e195d-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
