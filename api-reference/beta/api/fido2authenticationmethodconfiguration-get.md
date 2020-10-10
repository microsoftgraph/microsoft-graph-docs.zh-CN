---
title: 获取 fido2AuthenticationMethodConfiguration
description: 读取 fido2AuthenticationMethodConfiguration 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5411f9c76b6870eccdb43863b5a62380d7caafa3
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418199"
---
# <a name="get-fido2authenticationmethodconfiguration"></a><span data-ttu-id="65077-103">获取 fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="65077-103">Get fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="65077-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65077-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65077-105">检索 [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) 对象的属性和关系，它表示 Azure Active Directory (azure AD) 租户的 FIDO2 安全密钥 [身份验证方法策略](../resources/authenticationmethodspolicies-overview.md) 。</span><span class="sxs-lookup"><span data-stu-id="65077-105">Retrieve the properties and relationships of the [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="65077-106">权限</span><span class="sxs-lookup"><span data-stu-id="65077-106">Permissions</span></span>
<span data-ttu-id="65077-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65077-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65077-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="65077-109">Permission type</span></span>|<span data-ttu-id="65077-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65077-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65077-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65077-111">Delegated (work or school account)</span></span>|<span data-ttu-id="65077-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="65077-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="65077-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65077-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65077-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="65077-114">Not supported.</span></span>|
|<span data-ttu-id="65077-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="65077-115">Application</span></span>|<span data-ttu-id="65077-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="65077-116">Not supported.</span></span>|

<span data-ttu-id="65077-117">对于委派的方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="65077-117">For delegated scenarios the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="65077-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="65077-118">Global admin</span></span>
* <span data-ttu-id="65077-119">全局读取者</span><span class="sxs-lookup"><span data-stu-id="65077-119">Global reader</span></span>
* <span data-ttu-id="65077-120">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="65077-120">Privileged authentication admin</span></span>
* <span data-ttu-id="65077-121">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="65077-121">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="65077-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65077-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="65077-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="65077-123">Request headers</span></span>
|<span data-ttu-id="65077-124">名称</span><span class="sxs-lookup"><span data-stu-id="65077-124">Name</span></span>|<span data-ttu-id="65077-125">说明</span><span class="sxs-lookup"><span data-stu-id="65077-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="65077-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="65077-126">Authorization</span></span>|<span data-ttu-id="65077-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65077-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65077-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="65077-129">Request body</span></span>
<span data-ttu-id="65077-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="65077-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65077-131">响应</span><span class="sxs-lookup"><span data-stu-id="65077-131">Response</span></span>

<span data-ttu-id="65077-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65077-132">If successful, this method returns a `200 OK` response code and a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65077-133">示例</span><span class="sxs-lookup"><span data-stu-id="65077-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65077-134">请求</span><span class="sxs-lookup"><span data-stu-id="65077-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="65077-135">响应</span><span class="sxs-lookup"><span data-stu-id="65077-135">Response</span></span>
<span data-ttu-id="65077-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="65077-136">The following is an example of the response.</span></span>

<span data-ttu-id="65077-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="65077-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "value": {
    "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
    "id": "Fido2",
    "state": "enabled",
    "isSelfServiceRegistrationAllowed": true,
    "isAttestationEnforced": true,
    "keyRestrictions": {
        "isEnforced": false,
        "enforcementType": "block",
        "aaGuids": []
    },
    "includeTargets": [
        {
            "targetType": "group",
            "id": "all_users",
            "isRegistrationRequired": false,
            "useForSignIn": true
        }
    ]
  }
}
```

