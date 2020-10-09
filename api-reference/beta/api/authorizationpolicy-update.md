---
title: 更新 authorizationpolicy
description: 更新 authorizationPolicy 对象的属性。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3a51767eb02765b3c6914d8b04c5758202b3df1f
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401902"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="a038b-103">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="a038b-103">Update authorizationPolicy</span></span>

<span data-ttu-id="a038b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a038b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a038b-105">更新 [authorizationPolicy](../resources/authorizationpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a038b-105">Update the properties of a [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a038b-106">权限</span><span class="sxs-lookup"><span data-stu-id="a038b-106">Permissions</span></span>

<span data-ttu-id="a038b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a038b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a038b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a038b-109">Permission type</span></span>                        | <span data-ttu-id="a038b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a038b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a038b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a038b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a038b-112">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="a038b-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="a038b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a038b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a038b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a038b-114">Not supported.</span></span> |
| <span data-ttu-id="a038b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a038b-115">Application</span></span>                            | <span data-ttu-id="a038b-116">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="a038b-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="a038b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a038b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="a038b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a038b-118">Request headers</span></span>

| <span data-ttu-id="a038b-119">名称</span><span class="sxs-lookup"><span data-stu-id="a038b-119">Name</span></span>       | <span data-ttu-id="a038b-120">说明</span><span class="sxs-lookup"><span data-stu-id="a038b-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a038b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a038b-121">Authorization</span></span> | <span data-ttu-id="a038b-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="a038b-122">Bearer {token}</span></span> |
| <span data-ttu-id="a038b-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="a038b-123">Content-type</span></span> | <span data-ttu-id="a038b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a038b-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a038b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a038b-125">Request body</span></span>

<span data-ttu-id="a038b-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="a038b-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a038b-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="a038b-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a038b-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a038b-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a038b-129">属性</span><span class="sxs-lookup"><span data-stu-id="a038b-129">Property</span></span>     | <span data-ttu-id="a038b-130">类型</span><span class="sxs-lookup"><span data-stu-id="a038b-130">Type</span></span>        | <span data-ttu-id="a038b-131">说明</span><span class="sxs-lookup"><span data-stu-id="a038b-131">Description</span></span> |
|:-------------|:------------|:------------|  
|<span data-ttu-id="a038b-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a038b-132">displayName</span></span>|<span data-ttu-id="a038b-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a038b-133">String</span></span>| <span data-ttu-id="a038b-134">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a038b-134">Display name for this policy.</span></span> |  
|<span data-ttu-id="a038b-135">说明</span><span class="sxs-lookup"><span data-stu-id="a038b-135">description</span></span>|<span data-ttu-id="a038b-136">字符串</span><span class="sxs-lookup"><span data-stu-id="a038b-136">String</span></span>| <span data-ttu-id="a038b-137">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="a038b-137">Description of this policy.</span></span> |  
|<span data-ttu-id="a038b-138">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="a038b-138">guestUserRoleId</span></span>|<span data-ttu-id="a038b-139">Guid</span><span class="sxs-lookup"><span data-stu-id="a038b-139">Guid</span></span>| <span data-ttu-id="a038b-140">表示应向来宾用户授予的角色的角色 templateId。</span><span class="sxs-lookup"><span data-stu-id="a038b-140">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="a038b-141">若要查找可用角色模板的列表，请参阅 [List unifiedRoleDefinitions](./rbacapplication-list-roledefinitions.md) 。</span><span class="sxs-lookup"><span data-stu-id="a038b-141">Refer to [List unifiedRoleDefinitions](./rbacapplication-list-roledefinitions.md) to find the list of available role templates.</span></span> <span data-ttu-id="a038b-142">目前只有受支持的角色是用户 (a0b1b346-4d3e-4e8b-98f8-753987be4970) 、来宾用户 (10dae51f-b6af-4016-8d66-8c2a99b929b3) 和受限制的来宾用户 (2af84b1e-32c8-42b7-82bc-daa82404023b) 。</span><span class="sxs-lookup"><span data-stu-id="a038b-142">Only supported roles today are User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="a038b-143">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="a038b-143">enabledPreviewFeatures</span></span>|<span data-ttu-id="a038b-144">集合 (字符串) </span><span class="sxs-lookup"><span data-stu-id="a038b-144">Collection(string)</span></span>| <span data-ttu-id="a038b-145">租户上启用了专用预览的功能列表。</span><span class="sxs-lookup"><span data-stu-id="a038b-145">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="a038b-146">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="a038b-146">blockMsolPowerShell</span></span>|<span data-ttu-id="a038b-147">布尔</span><span class="sxs-lookup"><span data-stu-id="a038b-147">Boolean</span></span>| <span data-ttu-id="a038b-148">若要禁用 MSOL PowerShell 的使用，请将此属性设置为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="a038b-148">To disable the use of MSOL PowerShell, set this property to `true`.</span></span> <span data-ttu-id="a038b-149">设置为 `true` 将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。</span><span class="sxs-lookup"><span data-stu-id="a038b-149">Setting to `true` will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="a038b-150">这不会影响 Azure AD Connect 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="a038b-150">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="a038b-151">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="a038b-151">defaultUserRolePermissions</span></span>|[<span data-ttu-id="a038b-152">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="a038b-152">defaultUserRolePermissions</span></span>](../resources/defaultUserRolePermissions.md)| <span data-ttu-id="a038b-153">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="a038b-153">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="a038b-154">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="a038b-154">allowedToUseSSPR</span></span>|<span data-ttu-id="a038b-155">布尔</span><span class="sxs-lookup"><span data-stu-id="a038b-155">Boolean</span></span>| <span data-ttu-id="a038b-156">指示租户上的用户是否可以使用 Self-Serve 密码重置功能。</span><span class="sxs-lookup"><span data-stu-id="a038b-156">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="a038b-157">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="a038b-157">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="a038b-158">布尔</span><span class="sxs-lookup"><span data-stu-id="a038b-158">Boolean</span></span>| <span data-ttu-id="a038b-159">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="a038b-159">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="a038b-160">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="a038b-160">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="a038b-161">布尔</span><span class="sxs-lookup"><span data-stu-id="a038b-161">Boolean</span></span>| <span data-ttu-id="a038b-162">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="a038b-162">Indicates whether a user can join the tenant by email validation.</span></span> |
| <span data-ttu-id="a038b-163">permissionGrantPolicyIdsAssignedToDefaultUserRole</span><span class="sxs-lookup"><span data-stu-id="a038b-163">permissionGrantPolicyIdsAssignedToDefaultUserRole</span></span> | <span data-ttu-id="a038b-164">字符串集合</span><span class="sxs-lookup"><span data-stu-id="a038b-164">String collection</span></span> | <span data-ttu-id="a038b-165">指示是否允许用户同意应用程序，如果是，则使用哪个 [应用程序同意策略](/azure/active-directory/manage-apps/manage-app-consent-policies) 来控制授予许可的用户的权限。</span><span class="sxs-lookup"><span data-stu-id="a038b-165">Indicates whether user consent to apps is allowed, and if it is, which [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) governs the permission for users to grant consent.</span></span> <span data-ttu-id="a038b-166">值的格式应为 `managePermissionGrantsForSelf.{id}` ，其中 `{id}` 是内置或自定义[应用程序许可策略](/azure/active-directory/manage-apps/manage-app-consent-policies)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="a038b-166">Values should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="a038b-167">空列表指示用户同意应用程序已被禁用。</span><span class="sxs-lookup"><span data-stu-id="a038b-167">An empty list indicates user consent to apps is disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="a038b-168">响应</span><span class="sxs-lookup"><span data-stu-id="a038b-168">Response</span></span>

<span data-ttu-id="a038b-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a038b-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a038b-171">示例</span><span class="sxs-lookup"><span data-stu-id="a038b-171">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="a038b-172">示例1：更新或设置租户的来宾用户访问级别</span><span class="sxs-lookup"><span data-stu-id="a038b-172">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="a038b-173">请求</span><span class="sxs-lookup"><span data-stu-id="a038b-173">Request</span></span>

<span data-ttu-id="a038b-174">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a038b-174">The following is an example of the request.</span></span> <span data-ttu-id="a038b-175">在此示例中，将来宾访问级别修改为受限制的来宾用户。</span><span class="sxs-lookup"><span data-stu-id="a038b-175">In this example, guest access level is modified to Restricted Guest User.</span></span>

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

#### <a name="response"></a><span data-ttu-id="a038b-176">响应</span><span class="sxs-lookup"><span data-stu-id="a038b-176">Response</span></span>

<span data-ttu-id="a038b-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a038b-177">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a><span data-ttu-id="a038b-178">示例2：在租户上为预览启用新功能</span><span class="sxs-lookup"><span data-stu-id="a038b-178">Example 2: Enable new feature for preview on tenant</span></span>

#### <a name="request"></a><span data-ttu-id="a038b-179">请求</span><span class="sxs-lookup"><span data-stu-id="a038b-179">Request</span></span>

<span data-ttu-id="a038b-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a038b-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a038b-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="a038b-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a038b-182">C#</span><span class="sxs-lookup"><span data-stu-id="a038b-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-preview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a038b-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a038b-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-preview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a038b-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a038b-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-preview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a038b-185">响应</span><span class="sxs-lookup"><span data-stu-id="a038b-185">Response</span></span>

<span data-ttu-id="a038b-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a038b-186">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-block-msol-powershell-in-tenant"></a><span data-ttu-id="a038b-187">示例3：阻止租户中的 MSOL PowerShell</span><span class="sxs-lookup"><span data-stu-id="a038b-187">Example 3: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="a038b-188">请求</span><span class="sxs-lookup"><span data-stu-id="a038b-188">Request</span></span>

<span data-ttu-id="a038b-189">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a038b-189">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a038b-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="a038b-190">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a038b-191">C#</span><span class="sxs-lookup"><span data-stu-id="a038b-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a038b-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a038b-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a038b-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a038b-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a038b-194">响应</span><span class="sxs-lookup"><span data-stu-id="a038b-194">Response</span></span>

<span data-ttu-id="a038b-195">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a038b-195">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-4-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="a038b-196">示例4：禁用默认用户角色的权限以创建应用程序</span><span class="sxs-lookup"><span data-stu-id="a038b-196">Example 4: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="a038b-197">请求</span><span class="sxs-lookup"><span data-stu-id="a038b-197">Request</span></span>

<span data-ttu-id="a038b-198">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a038b-198">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a038b-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="a038b-199">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a038b-200">C#</span><span class="sxs-lookup"><span data-stu-id="a038b-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a038b-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a038b-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a038b-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a038b-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a038b-203">响应</span><span class="sxs-lookup"><span data-stu-id="a038b-203">Response</span></span>

<span data-ttu-id="a038b-204">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a038b-204">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="a038b-205">示例5：启用默认用户角色以使用 Self-Serve 密码重置功能</span><span class="sxs-lookup"><span data-stu-id="a038b-205">Example 5: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="a038b-206">请求</span><span class="sxs-lookup"><span data-stu-id="a038b-206">Request</span></span>

<span data-ttu-id="a038b-207">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a038b-207">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a038b-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="a038b-208">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a038b-209">C#</span><span class="sxs-lookup"><span data-stu-id="a038b-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a038b-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a038b-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a038b-211">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a038b-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a038b-212">响应</span><span class="sxs-lookup"><span data-stu-id="a038b-212">Response</span></span>

<span data-ttu-id="a038b-213">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a038b-213">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-6-disable-user-consent-to-apps-for-default-user-role"></a><span data-ttu-id="a038b-214">示例6：禁止用户同意默认用户角色的应用程序</span><span class="sxs-lookup"><span data-stu-id="a038b-214">Example 6: Disable user consent to apps for default user role</span></span>

#### <a name="request"></a><span data-ttu-id="a038b-215">请求</span><span class="sxs-lookup"><span data-stu-id="a038b-215">Request</span></span>

<span data-ttu-id="a038b-216">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a038b-216">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_disableUserConsent"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
    "permissionGrantPolicyIdsAssignedToDefaultUserRole": [ ]
}
```

#### <a name="response"></a><span data-ttu-id="a038b-217">响应</span><span class="sxs-lookup"><span data-stu-id="a038b-217">Response</span></span>

<span data-ttu-id="a038b-218">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a038b-218">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-7-enable-user-consent-to-apps-subject-to-app-consent-policy"></a><span data-ttu-id="a038b-219">示例7：允许用户同意应用程序，受应用程序许可策略的制约</span><span class="sxs-lookup"><span data-stu-id="a038b-219">Example 7: Enable user consent to apps, subject to app consent policy</span></span> 

#### <a name="request"></a><span data-ttu-id="a038b-220">请求</span><span class="sxs-lookup"><span data-stu-id="a038b-220">Request</span></span>

<span data-ttu-id="a038b-221">以下是允许用户同意应用程序的请求的示例，具体取决于内置 [应用程序许可策略，该策略](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low` 允许委派权限归为 "低"，适用于来自已验证的发布者或在同一租户中注册的客户端应用程序。</span><span class="sxs-lookup"><span data-stu-id="a038b-221">The following is an example of the request that allows user consent to apps, subject to the built-in [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low`, which allows delegated permissions classified "low", for client apps from verified publishers or registered in the same tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_enableUserConsentLow"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
    "permissionGrantPolicyIdsAssignedToDefaultUserRole": [
        "managePermissionGrantsForSelf.microsoft-user-default-low"
    ]
}
```

#### <a name="response"></a><span data-ttu-id="a038b-222">响应</span><span class="sxs-lookup"><span data-stu-id="a038b-222">Response</span></span>

<span data-ttu-id="a038b-223">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a038b-223">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationpolicy"
} -->

```http
HTTP/1.1 204 No Content
```
