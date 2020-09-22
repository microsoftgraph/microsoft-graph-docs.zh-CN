---
title: 更新 authorizationpolicy
description: 更新 authorizationPolicy 对象的属性。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c6b88a77101c504c6bf2c7979758a73a3755c638
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991584"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="adf16-103">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="adf16-103">Update authorizationPolicy</span></span>

<span data-ttu-id="adf16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adf16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adf16-105">更新 [authorizationPolicy](../resources/authorizationpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="adf16-105">Update the properties of a [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="adf16-106">权限</span><span class="sxs-lookup"><span data-stu-id="adf16-106">Permissions</span></span>

<span data-ttu-id="adf16-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="adf16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="adf16-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="adf16-109">Permission type</span></span>                        | <span data-ttu-id="adf16-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="adf16-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="adf16-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adf16-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="adf16-112">Policy。读身份验证</span><span class="sxs-lookup"><span data-stu-id="adf16-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="adf16-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adf16-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adf16-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="adf16-114">Not supported.</span></span> |
| <span data-ttu-id="adf16-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="adf16-115">Application</span></span>                            | <span data-ttu-id="adf16-116">Policy。读身份验证</span><span class="sxs-lookup"><span data-stu-id="adf16-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="adf16-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adf16-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="adf16-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="adf16-118">Request headers</span></span>

| <span data-ttu-id="adf16-119">名称</span><span class="sxs-lookup"><span data-stu-id="adf16-119">Name</span></span>       | <span data-ttu-id="adf16-120">说明</span><span class="sxs-lookup"><span data-stu-id="adf16-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="adf16-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="adf16-121">Authorization</span></span> | <span data-ttu-id="adf16-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="adf16-122">Bearer {token}</span></span> |
| <span data-ttu-id="adf16-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="adf16-123">Content-type</span></span> | <span data-ttu-id="adf16-124">application/json</span><span class="sxs-lookup"><span data-stu-id="adf16-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="adf16-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="adf16-125">Request body</span></span>

<span data-ttu-id="adf16-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="adf16-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="adf16-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="adf16-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="adf16-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="adf16-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="adf16-129">属性</span><span class="sxs-lookup"><span data-stu-id="adf16-129">Property</span></span>     | <span data-ttu-id="adf16-130">类型</span><span class="sxs-lookup"><span data-stu-id="adf16-130">Type</span></span>        | <span data-ttu-id="adf16-131">说明</span><span class="sxs-lookup"><span data-stu-id="adf16-131">Description</span></span> |
|:-------------|:------------|:------------|  
|<span data-ttu-id="adf16-132">displayName</span><span class="sxs-lookup"><span data-stu-id="adf16-132">displayName</span></span>|<span data-ttu-id="adf16-133">String</span><span class="sxs-lookup"><span data-stu-id="adf16-133">String</span></span>| <span data-ttu-id="adf16-134">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="adf16-134">Display name for this policy.</span></span> |  
|<span data-ttu-id="adf16-135">description</span><span class="sxs-lookup"><span data-stu-id="adf16-135">description</span></span>|<span data-ttu-id="adf16-136">String</span><span class="sxs-lookup"><span data-stu-id="adf16-136">String</span></span>| <span data-ttu-id="adf16-137">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="adf16-137">Description of this policy.</span></span> |  
|<span data-ttu-id="adf16-138">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="adf16-138">guestUserRoleId</span></span>|<span data-ttu-id="adf16-139">Guid</span><span class="sxs-lookup"><span data-stu-id="adf16-139">Guid</span></span>| <span data-ttu-id="adf16-140">表示应向来宾用户授予的角色的角色 templateId。</span><span class="sxs-lookup"><span data-stu-id="adf16-140">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="adf16-141">若要查找可用角色模板的列表，请参阅 [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) 。</span><span class="sxs-lookup"><span data-stu-id="adf16-141">Refer to [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) to find the list of available role templates.</span></span> <span data-ttu-id="adf16-142">目前只有受支持的角色是用户 (a0b1b346-4d3e-4e8b-98f8-753987be4970) 、来宾用户 (10dae51f-b6af-4016-8d66-8c2a99b929b3) 和受限制的来宾用户 (2af84b1e-32c8-42b7-82bc-daa82404023b) 。</span><span class="sxs-lookup"><span data-stu-id="adf16-142">Only supported roles today are User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="adf16-143">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="adf16-143">enabledPreviewFeatures</span></span>|<span data-ttu-id="adf16-144">集合 (字符串) </span><span class="sxs-lookup"><span data-stu-id="adf16-144">Collection(string)</span></span>| <span data-ttu-id="adf16-145">租户上启用了专用预览的功能列表。</span><span class="sxs-lookup"><span data-stu-id="adf16-145">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="adf16-146">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="adf16-146">blockMsolPowerShell</span></span>|<span data-ttu-id="adf16-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf16-147">Boolean</span></span>| <span data-ttu-id="adf16-148">若要禁用 MSOL PowerShell 的使用，请将此属性设置为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="adf16-148">To disable the use of MSOL PowerShell, set this property to `true`.</span></span> <span data-ttu-id="adf16-149">设置为 `true` 将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。</span><span class="sxs-lookup"><span data-stu-id="adf16-149">Setting to `true` will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="adf16-150">这不会影响 Azure AD Connect 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="adf16-150">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="adf16-151">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="adf16-151">defaultUserRolePermissions</span></span>|[<span data-ttu-id="adf16-152">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="adf16-152">defaultUserRolePermissions</span></span>](../resources/defaultUserRolePermissions.md)| <span data-ttu-id="adf16-153">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="adf16-153">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="adf16-154">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="adf16-154">allowedToUseSSPR</span></span>|<span data-ttu-id="adf16-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf16-155">Boolean</span></span>| <span data-ttu-id="adf16-156">指示租户上的用户是否可以使用自助服务密码重置功能。</span><span class="sxs-lookup"><span data-stu-id="adf16-156">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="adf16-157">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="adf16-157">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="adf16-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf16-158">Boolean</span></span>| <span data-ttu-id="adf16-159">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="adf16-159">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="adf16-160">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="adf16-160">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="adf16-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf16-161">Boolean</span></span>| <span data-ttu-id="adf16-162">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="adf16-162">Indicates whether a user can join the tenant by email validation.</span></span> | 

## <a name="response"></a><span data-ttu-id="adf16-163">响应</span><span class="sxs-lookup"><span data-stu-id="adf16-163">Response</span></span>

<span data-ttu-id="adf16-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="adf16-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="adf16-166">示例</span><span class="sxs-lookup"><span data-stu-id="adf16-166">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="adf16-167">示例1：更新或设置租户的来宾用户访问级别</span><span class="sxs-lookup"><span data-stu-id="adf16-167">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="adf16-168">请求</span><span class="sxs-lookup"><span data-stu-id="adf16-168">Request</span></span>

<span data-ttu-id="adf16-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="adf16-169">The following is an example of the request.</span></span> <span data-ttu-id="adf16-170">在此示例中，将来宾访问级别修改为受限制的来宾用户。</span><span class="sxs-lookup"><span data-stu-id="adf16-170">In this example, guest access level is modified to Restricted Guest User.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_guestUserLevel"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
  "guestUserRole": "2af84b1e-32c8-42b7-82bc-daa82404023b"
}

```
#### <a name="response"></a><span data-ttu-id="adf16-171">响应</span><span class="sxs-lookup"><span data-stu-id="adf16-171">Response</span></span>

<span data-ttu-id="adf16-172">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="adf16-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content

```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a><span data-ttu-id="adf16-173">示例2：在租户上为预览启用新功能</span><span class="sxs-lookup"><span data-stu-id="adf16-173">Example 2: Enable new feature for preview on tenant</span></span>

#### <a name="request"></a><span data-ttu-id="adf16-174">请求</span><span class="sxs-lookup"><span data-stu-id="adf16-174">Request</span></span>

<span data-ttu-id="adf16-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="adf16-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="adf16-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="adf16-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_preview"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
  "enabledPreviewFeatures": ["assignGroupsToRoles"]
}

```
# <a name="c"></a>[<span data-ttu-id="adf16-177">C#</span><span class="sxs-lookup"><span data-stu-id="adf16-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-preview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adf16-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adf16-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-preview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adf16-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adf16-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-preview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="adf16-180">响应</span><span class="sxs-lookup"><span data-stu-id="adf16-180">Response</span></span>

<span data-ttu-id="adf16-181">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="adf16-181">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```


### <a name="example-3-block-msol-powershell-in-tenant"></a><span data-ttu-id="adf16-182">示例3：阻止租户中的 MSOL PowerShell</span><span class="sxs-lookup"><span data-stu-id="adf16-182">Example 3: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="adf16-183">请求</span><span class="sxs-lookup"><span data-stu-id="adf16-183">Request</span></span>

<span data-ttu-id="adf16-184">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="adf16-184">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="adf16-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="adf16-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_blockMSOLPowerShell"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
  "blockMsolPowerShell": true
}

```
# <a name="c"></a>[<span data-ttu-id="adf16-186">C#</span><span class="sxs-lookup"><span data-stu-id="adf16-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adf16-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adf16-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adf16-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adf16-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="adf16-189">响应</span><span class="sxs-lookup"><span data-stu-id="adf16-189">Response</span></span>

<span data-ttu-id="adf16-190">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="adf16-190">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-4-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="adf16-191">示例4：禁用默认用户角色的权限以创建应用程序</span><span class="sxs-lookup"><span data-stu-id="adf16-191">Example 4: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="adf16-192">请求</span><span class="sxs-lookup"><span data-stu-id="adf16-192">Request</span></span>

<span data-ttu-id="adf16-193">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="adf16-193">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="adf16-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="adf16-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_applications"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
    "defaultUserRolePermissions":
    {
      "allowedToCreateApps": false
    }
}

```
# <a name="c"></a>[<span data-ttu-id="adf16-195">C#</span><span class="sxs-lookup"><span data-stu-id="adf16-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adf16-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adf16-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adf16-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adf16-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="adf16-198">响应</span><span class="sxs-lookup"><span data-stu-id="adf16-198">Response</span></span>

<span data-ttu-id="adf16-199">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="adf16-199">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="adf16-200">示例5：启用默认用户角色以使用自助密码重置功能</span><span class="sxs-lookup"><span data-stu-id="adf16-200">Example 5: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="adf16-201">请求</span><span class="sxs-lookup"><span data-stu-id="adf16-201">Request</span></span>

<span data-ttu-id="adf16-202">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="adf16-202">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="adf16-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="adf16-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_SSPR"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
    "allowedToUseSSPR": true
}

```
# <a name="c"></a>[<span data-ttu-id="adf16-204">C#</span><span class="sxs-lookup"><span data-stu-id="adf16-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adf16-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adf16-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adf16-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adf16-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="adf16-207">响应</span><span class="sxs-lookup"><span data-stu-id="adf16-207">Response</span></span>

<span data-ttu-id="adf16-208">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="adf16-208">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```


