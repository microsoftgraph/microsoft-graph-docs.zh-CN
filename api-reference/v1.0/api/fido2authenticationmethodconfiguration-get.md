---
title: 获取 fido2AuthenticationMethodConfiguration
description: 读取 fido2AuthenticationMethodConfiguration 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b517d9e8577c52b94f9f5bec301dc92495d00031
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964652"
---
# <a name="get-fido2authenticationmethodconfiguration"></a><span data-ttu-id="5c8d4-103">获取 fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c8d4-103">Get fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="5c8d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c8d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5c8d4-105">检索[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)对象的属性和关系，该对象表示 Azure Active Directory[](../resources/authenticationmethodspolicies-overview.md)租户的 FIDO2 安全密钥 (Azure AD) 策略。</span><span class="sxs-lookup"><span data-stu-id="5c8d4-105">Retrieve the properties and relationships of the [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c8d4-106">权限</span><span class="sxs-lookup"><span data-stu-id="5c8d4-106">Permissions</span></span>
<span data-ttu-id="5c8d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c8d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c8d4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c8d4-109">Permission type</span></span>|<span data-ttu-id="5c8d4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c8d4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c8d4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c8d4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c8d4-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5c8d4-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="5c8d4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c8d4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c8d4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c8d4-114">Not supported.</span></span>|
|<span data-ttu-id="5c8d4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c8d4-115">Application</span></span>|<span data-ttu-id="5c8d4-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5c8d4-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="5c8d4-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="5c8d4-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="5c8d4-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="5c8d4-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="5c8d4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c8d4-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="5c8d4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c8d4-120">Request headers</span></span>
|<span data-ttu-id="5c8d4-121">名称</span><span class="sxs-lookup"><span data-stu-id="5c8d4-121">Name</span></span>|<span data-ttu-id="5c8d4-122">说明</span><span class="sxs-lookup"><span data-stu-id="5c8d4-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5c8d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c8d4-123">Authorization</span></span>|<span data-ttu-id="5c8d4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5c8d4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c8d4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c8d4-126">Request body</span></span>
<span data-ttu-id="5c8d4-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5c8d4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c8d4-128">响应</span><span class="sxs-lookup"><span data-stu-id="5c8d4-128">Response</span></span>

<span data-ttu-id="5c8d4-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5c8d4-129">If successful, this method returns a `200 OK` response code and a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c8d4-130">示例</span><span class="sxs-lookup"><span data-stu-id="5c8d4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c8d4-131">请求</span><span class="sxs-lookup"><span data-stu-id="5c8d4-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="5c8d4-132">响应</span><span class="sxs-lookup"><span data-stu-id="5c8d4-132">Response</span></span>
<span data-ttu-id="5c8d4-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5c8d4-133">The following is an example of the response.</span></span>

<span data-ttu-id="5c8d4-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5c8d4-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fido2AuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "value":{
      "@odata.type":"#microsoft.graph.fido2AuthenticationMethodConfiguration",
      "id":"Fido2",
      "state":"enabled",
      "isSelfServiceRegistrationAllowed":true,
      "isAttestationEnforced":true,
      "keyRestrictions":{
         "isEnforced":false,
         "enforcementType":"block",
         "aaGuids":[
            
         ]
      },
      "includeTargets":[
         {
            "targetType":"group",
            "id":"all_users",
            "isRegistrationRequired":false,
            "useForSignIn":true
         }
      ]
   }
}
```

