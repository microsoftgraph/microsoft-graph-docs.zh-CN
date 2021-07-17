---
title: 获取 emailAuthenticationMethodConfiguration
description: 读取 emailAuthenticationMethodConfiguration 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 15aa3de4b66b566c1943709330478d035ead0977
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442926"
---
# <a name="get-emailauthenticationmethodconfiguration"></a><span data-ttu-id="2f866-103">获取 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f866-103">Get emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="2f866-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f866-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2f866-105">读取[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)对象的属性和关系，该对象表示 Azure Active Directory (Azure AD 租户的电子邮件[OTP](../resources/authenticationmethodspolicies-overview.md)) 策略。</span><span class="sxs-lookup"><span data-stu-id="2f866-105">Read the properties and relationships of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f866-106">权限</span><span class="sxs-lookup"><span data-stu-id="2f866-106">Permissions</span></span>

<span data-ttu-id="2f866-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f866-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f866-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f866-109">Permission type</span></span>|<span data-ttu-id="2f866-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f866-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f866-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f866-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f866-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2f866-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="2f866-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f866-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f866-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f866-114">Not supported.</span></span>|
|<span data-ttu-id="2f866-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f866-115">Application</span></span>|<span data-ttu-id="2f866-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2f866-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="2f866-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="2f866-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="2f866-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="2f866-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="2f866-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f866-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="2f866-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f866-120">Request headers</span></span>

|<span data-ttu-id="2f866-121">名称</span><span class="sxs-lookup"><span data-stu-id="2f866-121">Name</span></span>|<span data-ttu-id="2f866-122">说明</span><span class="sxs-lookup"><span data-stu-id="2f866-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2f866-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f866-123">Authorization</span></span>|<span data-ttu-id="2f866-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f866-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f866-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f866-126">Request body</span></span>

<span data-ttu-id="2f866-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2f866-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f866-128">响应</span><span class="sxs-lookup"><span data-stu-id="2f866-128">Response</span></span>

<span data-ttu-id="2f866-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f866-129">If successful, this method returns a `200 OK` response code and an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f866-130">示例</span><span class="sxs-lookup"><span data-stu-id="2f866-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f866-131">请求</span><span class="sxs-lookup"><span data-stu-id="2f866-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2f866-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f866-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethodconfiguration"
}
-->

```msgraph-interactive
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```
# <a name="c"></a>[<span data-ttu-id="2f866-133">C#</span><span class="sxs-lookup"><span data-stu-id="2f866-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f866-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f866-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f866-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f866-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f866-136">Java</span><span class="sxs-lookup"><span data-stu-id="2f866-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2f866-137">响应</span><span class="sxs-lookup"><span data-stu-id="2f866-137">Response</span></span>

<span data-ttu-id="2f866-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2f866-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethodConfiguration"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 491

{
  "value": {
    "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
    "id": "Email",
    "state": "enabled",
    "allowExternalIdToUseEmailOtp": "enabled"
  }
}
```
