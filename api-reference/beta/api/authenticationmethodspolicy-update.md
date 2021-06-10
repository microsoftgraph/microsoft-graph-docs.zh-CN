---
title: 更新 authenticationMethodsPolicy
description: 更新 authenticationMethodsPolicy 对象的属性。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: cc9c67d5f01d45b1231d1d92922c45c02b3515f4
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869082"
---
# <a name="update-authenticationmethodspolicy"></a><span data-ttu-id="84c1c-103">更新 authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="84c1c-103">Update authenticationMethodsPolicy</span></span>
<span data-ttu-id="84c1c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84c1c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84c1c-105">更新 [authenticationMethodsPolicy 对象](../resources/authenticationmethodspolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="84c1c-105">Update the properties of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="84c1c-106">权限</span><span class="sxs-lookup"><span data-stu-id="84c1c-106">Permissions</span></span>
<span data-ttu-id="84c1c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84c1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84c1c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="84c1c-109">Permission type</span></span>|<span data-ttu-id="84c1c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84c1c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84c1c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84c1c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="84c1c-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="84c1c-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="84c1c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84c1c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84c1c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="84c1c-114">Not supported.</span></span>|
|<span data-ttu-id="84c1c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="84c1c-115">Application</span></span>|<span data-ttu-id="84c1c-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="84c1c-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="84c1c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84c1c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="84c1c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="84c1c-118">Request headers</span></span>
|<span data-ttu-id="84c1c-119">名称</span><span class="sxs-lookup"><span data-stu-id="84c1c-119">Name</span></span>|<span data-ttu-id="84c1c-120">说明</span><span class="sxs-lookup"><span data-stu-id="84c1c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="84c1c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="84c1c-121">Authorization</span></span>|<span data-ttu-id="84c1c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84c1c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="84c1c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="84c1c-124">Content-Type</span></span>|<span data-ttu-id="84c1c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="84c1c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84c1c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="84c1c-127">Request body</span></span>
<span data-ttu-id="84c1c-128">在请求正文中，提供 [registrationEnforcement](../resources/registrationenforcement.md) 对象的 JSON 表示形式，以提示用户设置目标身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="84c1c-128">In the request body, supply a JSON representation of the [registrationEnforcement](../resources/registrationenforcement.md) object to prompt users to set up targeted authentication methods.</span></span> 

|<span data-ttu-id="84c1c-129">属性</span><span class="sxs-lookup"><span data-stu-id="84c1c-129">Property</span></span>|<span data-ttu-id="84c1c-130">类型</span><span class="sxs-lookup"><span data-stu-id="84c1c-130">Type</span></span>|<span data-ttu-id="84c1c-131">说明</span><span class="sxs-lookup"><span data-stu-id="84c1c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84c1c-132">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="84c1c-132">registrationEnforcement</span></span>|[<span data-ttu-id="84c1c-133">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="84c1c-133">registrationEnforcement</span></span>](../resources/registrationenforcement.md)|<span data-ttu-id="84c1c-134">在登录时强制注册。</span><span class="sxs-lookup"><span data-stu-id="84c1c-134">Enforce registration at sign-in time.</span></span> <span data-ttu-id="84c1c-135">此属性可用于提示用户设置目标身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="84c1c-135">This property can be used to prompt users to set up targeted authentication methods.</span></span>|

## <a name="response"></a><span data-ttu-id="84c1c-136">响应</span><span class="sxs-lookup"><span data-stu-id="84c1c-136">Response</span></span>
<span data-ttu-id="84c1c-137">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="84c1c-137">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="84c1c-138">示例</span><span class="sxs-lookup"><span data-stu-id="84c1c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="84c1c-139">请求</span><span class="sxs-lookup"><span data-stu-id="84c1c-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="84c1c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="84c1c-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authenticationmethodspolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy
Content-Type: application/json
Content-length: 293

{
  "registrationEnforcement": {
    "authenticationMethodsRegistrationCampaign": {
        "snoozeDurationInDays": 1,
        "state": "enabled",
        "excludeTargets": [],
        "includeTargets": [
            {
                "id": "3ee3a9de-0a86-4e12-a287-9769accf1ba2",
                "targetType": "group",
                "targetedAuthenticationMethod": "microsoftAuthenticator"
            }
        ]
    }
  }
}
```
# <a name="c"></a>[<span data-ttu-id="84c1c-141">C#</span><span class="sxs-lookup"><span data-stu-id="84c1c-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84c1c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84c1c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84c1c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84c1c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84c1c-144">Java</span><span class="sxs-lookup"><span data-stu-id="84c1c-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="84c1c-145">响应</span><span class="sxs-lookup"><span data-stu-id="84c1c-145">Response</span></span>
<span data-ttu-id="84c1c-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="84c1c-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethodsPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#authenticationMethodsPolicy",
  "id": "authenticationMethodsPolicy",
  "displayName": "Authentication Methods Policy",
  "description": "The tenant-wide policy that controls which authentication methods are allowed in the tenant, authentication method registration requirements, and self-service password reset settings",
  "lastModifiedDateTime": "2021-05-25T01:08:08.6712279Z",
  "policyVersion": "1.4",
  "registrationEnforcement": {
    "authenticationMethodsRegistrationCampaign": {
        "snoozeDurationInDays": 1,
        "state": "enabled",
        "excludeTargets": [],
        "includeTargets": [
            {
                "id": "3ee3a9de-0a86-4e12-a287-9769accf1ba2",
                "targetType": "group",
                "targetedAuthenticationMethod": "microsoftAuthenticator"
            }
        ]
    }
  }
}
```
