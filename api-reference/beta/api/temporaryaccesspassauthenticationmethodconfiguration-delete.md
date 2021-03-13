---
title: 删除 temporaryAccessPassAuthenticationMethodConfiguration
description: 删除对 temporaryAccessPassAuthenticationMethodConfiguration 对象所做的更改。
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f55afafed3863ffeab1c8bf786602606112e048b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761854"
---
# <a name="delete-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="cb4b2-103">删除 temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb4b2-103">Delete temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="cb4b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb4b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb4b2-105">将策略还原为默认配置，删除 [对 temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) 对象所做的更改。</span><span class="sxs-lookup"><span data-stu-id="cb4b2-105">Remove changes made to the [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb4b2-106">权限</span><span class="sxs-lookup"><span data-stu-id="cb4b2-106">Permissions</span></span>
<span data-ttu-id="cb4b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb4b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb4b2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb4b2-109">Permission type</span></span>|<span data-ttu-id="cb4b2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb4b2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb4b2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb4b2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cb4b2-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cb4b2-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="cb4b2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb4b2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb4b2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb4b2-114">Not supported.</span></span>|
|<span data-ttu-id="cb4b2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb4b2-115">Application</span></span>|<span data-ttu-id="cb4b2-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cb4b2-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="cb4b2-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="cb4b2-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="cb4b2-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="cb4b2-118">For more information, see [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="cb4b2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb4b2-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```


## <a name="request-headers"></a><span data-ttu-id="cb4b2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb4b2-120">Request headers</span></span>
|<span data-ttu-id="cb4b2-121">名称</span><span class="sxs-lookup"><span data-stu-id="cb4b2-121">Name</span></span>|<span data-ttu-id="cb4b2-122">说明</span><span class="sxs-lookup"><span data-stu-id="cb4b2-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cb4b2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb4b2-123">Authorization</span></span>|<span data-ttu-id="cb4b2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb4b2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb4b2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb4b2-126">Request body</span></span>
<span data-ttu-id="cb4b2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cb4b2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb4b2-128">响应</span><span class="sxs-lookup"><span data-stu-id="cb4b2-128">Response</span></span>

<span data-ttu-id="cb4b2-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cb4b2-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cb4b2-130">示例</span><span class="sxs-lookup"><span data-stu-id="cb4b2-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb4b2-131">请求</span><span class="sxs-lookup"><span data-stu-id="cb4b2-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cb4b2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb4b2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```
# <a name="c"></a>[<span data-ttu-id="cb4b2-133">C#</span><span class="sxs-lookup"><span data-stu-id="cb4b2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb4b2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb4b2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb4b2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb4b2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb4b2-136">Java</span><span class="sxs-lookup"><span data-stu-id="cb4b2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="cb4b2-137">响应</span><span class="sxs-lookup"><span data-stu-id="cb4b2-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
