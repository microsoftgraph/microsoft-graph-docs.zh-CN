---
title: 更新 emailAuthenticationMethodConfiguration
description: 更新 emailAuthenticationMethodConfiguration 对象的属性。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d2cdf7eeff97bc8bf28edb1fd4e139922cafa472
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231345"
---
# <a name="update-emailauthenticationmethodconfiguration"></a><span data-ttu-id="eae86-103">更新 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="eae86-103">Update emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="eae86-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eae86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eae86-105">更新[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)对象的属性，该对象表示 Azure Active Directory (Azure AD 租户的电子邮件[OTP](../resources/authenticationmethodspolicies-overview.md)) 策略。</span><span class="sxs-lookup"><span data-stu-id="eae86-105">Update the properties of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="eae86-106">权限</span><span class="sxs-lookup"><span data-stu-id="eae86-106">Permissions</span></span>
<span data-ttu-id="eae86-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eae86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eae86-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eae86-109">Permission type</span></span>|<span data-ttu-id="eae86-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eae86-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eae86-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eae86-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eae86-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="eae86-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="eae86-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eae86-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eae86-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eae86-114">Not supported.</span></span>|
|<span data-ttu-id="eae86-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eae86-115">Application</span></span>|<span data-ttu-id="eae86-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eae86-116">Not supported.</span></span>|

<span data-ttu-id="eae86-117">对于委派方案，管理员需要以下角色之 [一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="eae86-117">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="eae86-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="eae86-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="eae86-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eae86-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="eae86-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eae86-120">Request headers</span></span>

|<span data-ttu-id="eae86-121">名称</span><span class="sxs-lookup"><span data-stu-id="eae86-121">Name</span></span>|<span data-ttu-id="eae86-122">说明</span><span class="sxs-lookup"><span data-stu-id="eae86-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eae86-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eae86-123">Authorization</span></span>|<span data-ttu-id="eae86-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eae86-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="eae86-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eae86-126">Content-Type</span></span>|<span data-ttu-id="eae86-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="eae86-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eae86-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="eae86-129">Request body</span></span>

<span data-ttu-id="eae86-130">在请求正文中，提供 [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eae86-130">In the request body, supply a JSON representation of the [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object.</span></span> <span data-ttu-id="eae86-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="eae86-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="eae86-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="eae86-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="eae86-133">有关可更新的属性的列表，请参阅 [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="eae86-133">For the list of properties that can be updated, see [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="eae86-134">**注意：**`@odata.type`属性值为 的 `#microsoft.graph.emailAuthenticationMethodConfiguration` 属性必须包含在正文中。</span><span class="sxs-lookup"><span data-stu-id="eae86-134">**Note:** The `@odata.type` property with a value of `#microsoft.graph.emailAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="eae86-135">响应</span><span class="sxs-lookup"><span data-stu-id="eae86-135">Response</span></span>

<span data-ttu-id="eae86-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="eae86-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eae86-138">示例</span><span class="sxs-lookup"><span data-stu-id="eae86-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eae86-139">请求</span><span class="sxs-lookup"><span data-stu-id="eae86-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eae86-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="eae86-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_emailauthenticationmethodconfiguration"
}
-->

```http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
Content-Type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "allowExternalIdToUseEmailOtp": "disabled",
}
```
# <a name="c"></a>[<span data-ttu-id="eae86-141">C#</span><span class="sxs-lookup"><span data-stu-id="eae86-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-emailauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eae86-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eae86-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-emailauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eae86-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eae86-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-emailauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eae86-144">Java</span><span class="sxs-lookup"><span data-stu-id="eae86-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-emailauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eae86-145">响应</span><span class="sxs-lookup"><span data-stu-id="eae86-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 NO CONTENT
```

