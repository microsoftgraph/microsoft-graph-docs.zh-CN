---
title: 更新 fido2AuthenticationMethodConfiguration
description: 更新 fido2AuthenticationMethodConfiguration 对象的属性。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 93ea4ad235ba58df44c33be8c64beaa294557628
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435991"
---
# <a name="update-fido2authenticationmethodconfiguration"></a><span data-ttu-id="c8f12-103">更新 fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="c8f12-103">Update fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="c8f12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8f12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8f12-105">更新 [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) 对象的属性，该对象代表 Azure AD 租户的 FIDO2 安全密钥身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="c8f12-105">Update the properties of a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8f12-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c8f12-106">Permissions</span></span>
<span data-ttu-id="c8f12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8f12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8f12-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8f12-109">Permission type</span></span>|<span data-ttu-id="c8f12-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8f12-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8f12-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8f12-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c8f12-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c8f12-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="c8f12-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8f12-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8f12-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8f12-114">Not supported.</span></span>|
|<span data-ttu-id="c8f12-115">Application</span><span class="sxs-lookup"><span data-stu-id="c8f12-115">Application</span></span>|<span data-ttu-id="c8f12-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8f12-116">Not supported.</span></span>|

<span data-ttu-id="c8f12-117">对于委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="c8f12-117">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="c8f12-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="c8f12-118">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="c8f12-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8f12-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="c8f12-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8f12-120">Request headers</span></span>
|<span data-ttu-id="c8f12-121">名称</span><span class="sxs-lookup"><span data-stu-id="c8f12-121">Name</span></span>|<span data-ttu-id="c8f12-122">说明</span><span class="sxs-lookup"><span data-stu-id="c8f12-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c8f12-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8f12-123">Authorization</span></span>|<span data-ttu-id="c8f12-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8f12-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c8f12-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c8f12-126">Content-Type</span></span>|<span data-ttu-id="c8f12-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c8f12-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8f12-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8f12-129">Request body</span></span>
<span data-ttu-id="c8f12-130">在请求正文中，提供 [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) 对象的 JSON 表示形式以及应更新的字段的值。</span><span class="sxs-lookup"><span data-stu-id="c8f12-130">In the request body, supply a JSON representation of a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="c8f12-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="c8f12-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c8f12-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c8f12-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="c8f12-133">有关可更新的属性的列表，请参阅 [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c8f12-133">For the list of properties that can be updated, see [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="c8f12-134">**注意：**`@odata.type`属性值必须为 `#microsoft.graph.fido2AuthenticationMethodConfiguration` 1 的属性必须包含在正文中。</span><span class="sxs-lookup"><span data-stu-id="c8f12-134">**Note:** The `@odata.type` property with a value of `#microsoft.graph.fido2AuthenticationMethodConfiguration` must be included in the body.</span></span>


## <a name="response"></a><span data-ttu-id="c8f12-135">响应</span><span class="sxs-lookup"><span data-stu-id="c8f12-135">Response</span></span>

<span data-ttu-id="c8f12-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c8f12-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8f12-138">示例</span><span class="sxs-lookup"><span data-stu-id="c8f12-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8f12-139">请求</span><span class="sxs-lookup"><span data-stu-id="c8f12-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_fido2authenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
    "state": "enabled",
    "isAttestationEnforced": "true"
}
```


### <a name="response"></a><span data-ttu-id="c8f12-140">响应</span><span class="sxs-lookup"><span data-stu-id="c8f12-140">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

