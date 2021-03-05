---
title: 更新 smsAuthenticationMethodConfiguration
description: 更新 smsAuthenticationMethodConfiguration 对象的属性。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbdcddf77f2e85517b6c8d1685b4129b1e8d83f0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475596"
---
# <a name="update-smsauthenticationmethodconfiguration"></a><span data-ttu-id="5989f-103">更新 smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="5989f-103">Update smsAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="5989f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5989f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5989f-105">更新 [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) 对象的属性，该对象代表 Azure AD 租户的文本消息身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="5989f-105">Update the properties of a [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object, which represents the Text Message authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5989f-106">权限</span><span class="sxs-lookup"><span data-stu-id="5989f-106">Permissions</span></span>
<span data-ttu-id="5989f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5989f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5989f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5989f-109">Permission type</span></span>|<span data-ttu-id="5989f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5989f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5989f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5989f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5989f-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5989f-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="5989f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5989f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5989f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5989f-114">Not supported.</span></span>|
|<span data-ttu-id="5989f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5989f-115">Application</span></span>|<span data-ttu-id="5989f-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5989f-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="5989f-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="5989f-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="5989f-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="5989f-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="5989f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5989f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
```

## <a name="request-headers"></a><span data-ttu-id="5989f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5989f-120">Request headers</span></span>
|<span data-ttu-id="5989f-121">名称</span><span class="sxs-lookup"><span data-stu-id="5989f-121">Name</span></span>|<span data-ttu-id="5989f-122">说明</span><span class="sxs-lookup"><span data-stu-id="5989f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5989f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5989f-123">Authorization</span></span>|<span data-ttu-id="5989f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5989f-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5989f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5989f-126">Content-Type</span></span>|<span data-ttu-id="5989f-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5989f-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5989f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5989f-129">Request body</span></span>
<span data-ttu-id="5989f-130">在请求正文中，提供 [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) 对象的 JSON 表示形式以及应更新的字段的值。</span><span class="sxs-lookup"><span data-stu-id="5989f-130">In the request body, supply a JSON representation of the [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="5989f-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="5989f-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5989f-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5989f-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="5989f-133">下表显示更新 [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) 对象时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5989f-133">The following table shows the properties that are required when you update the [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object.</span></span>

|<span data-ttu-id="5989f-134">属性</span><span class="sxs-lookup"><span data-stu-id="5989f-134">Property</span></span>|<span data-ttu-id="5989f-135">类型</span><span class="sxs-lookup"><span data-stu-id="5989f-135">Type</span></span>|<span data-ttu-id="5989f-136">说明</span><span class="sxs-lookup"><span data-stu-id="5989f-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5989f-137">id</span><span class="sxs-lookup"><span data-stu-id="5989f-137">id</span></span>|<span data-ttu-id="5989f-138">String</span><span class="sxs-lookup"><span data-stu-id="5989f-138">String</span></span>|<span data-ttu-id="5989f-139">身份验证方法策略标识符。</span><span class="sxs-lookup"><span data-stu-id="5989f-139">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="5989f-140">state</span><span class="sxs-lookup"><span data-stu-id="5989f-140">state</span></span>|<span data-ttu-id="5989f-141">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="5989f-141">authenticationMethodState</span></span>|<span data-ttu-id="5989f-142">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="5989f-142">Possible values are: `enabled`, `disabled`.</span></span>|

><span data-ttu-id="5989f-143">**注意：**`@odata.type`属性值必须为 `#microsoft.graph.smsAuthenticationMethodConfiguration` 1 的属性必须包含在正文中。</span><span class="sxs-lookup"><span data-stu-id="5989f-143">**Note:** The `@odata.type` property with a value of `#microsoft.graph.smsAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="5989f-144">响应</span><span class="sxs-lookup"><span data-stu-id="5989f-144">Response</span></span>

<span data-ttu-id="5989f-145">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5989f-145">If successful, this method returns a `200 OK` response code and an updated [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5989f-146">示例</span><span class="sxs-lookup"><span data-stu-id="5989f-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5989f-147">请求</span><span class="sxs-lookup"><span data-stu-id="5989f-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5989f-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="5989f-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_smsauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
Content-Type: application/json
Content-length: 100

{
    "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
    "id": "Sms",
    "state": "enabled"
}
```
# <a name="c"></a>[<span data-ttu-id="5989f-149">C#</span><span class="sxs-lookup"><span data-stu-id="5989f-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-smsauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5989f-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5989f-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-smsauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5989f-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5989f-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-smsauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5989f-152">Java</span><span class="sxs-lookup"><span data-stu-id="5989f-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-smsauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5989f-153">响应</span><span class="sxs-lookup"><span data-stu-id="5989f-153">Response</span></span>
<span data-ttu-id="5989f-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5989f-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.smsAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
  "id": "713980c7-80c7-7139-c780-3971c7803971",
  "state": "String"
}
```

