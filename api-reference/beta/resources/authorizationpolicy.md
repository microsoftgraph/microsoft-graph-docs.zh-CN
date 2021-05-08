---
title: authorizationPolicy 资源类型
description: 表示可以控制用户授权设置Azure Active Directory。
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cb35f7745a22a4a2eda43c48b3fc870ba1a88cce
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231586"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="07e87-103">authorizationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="07e87-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="07e87-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07e87-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07e87-105">表示可以控制授权Azure Active Directory的策略。</span><span class="sxs-lookup"><span data-stu-id="07e87-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="07e87-106">它是从基本策略类型继承的单一对象，并且始终存在于租户中。</span><span class="sxs-lookup"><span data-stu-id="07e87-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span> 

## <a name="methods"></a><span data-ttu-id="07e87-107">方法</span><span class="sxs-lookup"><span data-stu-id="07e87-107">Methods</span></span>

| <span data-ttu-id="07e87-108">方法</span><span class="sxs-lookup"><span data-stu-id="07e87-108">Method</span></span>       | <span data-ttu-id="07e87-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="07e87-109">Return Type</span></span> | <span data-ttu-id="07e87-110">说明</span><span class="sxs-lookup"><span data-stu-id="07e87-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="07e87-111">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="07e87-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="07e87-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="07e87-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="07e87-113">读取 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="07e87-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="07e87-114">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="07e87-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="07e87-115">无</span><span class="sxs-lookup"><span data-stu-id="07e87-115">None</span></span> | <span data-ttu-id="07e87-116">更新 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="07e87-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="07e87-117">属性</span><span class="sxs-lookup"><span data-stu-id="07e87-117">Properties</span></span>  
| <span data-ttu-id="07e87-118">属性</span><span class="sxs-lookup"><span data-stu-id="07e87-118">Property</span></span> | <span data-ttu-id="07e87-119">类型</span><span class="sxs-lookup"><span data-stu-id="07e87-119">Type</span></span> | <span data-ttu-id="07e87-120">说明</span><span class="sxs-lookup"><span data-stu-id="07e87-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="07e87-121">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="07e87-121">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="07e87-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="07e87-122">Boolean</span></span>| <span data-ttu-id="07e87-123">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="07e87-123">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="07e87-124">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="07e87-124">allowedToUseSSPR</span></span>|<span data-ttu-id="07e87-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="07e87-125">Boolean</span></span>| <span data-ttu-id="07e87-126">指示租户Self-Serve是否可以使用密码重置功能。</span><span class="sxs-lookup"><span data-stu-id="07e87-126">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="07e87-127">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="07e87-127">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="07e87-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="07e87-128">Boolean</span></span>| <span data-ttu-id="07e87-129">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="07e87-129">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="07e87-130">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="07e87-130">allowInvitesFrom</span></span>|<span data-ttu-id="07e87-131">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="07e87-131">allowInvitesFrom</span></span>|<span data-ttu-id="07e87-132">指示谁可以邀请外部用户加入组织。</span><span class="sxs-lookup"><span data-stu-id="07e87-132">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="07e87-133">可取值为：`none`、`adminsAndGuestInviters`、`adminsGuestInvitersAndAllMembers`、`everyone`。</span><span class="sxs-lookup"><span data-stu-id="07e87-133">Possible values are: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span></span>  <span data-ttu-id="07e87-134">`everyone` 是除美国政府以外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="07e87-134">`everyone` is the default setting for all cloud environments except US Government.</span></span> <span data-ttu-id="07e87-135">请参阅下表中的 [，了解](#allowinvitesfrom-values)。</span><span class="sxs-lookup"><span data-stu-id="07e87-135">See more in the [table below](#allowinvitesfrom-values).</span></span>|
|<span data-ttu-id="07e87-136">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="07e87-136">blockMsolPowerShell</span></span>|<span data-ttu-id="07e87-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="07e87-137">Boolean</span></span>| <span data-ttu-id="07e87-138">若要禁止使用 MSOL PowerShell，将此属性设置为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="07e87-138">To disable the use of MSOL PowerShell set this property to `true`.</span></span> <span data-ttu-id="07e87-139">这还将禁止基于用户对 MSOL PowerShell 使用的旧服务终结点的访问。</span><span class="sxs-lookup"><span data-stu-id="07e87-139">This will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="07e87-140">这不会影响 Azure AD 连接 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="07e87-140">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="07e87-141">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="07e87-141">defaultUserRolePermissions</span></span>|[<span data-ttu-id="07e87-142">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="07e87-142">defaultUserRolePermissions</span></span>](defaultUserRolePermissions.md)| <span data-ttu-id="07e87-143">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="07e87-143">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="07e87-144">说明</span><span class="sxs-lookup"><span data-stu-id="07e87-144">description</span></span>|<span data-ttu-id="07e87-145">String</span><span class="sxs-lookup"><span data-stu-id="07e87-145">String</span></span>| <span data-ttu-id="07e87-146">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="07e87-146">Description of this policy.</span></span>|  
|<span data-ttu-id="07e87-147">displayName</span><span class="sxs-lookup"><span data-stu-id="07e87-147">displayName</span></span>|<span data-ttu-id="07e87-148">String</span><span class="sxs-lookup"><span data-stu-id="07e87-148">String</span></span>| <span data-ttu-id="07e87-149">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="07e87-149">Display name for this policy.</span></span> |  
|<span data-ttu-id="07e87-150">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="07e87-150">enabledPreviewFeatures</span></span>|<span data-ttu-id="07e87-151">String collection</span><span class="sxs-lookup"><span data-stu-id="07e87-151">String collection</span></span>| <span data-ttu-id="07e87-152">租户上启用专用预览的功能列表。</span><span class="sxs-lookup"><span data-stu-id="07e87-152">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="07e87-153">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="07e87-153">guestUserRoleId</span></span>|<span data-ttu-id="07e87-154">Guid</span><span class="sxs-lookup"><span data-stu-id="07e87-154">Guid</span></span>| <span data-ttu-id="07e87-155">表示应授予来宾用户的角色的角色 templateId。</span><span class="sxs-lookup"><span data-stu-id="07e87-155">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="07e87-156">请参阅 [列出 unifiedRoleDefinitions](../api/rbacapplication-list-roledefinitions.md) 以查找可用角色模板的列表。</span><span class="sxs-lookup"><span data-stu-id="07e87-156">Refer to [List unifiedRoleDefinitions](../api/rbacapplication-list-roledefinitions.md) to find the list of available role templates.</span></span> <span data-ttu-id="07e87-157">当前支持以下角色：用户角色 () 、来宾用户 `a0b1b346-4d3e-4e8b-98f8-753987be4970` `10dae51f-b6af-4016-8d66-8c2a99b929b3` () 和受限来宾 `2af84b1e-32c8-42b7-82bc-daa82404023b` () 。</span><span class="sxs-lookup"><span data-stu-id="07e87-157">Currently following roles are supported:  User (`a0b1b346-4d3e-4e8b-98f8-753987be4970`), Guest User (`10dae51f-b6af-4016-8d66-8c2a99b929b3`), and Restricted Guest User (`2af84b1e-32c8-42b7-82bc-daa82404023b`).</span></span> | 
|<span data-ttu-id="07e87-158">id</span><span class="sxs-lookup"><span data-stu-id="07e87-158">id</span></span>|<span data-ttu-id="07e87-159">String</span><span class="sxs-lookup"><span data-stu-id="07e87-159">String</span></span>| <span data-ttu-id="07e87-160">授权策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="07e87-160">ID of the authorization policy.</span></span> <span data-ttu-id="07e87-161">必需。</span><span class="sxs-lookup"><span data-stu-id="07e87-161">Required.</span></span> <span data-ttu-id="07e87-162">只读。</span><span class="sxs-lookup"><span data-stu-id="07e87-162">Read-only.</span></span>| 
|<span data-ttu-id="07e87-163">permissionGrantPolicyIdsAssignedToDefaultUserRole</span><span class="sxs-lookup"><span data-stu-id="07e87-163">permissionGrantPolicyIdsAssignedToDefaultUserRole</span></span>|<span data-ttu-id="07e87-164">String collection</span><span class="sxs-lookup"><span data-stu-id="07e87-164">String collection</span></span>|<span data-ttu-id="07e87-165">指示是否允许用户同意应用，如果是，哪个应用许可策略 (permissionGrantPolicy) 管理用户授予同意的权限。</span><span class="sxs-lookup"><span data-stu-id="07e87-165">Indicates if user consent to apps is allowed, and if it is, which app consent policy (permissionGrantPolicy) governs the permission for users to grant consent.</span></span> <span data-ttu-id="07e87-166">值的格式应为 ，其中 是内置或自定义应用同意策略 `managePermissionGrantsForSelf.{id}` `{id}` 的[ID。](/azure/active-directory/manage-apps/manage-app-consent-policies) </span><span class="sxs-lookup"><span data-stu-id="07e87-166">Values should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="07e87-167">空列表表示已禁用用户对应用的同意。</span><span class="sxs-lookup"><span data-stu-id="07e87-167">An empty list indicates user consent to apps is disabled.</span></span> |

### <a name="allowinvitesfrom-values"></a><span data-ttu-id="07e87-168">allowInvitesFrom 值</span><span class="sxs-lookup"><span data-stu-id="07e87-168">allowInvitesFrom values</span></span>

|<span data-ttu-id="07e87-169">成员</span><span class="sxs-lookup"><span data-stu-id="07e87-169">Member</span></span>|<span data-ttu-id="07e87-170">说明</span><span class="sxs-lookup"><span data-stu-id="07e87-170">Description</span></span>|
|:---|:---|
|<span data-ttu-id="07e87-171">无</span><span class="sxs-lookup"><span data-stu-id="07e87-171">none</span></span>|<span data-ttu-id="07e87-172">阻止包括管理员在内的所有人邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="07e87-172">Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="07e87-173">美国政府的默认设置。</span><span class="sxs-lookup"><span data-stu-id="07e87-173">Default setting for US Government.</span></span>|
|<span data-ttu-id="07e87-174">adminsAndGuestInviters</span><span class="sxs-lookup"><span data-stu-id="07e87-174">adminsAndGuestInviters</span></span>|<span data-ttu-id="07e87-175">允许全局管理员、用户管理员和来宾邀请者角色的成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="07e87-175">Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span>|
|<span data-ttu-id="07e87-176">adminsGuestInvitersAndAllMembers</span><span class="sxs-lookup"><span data-stu-id="07e87-176">adminsGuestInvitersAndAllMembers</span></span>|<span data-ttu-id="07e87-177">允许上述管理员角色和所有其他用户角色成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="07e87-177">Allow the above admin roles and all other User role members to invite external users.</span></span>|
|<span data-ttu-id="07e87-178">everyone</span><span class="sxs-lookup"><span data-stu-id="07e87-178">everyone</span></span>|<span data-ttu-id="07e87-179">允许组织中的每个人（包括来宾用户）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="07e87-179">Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="07e87-180">除美国政府以外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="07e87-180">The default setting for all cloud environments except US Government.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07e87-181">关系</span><span class="sxs-lookup"><span data-stu-id="07e87-181">Relationships</span></span>

<span data-ttu-id="07e87-182">无。</span><span class="sxs-lookup"><span data-stu-id="07e87-182">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07e87-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07e87-183">JSON representation</span></span>

<span data-ttu-id="07e87-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07e87-184">The following is a JSON representation of the resource.</span></span>

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
