---
title: 更新 authorizationpolicy
description: 更新 authorizationPolicy 对象的属性。
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1e57436cc396b78a8697516702004c7ea4f6d666
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231979"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="d7866-103">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="d7866-103">Update authorizationPolicy</span></span>

<span data-ttu-id="d7866-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7866-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d7866-105">更新 [authorizationPolicy 对象](../resources/authorizationpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="d7866-105">Update the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7866-106">权限</span><span class="sxs-lookup"><span data-stu-id="d7866-106">Permissions</span></span>

<span data-ttu-id="d7866-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7866-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7866-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7866-109">Permission type</span></span>                        | <span data-ttu-id="d7866-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7866-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d7866-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7866-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7866-112">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="d7866-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="d7866-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7866-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7866-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7866-114">Not supported.</span></span> |
| <span data-ttu-id="d7866-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7866-115">Application</span></span>                            | <span data-ttu-id="d7866-116">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="d7866-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7866-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7866-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="d7866-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7866-118">Request headers</span></span>

| <span data-ttu-id="d7866-119">名称</span><span class="sxs-lookup"><span data-stu-id="d7866-119">Name</span></span>       | <span data-ttu-id="d7866-120">说明</span><span class="sxs-lookup"><span data-stu-id="d7866-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d7866-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7866-121">Authorization</span></span> | <span data-ttu-id="d7866-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7866-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7866-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="d7866-124">Content-type</span></span> | <span data-ttu-id="d7866-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d7866-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7866-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7866-127">Request body</span></span>

<span data-ttu-id="d7866-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="d7866-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d7866-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="d7866-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d7866-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d7866-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d7866-131">属性</span><span class="sxs-lookup"><span data-stu-id="d7866-131">Property</span></span>     | <span data-ttu-id="d7866-132">类型</span><span class="sxs-lookup"><span data-stu-id="d7866-132">Type</span></span>        | <span data-ttu-id="d7866-133">说明</span><span class="sxs-lookup"><span data-stu-id="d7866-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d7866-134">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="d7866-134">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="d7866-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7866-135">Boolean</span></span>| <span data-ttu-id="d7866-136">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="d7866-136">Indicates whether users can sign up for email based subscriptions.</span></span> |
|<span data-ttu-id="d7866-137">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="d7866-137">allowedToUseSSPR</span></span>|<span data-ttu-id="d7866-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7866-138">Boolean</span></span>| <span data-ttu-id="d7866-139">指示租户Self-Serve是否可以使用密码重置功能。</span><span class="sxs-lookup"><span data-stu-id="d7866-139">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> |
|<span data-ttu-id="d7866-140">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="d7866-140">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="d7866-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7866-141">Boolean</span></span>| <span data-ttu-id="d7866-142">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="d7866-142">Indicates whether a user can join the tenant by email validation.</span></span> |
|<span data-ttu-id="d7866-143">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="d7866-143">allowInvitesFrom</span></span>|<span data-ttu-id="d7866-144">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="d7866-144">allowInvitesFrom</span></span>|<span data-ttu-id="d7866-145">指示谁可以邀请外部用户加入组织。</span><span class="sxs-lookup"><span data-stu-id="d7866-145">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="d7866-146">可取值为：`none`、`adminsAndGuestInviters`、`adminsGuestInvitersAndAllMembers`、`everyone`。</span><span class="sxs-lookup"><span data-stu-id="d7866-146">Possible values are: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span></span>  <span data-ttu-id="d7866-147">`everyone` 是除美国政府以外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="d7866-147">`everyone` is the default setting for all cloud environments except US Government.</span></span> <span data-ttu-id="d7866-148">有关详细信息，请参阅此表中的允许 [值](../resources/authorizationpolicy.md#allowinvitesfrom-values)。</span><span class="sxs-lookup"><span data-stu-id="d7866-148">See more on the allowed values in this [table](../resources/authorizationpolicy.md#allowinvitesfrom-values).</span></span> |
|<span data-ttu-id="d7866-149">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="d7866-149">blockMsolPowerShell</span></span>|<span data-ttu-id="d7866-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7866-150">Boolean</span></span>| <span data-ttu-id="d7866-151">若要禁止使用 MSOL PowerShell，将此属性设置为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="d7866-151">To disable the use of MSOL PowerShell set this property to `true`.</span></span> <span data-ttu-id="d7866-152">这还将禁止基于用户对 MSOL PowerShell 使用的旧服务终结点的访问。</span><span class="sxs-lookup"><span data-stu-id="d7866-152">This will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="d7866-153">这不会影响 Azure AD 连接 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="d7866-153">This does not affect Azure AD Connect or Microsoft Graph.</span></span> |
|<span data-ttu-id="d7866-154">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="d7866-154">defaultUserRolePermissions</span></span>|[<span data-ttu-id="d7866-155">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="d7866-155">defaultUserRolePermissions</span></span>](../resources/defaultuserrolepermissions.md)| <span data-ttu-id="d7866-156">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="d7866-156">Specifies certain customizable permissions for default user role.</span></span> |
|<span data-ttu-id="d7866-157">说明</span><span class="sxs-lookup"><span data-stu-id="d7866-157">description</span></span>|<span data-ttu-id="d7866-158">String</span><span class="sxs-lookup"><span data-stu-id="d7866-158">String</span></span>| <span data-ttu-id="d7866-159">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="d7866-159">Description of this policy.</span></span>|
|<span data-ttu-id="d7866-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d7866-160">displayName</span></span>|<span data-ttu-id="d7866-161">String</span><span class="sxs-lookup"><span data-stu-id="d7866-161">String</span></span>| <span data-ttu-id="d7866-162">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d7866-162">Display name for this policy.</span></span> |
|<span data-ttu-id="d7866-163">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="d7866-163">guestUserRoleId</span></span>|<span data-ttu-id="d7866-164">Guid</span><span class="sxs-lookup"><span data-stu-id="d7866-164">Guid</span></span>| <span data-ttu-id="d7866-165">表示应授予来宾用户的角色的角色 templateId。</span><span class="sxs-lookup"><span data-stu-id="d7866-165">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="d7866-166">当前支持以下角色：用户角色 () 、来宾用户 `a0b1b346-4d3e-4e8b-98f8-753987be4970` `10dae51f-b6af-4016-8d66-8c2a99b929b3` () 和受限来宾 `2af84b1e-32c8-42b7-82bc-daa82404023b` () 。</span><span class="sxs-lookup"><span data-stu-id="d7866-166">Currently following roles are supported:  User (`a0b1b346-4d3e-4e8b-98f8-753987be4970`), Guest User (`10dae51f-b6af-4016-8d66-8c2a99b929b3`), and Restricted Guest User (`2af84b1e-32c8-42b7-82bc-daa82404023b`).</span></span> |


## <a name="response"></a><span data-ttu-id="d7866-167">响应</span><span class="sxs-lookup"><span data-stu-id="d7866-167">Response</span></span>

<span data-ttu-id="d7866-p108">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d7866-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d7866-170">示例</span><span class="sxs-lookup"><span data-stu-id="d7866-170">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="d7866-171">示例 1：更新或设置租户的来宾用户访问级别</span><span class="sxs-lookup"><span data-stu-id="d7866-171">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="d7866-172">请求</span><span class="sxs-lookup"><span data-stu-id="d7866-172">Request</span></span>

<span data-ttu-id="d7866-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d7866-173">The following is an example of the request.</span></span> <span data-ttu-id="d7866-174">本示例将来宾访问级别修改为"受限来宾用户"。</span><span class="sxs-lookup"><span data-stu-id="d7866-174">In this example, guest access level is modified to Restricted Guest User.</span></span>


# <a name="http"></a>[<span data-ttu-id="d7866-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7866-175">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d7866-176">C#</span><span class="sxs-lookup"><span data-stu-id="d7866-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-guestuserlevel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7866-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7866-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-guestuserlevel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7866-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7866-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-guestuserlevel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7866-179">Java</span><span class="sxs-lookup"><span data-stu-id="d7866-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-guestuserlevel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d7866-180">响应</span><span class="sxs-lookup"><span data-stu-id="d7866-180">Response</span></span>

<span data-ttu-id="d7866-181">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d7866-181">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-block-msol-powershell-in-tenant"></a><span data-ttu-id="d7866-182">示例 2：在租户中阻止 MSOL PowerShell</span><span class="sxs-lookup"><span data-stu-id="d7866-182">Example 2: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="d7866-183">请求</span><span class="sxs-lookup"><span data-stu-id="d7866-183">Request</span></span>

<span data-ttu-id="d7866-184">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d7866-184">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d7866-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7866-185">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d7866-186">C#</span><span class="sxs-lookup"><span data-stu-id="d7866-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7866-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7866-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7866-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7866-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7866-189">Java</span><span class="sxs-lookup"><span data-stu-id="d7866-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-blockmsolpowershell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d7866-190">响应</span><span class="sxs-lookup"><span data-stu-id="d7866-190">Response</span></span>

<span data-ttu-id="d7866-191">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d7866-191">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="d7866-192">示例 3：禁用默认用户角色创建应用程序的权限</span><span class="sxs-lookup"><span data-stu-id="d7866-192">Example 3: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="d7866-193">请求</span><span class="sxs-lookup"><span data-stu-id="d7866-193">Request</span></span>

<span data-ttu-id="d7866-194">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d7866-194">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d7866-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7866-195">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d7866-196">C#</span><span class="sxs-lookup"><span data-stu-id="d7866-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7866-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7866-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7866-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7866-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7866-199">Java</span><span class="sxs-lookup"><span data-stu-id="d7866-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d7866-200">响应</span><span class="sxs-lookup"><span data-stu-id="d7866-200">Response</span></span>

<span data-ttu-id="d7866-201">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d7866-201">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-4-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="d7866-202">示例 4：启用默认用户角色以使用Self-Serve重置功能</span><span class="sxs-lookup"><span data-stu-id="d7866-202">Example 4: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="d7866-203">请求</span><span class="sxs-lookup"><span data-stu-id="d7866-203">Request</span></span>

<span data-ttu-id="d7866-204">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d7866-204">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d7866-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7866-205">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d7866-206">C#</span><span class="sxs-lookup"><span data-stu-id="d7866-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7866-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7866-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7866-208">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7866-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7866-209">Java</span><span class="sxs-lookup"><span data-stu-id="d7866-209">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-sspr-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d7866-210">响应</span><span class="sxs-lookup"><span data-stu-id="d7866-210">Response</span></span>

<span data-ttu-id="d7866-211">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d7866-211">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-disable-user-consent-to-apps-for-default-user-role"></a><span data-ttu-id="d7866-212">示例 5：禁用用户对默认用户角色的应用的同意</span><span class="sxs-lookup"><span data-stu-id="d7866-212">Example 5: Disable user consent to apps for default user role</span></span>

#### <a name="request"></a><span data-ttu-id="d7866-213">请求</span><span class="sxs-lookup"><span data-stu-id="d7866-213">Request</span></span>

<span data-ttu-id="d7866-214">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d7866-214">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d7866-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7866-215">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d7866-216">C#</span><span class="sxs-lookup"><span data-stu-id="d7866-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-disableuserconsent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7866-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7866-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-disableuserconsent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7866-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7866-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-disableuserconsent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7866-219">Java</span><span class="sxs-lookup"><span data-stu-id="d7866-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-disableuserconsent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d7866-220">响应</span><span class="sxs-lookup"><span data-stu-id="d7866-220">Response</span></span>

<span data-ttu-id="d7866-221">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d7866-221">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-6-enable-user-consent-to-apps-subject-to-app-consent-policy"></a><span data-ttu-id="d7866-222">示例 6：根据应用同意策略启用用户对应用的同意</span><span class="sxs-lookup"><span data-stu-id="d7866-222">Example 6: Enable user consent to apps, subject to app consent policy</span></span>

#### <a name="request"></a><span data-ttu-id="d7866-223">请求</span><span class="sxs-lookup"><span data-stu-id="d7866-223">Request</span></span>

<span data-ttu-id="d7866-224">下面是一个请求示例，该请求允许用户同意应用，但需遵循内置的应用许可策略，该[](/azure/active-directory/manage-apps/manage-app-consent-policies)策略允许来自已验证发布者或在同一租户中注册的客户端应用分类为"低"的委派权限。 `microsoft-user-default-low`</span><span class="sxs-lookup"><span data-stu-id="d7866-224">The following is an example of the request that allows user consent to apps, subject to the built-in [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low`, which allows delegated permissions classified "low", for client apps from verified publishers or registered in the same tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="d7866-225">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7866-225">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d7866-226">C#</span><span class="sxs-lookup"><span data-stu-id="d7866-226">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-enableuserconsentlow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7866-227">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7866-227">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-enableuserconsentlow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7866-228">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7866-228">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-enableuserconsentlow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7866-229">Java</span><span class="sxs-lookup"><span data-stu-id="d7866-229">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-enableuserconsentlow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d7866-230">响应</span><span class="sxs-lookup"><span data-stu-id="d7866-230">Response</span></span>

<span data-ttu-id="d7866-231">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d7866-231">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationpolicy"
} -->

```http
HTTP/1.1 204 No Content
```
