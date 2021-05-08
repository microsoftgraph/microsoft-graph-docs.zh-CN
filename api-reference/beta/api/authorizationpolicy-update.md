---
title: 更新 authorizationpolicy
description: 更新 authorizationPolicy 对象的属性。
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6b56548645503fc6bc3577fdb38749b7b8a2d210
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231937"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="ff6b3-103">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="ff6b3-103">Update authorizationPolicy</span></span>

<span data-ttu-id="ff6b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff6b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff6b3-105">更新 [authorizationPolicy 对象](../resources/authorizationpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-105">Update the properties of a [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff6b3-106">权限</span><span class="sxs-lookup"><span data-stu-id="ff6b3-106">Permissions</span></span>

<span data-ttu-id="ff6b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff6b3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff6b3-109">Permission type</span></span>                        | <span data-ttu-id="ff6b3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff6b3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ff6b3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff6b3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff6b3-112">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="ff6b3-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="ff6b3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff6b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff6b3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-114">Not supported.</span></span> |
| <span data-ttu-id="ff6b3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff6b3-115">Application</span></span>                            | <span data-ttu-id="ff6b3-116">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="ff6b3-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff6b3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff6b3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="ff6b3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff6b3-118">Request headers</span></span>

| <span data-ttu-id="ff6b3-119">名称</span><span class="sxs-lookup"><span data-stu-id="ff6b3-119">Name</span></span>       | <span data-ttu-id="ff6b3-120">说明</span><span class="sxs-lookup"><span data-stu-id="ff6b3-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ff6b3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff6b3-121">Authorization</span></span> | <span data-ttu-id="ff6b3-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ff6b3-122">Bearer {token}</span></span> |
| <span data-ttu-id="ff6b3-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="ff6b3-123">Content-type</span></span> | <span data-ttu-id="ff6b3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ff6b3-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff6b3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff6b3-125">Request body</span></span>

<span data-ttu-id="ff6b3-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ff6b3-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ff6b3-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ff6b3-129">属性</span><span class="sxs-lookup"><span data-stu-id="ff6b3-129">Property</span></span>     | <span data-ttu-id="ff6b3-130">类型</span><span class="sxs-lookup"><span data-stu-id="ff6b3-130">Type</span></span>        | <span data-ttu-id="ff6b3-131">说明</span><span class="sxs-lookup"><span data-stu-id="ff6b3-131">Description</span></span> |
|:-------------|:------------|:------------|  
|<span data-ttu-id="ff6b3-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ff6b3-132">displayName</span></span>|<span data-ttu-id="ff6b3-133">String</span><span class="sxs-lookup"><span data-stu-id="ff6b3-133">String</span></span>| <span data-ttu-id="ff6b3-134">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-134">Display name for this policy.</span></span> |  
|<span data-ttu-id="ff6b3-135">说明</span><span class="sxs-lookup"><span data-stu-id="ff6b3-135">description</span></span>|<span data-ttu-id="ff6b3-136">String</span><span class="sxs-lookup"><span data-stu-id="ff6b3-136">String</span></span>| <span data-ttu-id="ff6b3-137">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-137">Description of this policy.</span></span> |  
|<span data-ttu-id="ff6b3-138">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="ff6b3-138">guestUserRoleId</span></span>|<span data-ttu-id="ff6b3-139">Guid</span><span class="sxs-lookup"><span data-stu-id="ff6b3-139">Guid</span></span>| <span data-ttu-id="ff6b3-140">表示应授予来宾用户的角色的角色 templateId。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-140">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="ff6b3-141">请参阅 [列出 unifiedRoleDefinitions](./rbacapplication-list-roledefinitions.md) 以查找可用角色模板的列表。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-141">Refer to [List unifiedRoleDefinitions](./rbacapplication-list-roledefinitions.md) to find the list of available role templates.</span></span> <span data-ttu-id="ff6b3-142">目前仅支持用户角色 () 、来宾用户 `a0b1b346-4d3e-4e8b-98f8-753987be4970` `10dae51f-b6af-4016-8d66-8c2a99b929b3` () 和受限来宾用户 `2af84b1e-32c8-42b7-82bc-daa82404023b` () 。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-142">Only supported roles today are User (`a0b1b346-4d3e-4e8b-98f8-753987be4970`), Guest User (`10dae51f-b6af-4016-8d66-8c2a99b929b3`), and Restricted Guest User (`2af84b1e-32c8-42b7-82bc-daa82404023b`).</span></span> | 
|<span data-ttu-id="ff6b3-143">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="ff6b3-143">enabledPreviewFeatures</span></span>|<span data-ttu-id="ff6b3-144">集合 (字符串) </span><span class="sxs-lookup"><span data-stu-id="ff6b3-144">Collection(string)</span></span>| <span data-ttu-id="ff6b3-145">租户上启用专用预览的功能列表。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-145">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="ff6b3-146">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="ff6b3-146">blockMsolPowerShell</span></span>|<span data-ttu-id="ff6b3-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff6b3-147">Boolean</span></span>| <span data-ttu-id="ff6b3-148">若要禁止使用 MSOL PowerShell，将此属性设置为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-148">To disable the use of MSOL PowerShell, set this property to `true`.</span></span> <span data-ttu-id="ff6b3-149">这还将禁止基于用户对 MSOL PowerShell 使用的旧服务终结点的访问。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-149">This will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="ff6b3-150">这不会影响 Azure AD 连接 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-150">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="ff6b3-151">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="ff6b3-151">defaultUserRolePermissions</span></span>|[<span data-ttu-id="ff6b3-152">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="ff6b3-152">defaultUserRolePermissions</span></span>](../resources/defaultUserRolePermissions.md)| <span data-ttu-id="ff6b3-153">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-153">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="ff6b3-154">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="ff6b3-154">allowedToUseSSPR</span></span>|<span data-ttu-id="ff6b3-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff6b3-155">Boolean</span></span>| <span data-ttu-id="ff6b3-156">指示租户Self-Serve是否可以使用密码重置功能。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-156">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="ff6b3-157">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="ff6b3-157">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="ff6b3-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff6b3-158">Boolean</span></span>| <span data-ttu-id="ff6b3-159">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-159">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="ff6b3-160">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="ff6b3-160">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="ff6b3-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff6b3-161">Boolean</span></span>| <span data-ttu-id="ff6b3-162">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-162">Indicates whether a user can join the tenant by email validation.</span></span> |
| <span data-ttu-id="ff6b3-163">permissionGrantPolicyIdsAssignedToDefaultUserRole</span><span class="sxs-lookup"><span data-stu-id="ff6b3-163">permissionGrantPolicyIdsAssignedToDefaultUserRole</span></span> | <span data-ttu-id="ff6b3-164">String collection</span><span class="sxs-lookup"><span data-stu-id="ff6b3-164">String collection</span></span> | <span data-ttu-id="ff6b3-165">指示是否允许用户同意应用，如果是，由哪个应用许可策略管理用户授予[](/azure/active-directory/manage-apps/manage-app-consent-policies)同意的权限。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-165">Indicates whether user consent to apps is allowed, and if it is, which [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) governs the permission for users to grant consent.</span></span> <span data-ttu-id="ff6b3-166">值的格式应为 ，其中 是内置或自定义应用同意策略 `managePermissionGrantsForSelf.{id}` `{id}` 的[ID。](/azure/active-directory/manage-apps/manage-app-consent-policies) </span><span class="sxs-lookup"><span data-stu-id="ff6b3-166">Values should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="ff6b3-167">空列表表示已禁用用户对应用的同意。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-167">An empty list indicates user consent to apps is disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="ff6b3-168">响应</span><span class="sxs-lookup"><span data-stu-id="ff6b3-168">Response</span></span>

<span data-ttu-id="ff6b3-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff6b3-171">示例</span><span class="sxs-lookup"><span data-stu-id="ff6b3-171">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="ff6b3-172">示例 1：更新或设置租户的来宾用户访问级别</span><span class="sxs-lookup"><span data-stu-id="ff6b3-172">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="ff6b3-173">请求</span><span class="sxs-lookup"><span data-stu-id="ff6b3-173">Request</span></span>

<span data-ttu-id="ff6b3-174">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-174">The following is an example of the request.</span></span> <span data-ttu-id="ff6b3-175">本示例将来宾访问级别修改为"受限来宾用户"。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-175">In this example, guest access level is modified to Restricted Guest User.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_guestUserLevel"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "guestUserRole":"2af84b1e-32c8-42b7-82bc-daa82404023b"
}
```

#### <a name="response"></a><span data-ttu-id="ff6b3-176">响应</span><span class="sxs-lookup"><span data-stu-id="ff6b3-176">Response</span></span>

<span data-ttu-id="ff6b3-177">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-177">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a><span data-ttu-id="ff6b3-178">示例 2：在租户上启用预览新功能</span><span class="sxs-lookup"><span data-stu-id="ff6b3-178">Example 2: Enable new feature for preview on tenant</span></span>

#### <a name="request"></a><span data-ttu-id="ff6b3-179">请求</span><span class="sxs-lookup"><span data-stu-id="ff6b3-179">Request</span></span>

<span data-ttu-id="ff6b3-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ff6b3-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff6b3-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_preview"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "enabledPreviewFeatures":[
      "assignGroupsToRoles"
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="ff6b3-182">C#</span><span class="sxs-lookup"><span data-stu-id="ff6b3-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-preview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff6b3-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff6b3-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-preview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff6b3-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff6b3-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-preview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff6b3-185">Java</span><span class="sxs-lookup"><span data-stu-id="ff6b3-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-preview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ff6b3-186">响应</span><span class="sxs-lookup"><span data-stu-id="ff6b3-186">Response</span></span>

<span data-ttu-id="ff6b3-187">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-187">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-block-msol-powershell-in-tenant"></a><span data-ttu-id="ff6b3-188">示例 3：在租户中阻止 MSOL PowerShell</span><span class="sxs-lookup"><span data-stu-id="ff6b3-188">Example 3: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="ff6b3-189">请求</span><span class="sxs-lookup"><span data-stu-id="ff6b3-189">Request</span></span>

<span data-ttu-id="ff6b3-190">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-190">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff6b3-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff6b3-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_blockMSOLPowerShell"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "blockMsolPowerShell":true
}
```
# <a name="c"></a>[<span data-ttu-id="ff6b3-192">C#</span><span class="sxs-lookup"><span data-stu-id="ff6b3-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff6b3-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff6b3-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff6b3-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff6b3-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff6b3-195">Java</span><span class="sxs-lookup"><span data-stu-id="ff6b3-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-blockmsolpowershell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ff6b3-196">响应</span><span class="sxs-lookup"><span data-stu-id="ff6b3-196">Response</span></span>

<span data-ttu-id="ff6b3-197">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-197">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-4-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="ff6b3-198">示例 4：禁用默认用户角色创建应用程序的权限</span><span class="sxs-lookup"><span data-stu-id="ff6b3-198">Example 4: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="ff6b3-199">请求</span><span class="sxs-lookup"><span data-stu-id="ff6b3-199">Request</span></span>

<span data-ttu-id="ff6b3-200">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-200">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ff6b3-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff6b3-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_applications"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "defaultUserRolePermissions":{
      "allowedToCreateApps":false
   }
}
```
# <a name="c"></a>[<span data-ttu-id="ff6b3-202">C#</span><span class="sxs-lookup"><span data-stu-id="ff6b3-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff6b3-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff6b3-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff6b3-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff6b3-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff6b3-205">Java</span><span class="sxs-lookup"><span data-stu-id="ff6b3-205">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ff6b3-206">响应</span><span class="sxs-lookup"><span data-stu-id="ff6b3-206">Response</span></span>

<span data-ttu-id="ff6b3-207">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-207">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="ff6b3-208">示例 5：启用默认用户角色以使用Self-Serve重置功能</span><span class="sxs-lookup"><span data-stu-id="ff6b3-208">Example 5: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="ff6b3-209">请求</span><span class="sxs-lookup"><span data-stu-id="ff6b3-209">Request</span></span>

<span data-ttu-id="ff6b3-210">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-210">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ff6b3-211">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff6b3-211">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_SSPR"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "allowedToUseSSPR":true
}
```
# <a name="c"></a>[<span data-ttu-id="ff6b3-212">C#</span><span class="sxs-lookup"><span data-stu-id="ff6b3-212">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff6b3-213">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff6b3-213">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff6b3-214">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff6b3-214">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff6b3-215">Java</span><span class="sxs-lookup"><span data-stu-id="ff6b3-215">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-sspr-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ff6b3-216">响应</span><span class="sxs-lookup"><span data-stu-id="ff6b3-216">Response</span></span>

<span data-ttu-id="ff6b3-217">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-217">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-6-disable-user-consent-to-apps-for-default-user-role"></a><span data-ttu-id="ff6b3-218">示例 6：针对默认用户角色禁用用户对应用的同意</span><span class="sxs-lookup"><span data-stu-id="ff6b3-218">Example 6: Disable user consent to apps for default user role</span></span>

#### <a name="request"></a><span data-ttu-id="ff6b3-219">请求</span><span class="sxs-lookup"><span data-stu-id="ff6b3-219">Request</span></span>

<span data-ttu-id="ff6b3-220">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-220">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ff6b3-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff6b3-221">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_disableUserConsent"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "permissionGrantPolicyIdsAssignedToDefaultUserRole":[
   
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="ff6b3-222">C#</span><span class="sxs-lookup"><span data-stu-id="ff6b3-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-disableuserconsent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff6b3-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff6b3-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-disableuserconsent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff6b3-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff6b3-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-disableuserconsent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff6b3-225">Java</span><span class="sxs-lookup"><span data-stu-id="ff6b3-225">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-disableuserconsent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ff6b3-226">响应</span><span class="sxs-lookup"><span data-stu-id="ff6b3-226">Response</span></span>

<span data-ttu-id="ff6b3-227">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-227">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-7-enable-user-consent-to-apps-subject-to-app-consent-policy"></a><span data-ttu-id="ff6b3-228">示例 7：根据应用同意策略启用用户对应用的同意</span><span class="sxs-lookup"><span data-stu-id="ff6b3-228">Example 7: Enable user consent to apps, subject to app consent policy</span></span> 

#### <a name="request"></a><span data-ttu-id="ff6b3-229">请求</span><span class="sxs-lookup"><span data-stu-id="ff6b3-229">Request</span></span>

<span data-ttu-id="ff6b3-230">下面是一个请求示例，该请求允许用户同意应用，但需遵循内置的应用许可策略，该[](/azure/active-directory/manage-apps/manage-app-consent-policies)策略允许来自已验证发布者或在同一租户中注册的客户端应用分类为"低"的委派权限。 `microsoft-user-default-low`</span><span class="sxs-lookup"><span data-stu-id="ff6b3-230">The following is an example of the request that allows user consent to apps, subject to the built-in [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low`, which allows delegated permissions classified "low", for client apps from verified publishers or registered in the same tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="ff6b3-231">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff6b3-231">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_enableUserConsentLow"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "permissionGrantPolicyIdsAssignedToDefaultUserRole":[
      "managePermissionGrantsForSelf.microsoft-user-default-low"
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="ff6b3-232">C#</span><span class="sxs-lookup"><span data-stu-id="ff6b3-232">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-enableuserconsentlow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff6b3-233">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff6b3-233">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-enableuserconsentlow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff6b3-234">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff6b3-234">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-enableuserconsentlow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff6b3-235">Java</span><span class="sxs-lookup"><span data-stu-id="ff6b3-235">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-enableuserconsentlow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ff6b3-236">响应</span><span class="sxs-lookup"><span data-stu-id="ff6b3-236">Response</span></span>

<span data-ttu-id="ff6b3-237">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ff6b3-237">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationpolicy"
} -->

```http
HTTP/1.1 204 No Content
```
