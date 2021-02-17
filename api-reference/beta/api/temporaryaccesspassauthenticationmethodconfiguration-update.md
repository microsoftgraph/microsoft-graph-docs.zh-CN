---
title: 更新 temporaryAccessPassAuthenticationMethodConfiguration
description: 更新 temporaryAccessPassAuthenticationMethodConfiguration 对象的属性。
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 868234129fbcaa89d19ac2778c80e8aac6a93aed
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272609"
---
# <a name="update-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="73a62-103">更新 temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="73a62-103">Update temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="73a62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73a62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73a62-105">更新 [临时AccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) 对象的属性，该对象表示 Azure AD 租户的临时访问传递身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="73a62-105">Update the properties of a [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object,  which represents the Temporary Access Pass authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="73a62-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="73a62-106">Permissions</span></span>
<span data-ttu-id="73a62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73a62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73a62-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73a62-109">Permission type</span></span>|<span data-ttu-id="73a62-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73a62-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73a62-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73a62-111">Delegated (work or school account)</span></span>|<span data-ttu-id="73a62-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73a62-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="73a62-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73a62-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73a62-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73a62-114">Not supported.</span></span>|
|<span data-ttu-id="73a62-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="73a62-115">Application</span></span>|<span data-ttu-id="73a62-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73a62-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="73a62-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="73a62-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="73a62-118">有关详细信息，请参阅[角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="73a62-118">For more information, see[roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="73a62-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73a62-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```

## <a name="request-headers"></a><span data-ttu-id="73a62-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="73a62-120">Request headers</span></span>
|<span data-ttu-id="73a62-121">名称</span><span class="sxs-lookup"><span data-stu-id="73a62-121">Name</span></span>|<span data-ttu-id="73a62-122">说明</span><span class="sxs-lookup"><span data-stu-id="73a62-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="73a62-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="73a62-123">Authorization</span></span>|<span data-ttu-id="73a62-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73a62-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="73a62-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73a62-126">Content-Type</span></span>|<span data-ttu-id="73a62-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="73a62-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73a62-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="73a62-129">Request body</span></span>
<span data-ttu-id="73a62-130">在请求正文中，提供 [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) 对象的 JSON 表示形式以及应更新的字段的值。</span><span class="sxs-lookup"><span data-stu-id="73a62-130">In the request body, supply a JSON representation of the [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="73a62-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="73a62-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="73a62-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="73a62-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="73a62-133">对象的所有属性都可以更新。</span><span class="sxs-lookup"><span data-stu-id="73a62-133">All properties of the object can be updated.</span></span> <span data-ttu-id="73a62-134">有关属性的列表，请参阅 [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="73a62-134">For a list of properties, see [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="73a62-135">**注意：**`@odata.type`属性值必须为 `#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration` 1 的属性必须包含在正文中。</span><span class="sxs-lookup"><span data-stu-id="73a62-135">**Note:** The `@odata.type` property with a value of `#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="73a62-136">响应</span><span class="sxs-lookup"><span data-stu-id="73a62-136">Response</span></span>

<span data-ttu-id="73a62-p107">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="73a62-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73a62-139">示例</span><span class="sxs-lookup"><span data-stu-id="73a62-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73a62-140">请求</span><span class="sxs-lookup"><span data-stu-id="73a62-140">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="73a62-141">响应</span><span class="sxs-lookup"><span data-stu-id="73a62-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```