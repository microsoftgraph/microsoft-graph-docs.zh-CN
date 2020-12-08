---
title: 更新 authorizationpolicy
description: 更新 authorizationPolicy 对象的属性。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ccd2e5b95059ec4e3a38eadf3f62b25377eabd3
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581194"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="9cb2a-103">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="9cb2a-103">Update authorizationPolicy</span></span>

<span data-ttu-id="9cb2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cb2a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9cb2a-105">更新 [authorizationPolicy](../resources/authorizationpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-105">Update the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cb2a-106">权限</span><span class="sxs-lookup"><span data-stu-id="9cb2a-106">Permissions</span></span>

<span data-ttu-id="9cb2a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9cb2a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cb2a-109">Permission type</span></span>                        | <span data-ttu-id="9cb2a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cb2a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9cb2a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cb2a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cb2a-112">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="9cb2a-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="9cb2a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cb2a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cb2a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-114">Not supported.</span></span> |
| <span data-ttu-id="9cb2a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cb2a-115">Application</span></span>                            | <span data-ttu-id="9cb2a-116">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="9cb2a-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cb2a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cb2a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="9cb2a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cb2a-118">Request headers</span></span>

| <span data-ttu-id="9cb2a-119">名称</span><span class="sxs-lookup"><span data-stu-id="9cb2a-119">Name</span></span>       | <span data-ttu-id="9cb2a-120">说明</span><span class="sxs-lookup"><span data-stu-id="9cb2a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9cb2a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cb2a-121">Authorization</span></span> | <span data-ttu-id="9cb2a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9cb2a-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="9cb2a-124">Content-type</span></span> | <span data-ttu-id="9cb2a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9cb2a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cb2a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cb2a-127">Request body</span></span>

<span data-ttu-id="9cb2a-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9cb2a-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9cb2a-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9cb2a-131">属性</span><span class="sxs-lookup"><span data-stu-id="9cb2a-131">Property</span></span>     | <span data-ttu-id="9cb2a-132">类型</span><span class="sxs-lookup"><span data-stu-id="9cb2a-132">Type</span></span>        | <span data-ttu-id="9cb2a-133">说明</span><span class="sxs-lookup"><span data-stu-id="9cb2a-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9cb2a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="9cb2a-134">displayName</span></span>|<span data-ttu-id="9cb2a-135">String</span><span class="sxs-lookup"><span data-stu-id="9cb2a-135">String</span></span>| <span data-ttu-id="9cb2a-136">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-136">Display name for this policy.</span></span> |
|<span data-ttu-id="9cb2a-137">说明</span><span class="sxs-lookup"><span data-stu-id="9cb2a-137">description</span></span>|<span data-ttu-id="9cb2a-138">String</span><span class="sxs-lookup"><span data-stu-id="9cb2a-138">String</span></span>| <span data-ttu-id="9cb2a-139">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-139">Description of this policy.</span></span>|
|<span data-ttu-id="9cb2a-140">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="9cb2a-140">blockMsolPowerShell</span></span>|<span data-ttu-id="9cb2a-141">布尔值</span><span class="sxs-lookup"><span data-stu-id="9cb2a-141">Boolean</span></span>| <span data-ttu-id="9cb2a-142">若要禁用 MSOL PowerShell 的使用，请将此属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-142">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="9cb2a-143">如果设置为 true，则还将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-143">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="9cb2a-144">这不会影响 Azure AD Connect 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-144">This does not affect Azure AD Connect or Microsoft Graph.</span></span> |
|<span data-ttu-id="9cb2a-145">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="9cb2a-145">defaultUserRolePermissions</span></span>|[<span data-ttu-id="9cb2a-146">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="9cb2a-146">defaultUserRolePermissions</span></span>](../resources/defaultuserrolepermissions.md)| <span data-ttu-id="9cb2a-147">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-147">Specifies certain customizable permissions for default user role.</span></span> |
|<span data-ttu-id="9cb2a-148">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="9cb2a-148">allowedToUseSSPR</span></span>|<span data-ttu-id="9cb2a-149">布尔值</span><span class="sxs-lookup"><span data-stu-id="9cb2a-149">Boolean</span></span>| <span data-ttu-id="9cb2a-150">指示租户上的用户是否可以使用 Self-Serve 密码重置功能。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-150">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> |
|<span data-ttu-id="9cb2a-151">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="9cb2a-151">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="9cb2a-152">布尔值</span><span class="sxs-lookup"><span data-stu-id="9cb2a-152">Boolean</span></span>| <span data-ttu-id="9cb2a-153">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-153">Indicates whether users can sign up for email based subscriptions.</span></span> |
|<span data-ttu-id="9cb2a-154">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="9cb2a-154">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="9cb2a-155">布尔值</span><span class="sxs-lookup"><span data-stu-id="9cb2a-155">Boolean</span></span>| <span data-ttu-id="9cb2a-156">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-156">Indicates whether a user can join the tenant by email validation.</span></span> |
|<span data-ttu-id="9cb2a-157">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="9cb2a-157">allowInvitesFrom</span></span>|<span data-ttu-id="9cb2a-158">String</span><span class="sxs-lookup"><span data-stu-id="9cb2a-158">String</span></span>|<span data-ttu-id="9cb2a-159">指示谁可以邀请外部用户加入组织。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-159">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="9cb2a-160">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="9cb2a-160">Possible values are:</span></span><ul><li><span data-ttu-id="9cb2a-161">`none` -防止用户（包括管理员）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-161">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="9cb2a-162">美国政府版的默认设置。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-162">Default setting for US Government.</span></span></li><li><span data-ttu-id="9cb2a-163">`adminsAndGuestInviters` -允许全局管理员、用户管理员和来宾邀请者角色的成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-163">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="9cb2a-164">`adminsGuestInvitersAndAllMembers` -允许上述管理员角色和所有其他用户角色成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-164">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="9cb2a-165">`everyone` -允许组织中的每个人（包括来宾用户）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-165">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="9cb2a-166">除美国政府之外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-166">Default setting for all cloud environments except US Government.</span></span></li></ul> |

## <a name="response"></a><span data-ttu-id="9cb2a-167">响应</span><span class="sxs-lookup"><span data-stu-id="9cb2a-167">Response</span></span>

<span data-ttu-id="9cb2a-p109">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-p109">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9cb2a-170">示例</span><span class="sxs-lookup"><span data-stu-id="9cb2a-170">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="9cb2a-171">示例1：更新或设置租户的来宾用户访问级别</span><span class="sxs-lookup"><span data-stu-id="9cb2a-171">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="9cb2a-172">请求</span><span class="sxs-lookup"><span data-stu-id="9cb2a-172">Request</span></span>

<span data-ttu-id="9cb2a-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-173">The following is an example of the request.</span></span> <span data-ttu-id="9cb2a-174">在此示例中，将来宾访问级别修改为受限制的来宾用户。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-174">In this example, guest access level is modified to Restricted Guest User.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_guestUserLevel"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
  "allowEmailVerifiedUsersToJoinOrganization":false
}
```

#### <a name="response"></a><span data-ttu-id="9cb2a-175">响应</span><span class="sxs-lookup"><span data-stu-id="9cb2a-175">Response</span></span>

<span data-ttu-id="9cb2a-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-176">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-block-msol-powershell-in-tenant"></a><span data-ttu-id="9cb2a-177">示例2：阻止租户中的 MSOL PowerShell</span><span class="sxs-lookup"><span data-stu-id="9cb2a-177">Example 2: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="9cb2a-178">请求</span><span class="sxs-lookup"><span data-stu-id="9cb2a-178">Request</span></span>

<span data-ttu-id="9cb2a-179">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-179">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_blockMSOLPowerShell"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "blockMsolPowerShell":true
}
```

#### <a name="response"></a><span data-ttu-id="9cb2a-180">响应</span><span class="sxs-lookup"><span data-stu-id="9cb2a-180">Response</span></span>

<span data-ttu-id="9cb2a-181">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-181">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="9cb2a-182">示例3：禁用默认用户角色的权限以创建应用程序</span><span class="sxs-lookup"><span data-stu-id="9cb2a-182">Example 3: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="9cb2a-183">请求</span><span class="sxs-lookup"><span data-stu-id="9cb2a-183">Request</span></span>

<span data-ttu-id="9cb2a-184">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-184">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_applications"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions":{
      "allowedToCreateApps":false
   }
}
```

#### <a name="response"></a><span data-ttu-id="9cb2a-185">响应</span><span class="sxs-lookup"><span data-stu-id="9cb2a-185">Response</span></span>

<span data-ttu-id="9cb2a-186">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-186">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-4-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="9cb2a-187">示例4：启用默认用户角色以使用 Self-Serve 密码重置功能</span><span class="sxs-lookup"><span data-stu-id="9cb2a-187">Example 4: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="9cb2a-188">请求</span><span class="sxs-lookup"><span data-stu-id="9cb2a-188">Request</span></span>

<span data-ttu-id="9cb2a-189">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-189">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_SSPR"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "allowedToUseSSPR":true
}
```

#### <a name="response"></a><span data-ttu-id="9cb2a-190">响应</span><span class="sxs-lookup"><span data-stu-id="9cb2a-190">Response</span></span>

<span data-ttu-id="9cb2a-191">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-191">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-disable-user-consent-to-apps-for-default-user-role"></a><span data-ttu-id="9cb2a-192">示例5：禁止用户同意默认用户角色的应用程序</span><span class="sxs-lookup"><span data-stu-id="9cb2a-192">Example 5: Disable user consent to apps for default user role</span></span>

#### <a name="request"></a><span data-ttu-id="9cb2a-193">请求</span><span class="sxs-lookup"><span data-stu-id="9cb2a-193">Request</span></span>

<span data-ttu-id="9cb2a-194">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-194">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_disableUserConsent"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions": {
      "permissionGrantPoliciesAssigned": []
   }
}
```

#### <a name="response"></a><span data-ttu-id="9cb2a-195">响应</span><span class="sxs-lookup"><span data-stu-id="9cb2a-195">Response</span></span>

<span data-ttu-id="9cb2a-196">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-196">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-6-enable-user-consent-to-apps-subject-to-app-consent-policy"></a><span data-ttu-id="9cb2a-197">示例6：允许用户同意应用程序，但受应用程序许可策略的制约</span><span class="sxs-lookup"><span data-stu-id="9cb2a-197">Example 6: Enable user consent to apps, subject to app consent policy</span></span>

#### <a name="request"></a><span data-ttu-id="9cb2a-198">请求</span><span class="sxs-lookup"><span data-stu-id="9cb2a-198">Request</span></span>

<span data-ttu-id="9cb2a-199">以下是允许用户同意应用程序的请求的示例，具体取决于内置 [应用程序许可策略，该策略](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low` 允许委派权限归为 "低"，适用于来自已验证的发布者或在同一租户中注册的客户端应用程序。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-199">The following is an example of the request that allows user consent to apps, subject to the built-in [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low`, which allows delegated permissions classified "low", for client apps from verified publishers or registered in the same tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_enableUserConsentLow"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions": {
      "permissionGrantPoliciesAssigned": [
         "managePermissionGrantsForSelf.microsoft-user-default-low"
      ]
   }
}
```

#### <a name="response"></a><span data-ttu-id="9cb2a-200">响应</span><span class="sxs-lookup"><span data-stu-id="9cb2a-200">Response</span></span>

<span data-ttu-id="9cb2a-201">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9cb2a-201">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationpolicy"
} -->

```http
HTTP/1.1 204 No Content
```
