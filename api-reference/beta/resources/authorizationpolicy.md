---
title: authorizationPolicy 资源类型
description: 表示可以控制 Azure Active Directory 的授权设置的策略。
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3b52ba6c458a69a63135b00a9b53a717eef77091
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962100"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="e7428-103">authorizationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7428-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="e7428-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7428-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7428-105">表示可以控制 Azure Active Directory 授权设置的策略。</span><span class="sxs-lookup"><span data-stu-id="e7428-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="e7428-106">它是从基本策略类型继承的单一对象，并且始终存在于租户中。</span><span class="sxs-lookup"><span data-stu-id="e7428-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span> 

## <a name="methods"></a><span data-ttu-id="e7428-107">Methods</span><span class="sxs-lookup"><span data-stu-id="e7428-107">Methods</span></span>

| <span data-ttu-id="e7428-108">方法</span><span class="sxs-lookup"><span data-stu-id="e7428-108">Method</span></span>       | <span data-ttu-id="e7428-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e7428-109">Return Type</span></span> | <span data-ttu-id="e7428-110">说明</span><span class="sxs-lookup"><span data-stu-id="e7428-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e7428-111">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="e7428-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="e7428-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="e7428-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="e7428-113">读取 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="e7428-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="e7428-114">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="e7428-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="e7428-115">无</span><span class="sxs-lookup"><span data-stu-id="e7428-115">None</span></span> | <span data-ttu-id="e7428-116">更新 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="e7428-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e7428-117">属性</span><span class="sxs-lookup"><span data-stu-id="e7428-117">Properties</span></span>  
| <span data-ttu-id="e7428-118">属性</span><span class="sxs-lookup"><span data-stu-id="e7428-118">Property</span></span> | <span data-ttu-id="e7428-119">类型</span><span class="sxs-lookup"><span data-stu-id="e7428-119">Type</span></span> | <span data-ttu-id="e7428-120">说明</span><span class="sxs-lookup"><span data-stu-id="e7428-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="e7428-121">id</span><span class="sxs-lookup"><span data-stu-id="e7428-121">id</span></span>|<span data-ttu-id="e7428-122">String</span><span class="sxs-lookup"><span data-stu-id="e7428-122">String</span></span>| <span data-ttu-id="e7428-123">授权策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="e7428-123">ID of the authorization policy.</span></span> <span data-ttu-id="e7428-124">必填。</span><span class="sxs-lookup"><span data-stu-id="e7428-124">Required.</span></span> <span data-ttu-id="e7428-125">只读。</span><span class="sxs-lookup"><span data-stu-id="e7428-125">Read-only.</span></span>| 
|<span data-ttu-id="e7428-126">displayName</span><span class="sxs-lookup"><span data-stu-id="e7428-126">displayName</span></span>|<span data-ttu-id="e7428-127">String</span><span class="sxs-lookup"><span data-stu-id="e7428-127">String</span></span>| <span data-ttu-id="e7428-128">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e7428-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="e7428-129">说明</span><span class="sxs-lookup"><span data-stu-id="e7428-129">description</span></span>|<span data-ttu-id="e7428-130">String</span><span class="sxs-lookup"><span data-stu-id="e7428-130">String</span></span>| <span data-ttu-id="e7428-131">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="e7428-131">Description of this policy.</span></span>|  
|<span data-ttu-id="e7428-132">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="e7428-132">guestUserRoleId</span></span>|<span data-ttu-id="e7428-133">Guid</span><span class="sxs-lookup"><span data-stu-id="e7428-133">Guid</span></span>| <span data-ttu-id="e7428-134">表示应授予来宾用户的角色的角色 templateId。</span><span class="sxs-lookup"><span data-stu-id="e7428-134">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="e7428-135">请参阅 [列出 unifiedRoleDefinitions](../api/rbacapplication-list-roledefinitions.md) 以查找可用角色模板的列表。</span><span class="sxs-lookup"><span data-stu-id="e7428-135">Refer to [List unifiedRoleDefinitions](../api/rbacapplication-list-roledefinitions.md) to find the list of available role templates.</span></span> <span data-ttu-id="e7428-136">当前支持以下角色：用户角色 () 、来宾用户 `a0b1b346-4d3e-4e8b-98f8-753987be4970` `10dae51f-b6af-4016-8d66-8c2a99b929b3` () 和受限来宾 `2af84b1e-32c8-42b7-82bc-daa82404023b` () 。</span><span class="sxs-lookup"><span data-stu-id="e7428-136">Currently following roles are supported:  User (`a0b1b346-4d3e-4e8b-98f8-753987be4970`), Guest User (`10dae51f-b6af-4016-8d66-8c2a99b929b3`), and Restricted Guest User (`2af84b1e-32c8-42b7-82bc-daa82404023b`).</span></span> | 
|<span data-ttu-id="e7428-137">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="e7428-137">enabledPreviewFeatures</span></span>|<span data-ttu-id="e7428-138">String collection</span><span class="sxs-lookup"><span data-stu-id="e7428-138">String collection</span></span>| <span data-ttu-id="e7428-139">租户上启用专用预览的功能列表。</span><span class="sxs-lookup"><span data-stu-id="e7428-139">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="e7428-140">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="e7428-140">blockMsolPowerShell</span></span>|<span data-ttu-id="e7428-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7428-141">Boolean</span></span>| <span data-ttu-id="e7428-142">若要禁止使用 MSOL PowerShell，请设置此属性为 true。</span><span class="sxs-lookup"><span data-stu-id="e7428-142">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="e7428-143">设置为 true 还将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。</span><span class="sxs-lookup"><span data-stu-id="e7428-143">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="e7428-144">这不会影响 Azure AD Connect 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="e7428-144">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="e7428-145">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="e7428-145">defaultUserRolePermissions</span></span>|[<span data-ttu-id="e7428-146">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="e7428-146">defaultUserRolePermissions</span></span>](defaultUserRolePermissions.md)| <span data-ttu-id="e7428-147">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="e7428-147">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="e7428-148">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="e7428-148">allowedToUseSSPR</span></span>|<span data-ttu-id="e7428-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7428-149">Boolean</span></span>| <span data-ttu-id="e7428-150">指示租户Self-Serve是否可以使用密码重置功能。</span><span class="sxs-lookup"><span data-stu-id="e7428-150">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="e7428-151">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="e7428-151">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="e7428-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7428-152">Boolean</span></span>| <span data-ttu-id="e7428-153">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="e7428-153">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="e7428-154">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="e7428-154">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="e7428-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7428-155">Boolean</span></span>| <span data-ttu-id="e7428-156">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="e7428-156">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="e7428-157">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="e7428-157">allowInvitesFrom</span></span>|<span data-ttu-id="e7428-158">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="e7428-158">allowInvitesFrom</span></span>|<span data-ttu-id="e7428-159">指示谁可以邀请外部用户加入组织。</span><span class="sxs-lookup"><span data-stu-id="e7428-159">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="e7428-160">可取值为：`none`、`adminsAndGuestInviters`、`adminsGuestInvitersAndAllMembers`、`everyone`。</span><span class="sxs-lookup"><span data-stu-id="e7428-160">Possible values are: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span></span>  <span data-ttu-id="e7428-161">`everyone` 是除美国政府以外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="e7428-161">`everyone` is the default setting for all cloud environments except US Government.</span></span> <span data-ttu-id="e7428-162">请参阅下表 [中的更多内容](#allowinvitesfrom-values)。</span><span class="sxs-lookup"><span data-stu-id="e7428-162">See more in the [table below](#allowinvitesfrom-values).</span></span>|
|<span data-ttu-id="e7428-163">permissionGrantPolicyIdsAssignedToDefaultUserRole</span><span class="sxs-lookup"><span data-stu-id="e7428-163">permissionGrantPolicyIdsAssignedToDefaultUserRole</span></span>|<span data-ttu-id="e7428-164">String collection</span><span class="sxs-lookup"><span data-stu-id="e7428-164">String collection</span></span>|<span data-ttu-id="e7428-165">指示是否允许用户同意应用，如果是，哪个应用许可策略 (permissionGrantPolicy) 管理用户授予同意的权限。</span><span class="sxs-lookup"><span data-stu-id="e7428-165">Indicates if user consent to apps is allowed, and if it is, which app consent policy (permissionGrantPolicy) governs the permission for users to grant consent.</span></span> <span data-ttu-id="e7428-166">值的格式应为 ，其中 是内置或自定义应用同意策略 `managePermissionGrantsForSelf.{id}` `{id}` 的[ID。](/azure/active-directory/manage-apps/manage-app-consent-policies) </span><span class="sxs-lookup"><span data-stu-id="e7428-166">Values should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="e7428-167">空列表表示已禁用用户对应用的同意。</span><span class="sxs-lookup"><span data-stu-id="e7428-167">An empty list indicates user consent to apps is disabled.</span></span> |

### <a name="allowinvitesfrom-values"></a><span data-ttu-id="e7428-168">allowInvitesFrom 值</span><span class="sxs-lookup"><span data-stu-id="e7428-168">allowInvitesFrom values</span></span>

|<span data-ttu-id="e7428-169">成员</span><span class="sxs-lookup"><span data-stu-id="e7428-169">Member</span></span>|<span data-ttu-id="e7428-170">说明</span><span class="sxs-lookup"><span data-stu-id="e7428-170">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e7428-171">无</span><span class="sxs-lookup"><span data-stu-id="e7428-171">none</span></span>|<span data-ttu-id="e7428-172">阻止包括管理员在内的所有人邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="e7428-172">Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="e7428-173">美国政府的默认设置。</span><span class="sxs-lookup"><span data-stu-id="e7428-173">Default setting for US Government.</span></span>|
|<span data-ttu-id="e7428-174">adminsAndGuestInviters</span><span class="sxs-lookup"><span data-stu-id="e7428-174">adminsAndGuestInviters</span></span>|<span data-ttu-id="e7428-175">允许全局管理员、用户管理员和来宾邀请者角色的成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="e7428-175">Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span>|
|<span data-ttu-id="e7428-176">adminsGuestInvitersAndAllMembers</span><span class="sxs-lookup"><span data-stu-id="e7428-176">adminsGuestInvitersAndAllMembers</span></span>|<span data-ttu-id="e7428-177">允许上述管理员角色和所有其他用户角色成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="e7428-177">Allow the above admin roles and all other User role members to invite external users.</span></span>|
|<span data-ttu-id="e7428-178">everyone</span><span class="sxs-lookup"><span data-stu-id="e7428-178">everyone</span></span>|<span data-ttu-id="e7428-179">允许组织中的每个人（包括来宾用户）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="e7428-179">Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="e7428-180">除美国政府以外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="e7428-180">The default setting for all cloud environments except US Government.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7428-181">关系</span><span class="sxs-lookup"><span data-stu-id="e7428-181">Relationships</span></span>

<span data-ttu-id="e7428-182">无。</span><span class="sxs-lookup"><span data-stu-id="e7428-182">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7428-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7428-183">JSON representation</span></span>

<span data-ttu-id="e7428-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7428-184">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authorizationPolicy",
  "keyProperty": "id"
}-->

```json
{
   "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "enabledPreviewFeatures": "[String]",
  "guestUserRoleId": "Guid",
  "blockMsolPowerShell": true,
  "defaultUserRolePermissions": {"@odata.type": "microsoft.graph.defaultUserRolePermissions"},
  "allowedToUseSSPR": true,
  "allowedToSignUpEmailBasedSubscriptions": true,
  "allowEmailVerifiedUsersToJoinOrganization": true,
  "allowInvitesFrom": "String",
  "permissionGrantPolicyIdsAssignedToDefaultUserRole": "[String]"
}
```
