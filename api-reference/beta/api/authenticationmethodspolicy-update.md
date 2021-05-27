---
title: 更新 authenticationMethodsPolicy
description: 更新 authenticationMethodsPolicy 对象的属性。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 22630c6651e94faa243e98f275c6d299edd88173
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682875"
---
# <a name="update-authenticationmethodspolicy"></a><span data-ttu-id="85824-103">更新 authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="85824-103">Update authenticationMethodsPolicy</span></span>
<span data-ttu-id="85824-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85824-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85824-105">更新 [authenticationMethodsPolicy 对象](../resources/authenticationmethodspolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="85824-105">Update the properties of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="85824-106">权限</span><span class="sxs-lookup"><span data-stu-id="85824-106">Permissions</span></span>
<span data-ttu-id="85824-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85824-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85824-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="85824-109">Permission type</span></span>|<span data-ttu-id="85824-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="85824-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85824-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85824-111">Delegated (work or school account)</span></span>|<span data-ttu-id="85824-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="85824-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="85824-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85824-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85824-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="85824-114">Not supported.</span></span>|
|<span data-ttu-id="85824-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="85824-115">Application</span></span>|<span data-ttu-id="85824-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="85824-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="85824-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85824-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="85824-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="85824-118">Request headers</span></span>
|<span data-ttu-id="85824-119">名称</span><span class="sxs-lookup"><span data-stu-id="85824-119">Name</span></span>|<span data-ttu-id="85824-120">说明</span><span class="sxs-lookup"><span data-stu-id="85824-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="85824-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="85824-121">Authorization</span></span>|<span data-ttu-id="85824-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="85824-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="85824-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85824-124">Content-Type</span></span>|<span data-ttu-id="85824-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="85824-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85824-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="85824-127">Request body</span></span>
<span data-ttu-id="85824-128">在请求正文中，提供 [registrationEnforcement](../resources/registrationenforcement.md) 对象的 JSON 表示形式，以提示用户设置目标身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="85824-128">In the request body, supply a JSON representation of the [registrationEnforcement](../resources/registrationenforcement.md) object to prompt users to set up targeted authentication methods.</span></span> 

|<span data-ttu-id="85824-129">属性</span><span class="sxs-lookup"><span data-stu-id="85824-129">Property</span></span>|<span data-ttu-id="85824-130">类型</span><span class="sxs-lookup"><span data-stu-id="85824-130">Type</span></span>|<span data-ttu-id="85824-131">说明</span><span class="sxs-lookup"><span data-stu-id="85824-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85824-132">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="85824-132">registrationEnforcement</span></span>|[<span data-ttu-id="85824-133">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="85824-133">registrationEnforcement</span></span>](../resources/registrationenforcement.md)|<span data-ttu-id="85824-134">在登录时强制注册。</span><span class="sxs-lookup"><span data-stu-id="85824-134">Enforce registration at sign-in time.</span></span> <span data-ttu-id="85824-135">此属性可用于提示用户设置目标身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="85824-135">This property can be used to prompt users to set up targeted authentication methods.</span></span>|

## <a name="response"></a><span data-ttu-id="85824-136">响应</span><span class="sxs-lookup"><span data-stu-id="85824-136">Response</span></span>
<span data-ttu-id="85824-137">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="85824-137">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="85824-138">示例</span><span class="sxs-lookup"><span data-stu-id="85824-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85824-139">请求</span><span class="sxs-lookup"><span data-stu-id="85824-139">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="85824-140">响应</span><span class="sxs-lookup"><span data-stu-id="85824-140">Response</span></span>
<span data-ttu-id="85824-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="85824-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
