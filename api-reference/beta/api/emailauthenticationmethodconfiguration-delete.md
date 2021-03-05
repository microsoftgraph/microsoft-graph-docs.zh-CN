---
title: 删除 emailAuthenticationMethodConfiguration
description: 删除 emailAuthenticationMethodConfiguration 对象。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: de27ecad11f484040790e2df0d327ba954c775dc
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472962"
---
# <a name="delete-emailauthenticationmethodconfiguration"></a><span data-ttu-id="9d311-103">删除 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="9d311-103">Delete emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="9d311-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d311-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d311-105">将电子邮件身份验证方法策略 [恢复](../resources/emailauthenticationmethodconfiguration.md) 为默认配置，以删除对策略所做的更改。</span><span class="sxs-lookup"><span data-stu-id="9d311-105">Remove changes made to the [email authentication method policy](../resources/emailauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d311-106">权限</span><span class="sxs-lookup"><span data-stu-id="9d311-106">Permissions</span></span>
<span data-ttu-id="9d311-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d311-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d311-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d311-109">Permission type</span></span>|<span data-ttu-id="9d311-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d311-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d311-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d311-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9d311-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9d311-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="9d311-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d311-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d311-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d311-114">Not supported.</span></span>|
|<span data-ttu-id="9d311-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d311-115">Application</span></span>|<span data-ttu-id="9d311-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d311-116">Not supported.</span></span>|

<span data-ttu-id="9d311-117">对于委派方案，管理员需要以下角色之 [一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="9d311-117">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="9d311-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="9d311-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="9d311-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d311-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="9d311-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d311-120">Request headers</span></span>

|<span data-ttu-id="9d311-121">名称</span><span class="sxs-lookup"><span data-stu-id="9d311-121">Name</span></span>|<span data-ttu-id="9d311-122">说明</span><span class="sxs-lookup"><span data-stu-id="9d311-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9d311-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d311-123">Authorization</span></span>|<span data-ttu-id="9d311-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9d311-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d311-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d311-126">Request body</span></span>

<span data-ttu-id="9d311-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9d311-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d311-128">响应</span><span class="sxs-lookup"><span data-stu-id="9d311-128">Response</span></span>

<span data-ttu-id="9d311-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9d311-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9d311-130">示例</span><span class="sxs-lookup"><span data-stu-id="9d311-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9d311-131">请求</span><span class="sxs-lookup"><span data-stu-id="9d311-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9d311-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d311-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethodconfiguration"
}
-->

```http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```
# <a name="c"></a>[<span data-ttu-id="9d311-133">C#</span><span class="sxs-lookup"><span data-stu-id="9d311-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-emailauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d311-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d311-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-emailauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d311-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d311-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-emailauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d311-136">Java</span><span class="sxs-lookup"><span data-stu-id="9d311-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-emailauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9d311-137">响应</span><span class="sxs-lookup"><span data-stu-id="9d311-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

