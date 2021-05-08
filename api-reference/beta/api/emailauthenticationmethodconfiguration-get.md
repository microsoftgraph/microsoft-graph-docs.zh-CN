---
title: 获取 emailAuthenticationMethodConfiguration
description: 读取 emailAuthenticationMethodConfiguration 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9f0b19a44998134d9b4fc1b3d25b194c10ed80e4
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231380"
---
# <a name="get-emailauthenticationmethodconfiguration"></a><span data-ttu-id="d0ef9-103">获取 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0ef9-103">Get emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="d0ef9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0ef9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0ef9-105">读取[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)对象的属性和关系，该对象表示 Azure Active Directory (Azure AD 租户的电子邮件[OTP](../resources/authenticationmethodspolicies-overview.md)) 策略。</span><span class="sxs-lookup"><span data-stu-id="d0ef9-105">Read the properties and relationships of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0ef9-106">权限</span><span class="sxs-lookup"><span data-stu-id="d0ef9-106">Permissions</span></span>

<span data-ttu-id="d0ef9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0ef9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0ef9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0ef9-109">Permission type</span></span>|<span data-ttu-id="d0ef9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0ef9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0ef9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0ef9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d0ef9-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d0ef9-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="d0ef9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0ef9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0ef9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0ef9-114">Not supported.</span></span>|
|<span data-ttu-id="d0ef9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0ef9-115">Application</span></span>|<span data-ttu-id="d0ef9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0ef9-116">Not supported.</span></span>|

<span data-ttu-id="d0ef9-117">对于委派方案，管理员需要以下角色之 [一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="d0ef9-117">For delegated scenarios the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="d0ef9-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="d0ef9-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="d0ef9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0ef9-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="d0ef9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0ef9-120">Request headers</span></span>

|<span data-ttu-id="d0ef9-121">名称</span><span class="sxs-lookup"><span data-stu-id="d0ef9-121">Name</span></span>|<span data-ttu-id="d0ef9-122">说明</span><span class="sxs-lookup"><span data-stu-id="d0ef9-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d0ef9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0ef9-123">Authorization</span></span>|<span data-ttu-id="d0ef9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0ef9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0ef9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0ef9-126">Request body</span></span>

<span data-ttu-id="d0ef9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d0ef9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0ef9-128">响应</span><span class="sxs-lookup"><span data-stu-id="d0ef9-128">Response</span></span>

<span data-ttu-id="d0ef9-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0ef9-129">If successful, this method returns a `200 OK` response code and an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0ef9-130">示例</span><span class="sxs-lookup"><span data-stu-id="d0ef9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0ef9-131">请求</span><span class="sxs-lookup"><span data-stu-id="d0ef9-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d0ef9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0ef9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethodconfiguration"
}
-->

```msgraph-interactive
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```
# <a name="c"></a>[<span data-ttu-id="d0ef9-133">C#</span><span class="sxs-lookup"><span data-stu-id="d0ef9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0ef9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0ef9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0ef9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0ef9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0ef9-136">Java</span><span class="sxs-lookup"><span data-stu-id="d0ef9-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d0ef9-137">响应</span><span class="sxs-lookup"><span data-stu-id="d0ef9-137">Response</span></span>

<span data-ttu-id="d0ef9-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d0ef9-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
   "value":{
      "@odata.type":"#microsoft.graph.emailAuthenticationMethodConfiguration",
      "id":"Email",
      "state":"enabled",
      "allowExternalIdToUseEmailOtp":"enabled",
      "includeTargets":[
         {
            "targetType":"group",
            "id":"all_users",
            "isRegistrationRequired":false
         }
      ]
   }
}
```

