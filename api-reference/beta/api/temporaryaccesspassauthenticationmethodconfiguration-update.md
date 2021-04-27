---
title: 更新 temporaryAccessPassAuthenticationMethodConfiguration
description: 更新 temporaryAccessPassAuthenticationMethodConfiguration 对象的属性。
author: inbarckms
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6cd30c6016739fcb40c3d6541b1fd1b03f72bee6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049637"
---
# <a name="update-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="e35c3-103">更新 temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="e35c3-103">Update temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="e35c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e35c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e35c3-105">更新 [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) 对象的属性，该对象表示 Azure AD 租户的临时访问传递身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="e35c3-105">Update the properties of a [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object,  which represents the Temporary Access Pass authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e35c3-106">权限</span><span class="sxs-lookup"><span data-stu-id="e35c3-106">Permissions</span></span>
<span data-ttu-id="e35c3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e35c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e35c3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e35c3-109">Permission type</span></span>|<span data-ttu-id="e35c3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e35c3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e35c3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e35c3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e35c3-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e35c3-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="e35c3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e35c3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e35c3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e35c3-114">Not supported.</span></span>|
|<span data-ttu-id="e35c3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e35c3-115">Application</span></span>|<span data-ttu-id="e35c3-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e35c3-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="e35c3-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="e35c3-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="e35c3-118">有关详细信息，请参阅[角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="e35c3-118">For more information, see[roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="e35c3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e35c3-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```

## <a name="request-headers"></a><span data-ttu-id="e35c3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e35c3-120">Request headers</span></span>
|<span data-ttu-id="e35c3-121">名称</span><span class="sxs-lookup"><span data-stu-id="e35c3-121">Name</span></span>|<span data-ttu-id="e35c3-122">说明</span><span class="sxs-lookup"><span data-stu-id="e35c3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e35c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e35c3-123">Authorization</span></span>|<span data-ttu-id="e35c3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e35c3-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e35c3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e35c3-126">Content-Type</span></span>|<span data-ttu-id="e35c3-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e35c3-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e35c3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e35c3-129">Request body</span></span>
<span data-ttu-id="e35c3-130">在请求正文中，提供 [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) 对象的 JSON 表示形式以及应更新的字段的值。</span><span class="sxs-lookup"><span data-stu-id="e35c3-130">In the request body, supply a JSON representation of the [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="e35c3-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="e35c3-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e35c3-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e35c3-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="e35c3-133">对象的所有属性都可以更新。</span><span class="sxs-lookup"><span data-stu-id="e35c3-133">All properties of the object can be updated.</span></span> <span data-ttu-id="e35c3-134">有关属性的列表，请参阅 [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="e35c3-134">For a list of properties, see [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="e35c3-135">**注意：**`@odata.type`属性值为 的 `#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration` 属性必须包含在正文中。</span><span class="sxs-lookup"><span data-stu-id="e35c3-135">**Note:** The `@odata.type` property with a value of `#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="e35c3-136">响应</span><span class="sxs-lookup"><span data-stu-id="e35c3-136">Response</span></span>

<span data-ttu-id="e35c3-p107">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e35c3-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e35c3-139">示例</span><span class="sxs-lookup"><span data-stu-id="e35c3-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e35c3-140">请求</span><span class="sxs-lookup"><span data-stu-id="e35c3-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e35c3-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e35c3-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_temporaryaccesspassauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
Content-Type: application/json

{
  "@odata.type":"#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
  "state":"enabled",
  "defaultLifetimeInMinutes":60,
  "defaultLength":8,
  "minimumLifetimeInMinutes":60,
  "maximumLifetimeInMinutes":1440,"
  isUsableOnce":false,
  "includeTargets": [
        {
            "targetType": "group",
            "id": "all_users",
            "isRegistrationRequired": false,
            "useForSignIn": true
        }
    ]
}


```
# <a name="javascript"></a>[<span data-ttu-id="e35c3-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e35c3-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-temporaryaccesspassauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e35c3-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e35c3-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-temporaryaccesspassauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e35c3-144">Java</span><span class="sxs-lookup"><span data-stu-id="e35c3-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-temporaryaccesspassauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e35c3-145">响应</span><span class="sxs-lookup"><span data-stu-id="e35c3-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
