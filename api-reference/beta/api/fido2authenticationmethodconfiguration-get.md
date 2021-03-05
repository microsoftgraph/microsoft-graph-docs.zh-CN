---
title: 获取 fido2AuthenticationMethodConfiguration
description: 读取 fido2AuthenticationMethodConfiguration 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1c956d838a4edba209766d076b5b792f4b819c84
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471112"
---
# <a name="get-fido2authenticationmethodconfiguration"></a><span data-ttu-id="96d2b-103">获取 fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="96d2b-103">Get fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="96d2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96d2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96d2b-105">检索[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)对象的属性和关系，该对象代表 Azure Active Directory [](../resources/authenticationmethodspolicies-overview.md) (Azure AD) 租户的 FIDO2 安全密钥身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="96d2b-105">Retrieve the properties and relationships of the [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="96d2b-106">权限</span><span class="sxs-lookup"><span data-stu-id="96d2b-106">Permissions</span></span>
<span data-ttu-id="96d2b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96d2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96d2b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="96d2b-109">Permission type</span></span>|<span data-ttu-id="96d2b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96d2b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96d2b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96d2b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="96d2b-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="96d2b-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="96d2b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96d2b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96d2b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="96d2b-114">Not supported.</span></span>|
|<span data-ttu-id="96d2b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="96d2b-115">Application</span></span>|<span data-ttu-id="96d2b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="96d2b-116">Not supported.</span></span>|

<span data-ttu-id="96d2b-117">对于委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="96d2b-117">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="96d2b-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="96d2b-118">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="96d2b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96d2b-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="96d2b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="96d2b-120">Request headers</span></span>
|<span data-ttu-id="96d2b-121">名称</span><span class="sxs-lookup"><span data-stu-id="96d2b-121">Name</span></span>|<span data-ttu-id="96d2b-122">说明</span><span class="sxs-lookup"><span data-stu-id="96d2b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="96d2b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96d2b-123">Authorization</span></span>|<span data-ttu-id="96d2b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96d2b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96d2b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="96d2b-126">Request body</span></span>
<span data-ttu-id="96d2b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96d2b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96d2b-128">响应</span><span class="sxs-lookup"><span data-stu-id="96d2b-128">Response</span></span>

<span data-ttu-id="96d2b-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="96d2b-129">If successful, this method returns a `200 OK` response code and a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96d2b-130">示例</span><span class="sxs-lookup"><span data-stu-id="96d2b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96d2b-131">请求</span><span class="sxs-lookup"><span data-stu-id="96d2b-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="96d2b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="96d2b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```
# <a name="c"></a>[<span data-ttu-id="96d2b-133">C#</span><span class="sxs-lookup"><span data-stu-id="96d2b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96d2b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96d2b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96d2b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96d2b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96d2b-136">Java</span><span class="sxs-lookup"><span data-stu-id="96d2b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fido2authenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="96d2b-137">响应</span><span class="sxs-lookup"><span data-stu-id="96d2b-137">Response</span></span>
<span data-ttu-id="96d2b-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="96d2b-138">The following is an example of the response.</span></span>

<span data-ttu-id="96d2b-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="96d2b-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

