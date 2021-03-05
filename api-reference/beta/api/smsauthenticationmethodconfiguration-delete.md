---
title: 删除 smsAuthenticationMethodConfiguration
description: 删除 smsAuthenticationMethodConfiguration 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ec22cabd9ca43a6415509f114fa1592855f0b8a8
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475620"
---
# <a name="delete-smsauthenticationmethodconfiguration"></a><span data-ttu-id="2ed60-103">删除 smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ed60-103">Delete smsAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="2ed60-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ed60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ed60-105">将策略还原为默认[](../resources/smsauthenticationmethodconfiguration.md)配置，删除对短信身份验证方法策略所做的更改。</span><span class="sxs-lookup"><span data-stu-id="2ed60-105">Remove changes made to the [Text Message authentication method policy](../resources/smsauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ed60-106">权限</span><span class="sxs-lookup"><span data-stu-id="2ed60-106">Permissions</span></span>
<span data-ttu-id="2ed60-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ed60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ed60-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ed60-109">Permission type</span></span>|<span data-ttu-id="2ed60-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ed60-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ed60-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ed60-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2ed60-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2ed60-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="2ed60-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ed60-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ed60-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ed60-114">Not supported.</span></span>|
|<span data-ttu-id="2ed60-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ed60-115">Application</span></span>|<span data-ttu-id="2ed60-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2ed60-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="2ed60-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="2ed60-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="2ed60-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="2ed60-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="2ed60-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ed60-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
```

## <a name="request-headers"></a><span data-ttu-id="2ed60-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ed60-120">Request headers</span></span>
|<span data-ttu-id="2ed60-121">名称</span><span class="sxs-lookup"><span data-stu-id="2ed60-121">Name</span></span>|<span data-ttu-id="2ed60-122">说明</span><span class="sxs-lookup"><span data-stu-id="2ed60-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2ed60-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ed60-123">Authorization</span></span>|<span data-ttu-id="2ed60-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ed60-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ed60-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ed60-126">Request body</span></span>
<span data-ttu-id="2ed60-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ed60-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ed60-128">响应</span><span class="sxs-lookup"><span data-stu-id="2ed60-128">Response</span></span>

<span data-ttu-id="2ed60-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2ed60-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2ed60-130">示例</span><span class="sxs-lookup"><span data-stu-id="2ed60-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ed60-131">请求</span><span class="sxs-lookup"><span data-stu-id="2ed60-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2ed60-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ed60-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_smsauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
```
# <a name="c"></a>[<span data-ttu-id="2ed60-133">C#</span><span class="sxs-lookup"><span data-stu-id="2ed60-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-smsauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ed60-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ed60-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-smsauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ed60-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ed60-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-smsauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ed60-136">Java</span><span class="sxs-lookup"><span data-stu-id="2ed60-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-smsauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2ed60-137">响应</span><span class="sxs-lookup"><span data-stu-id="2ed60-137">Response</span></span>
<span data-ttu-id="2ed60-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2ed60-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

