---
title: authorizationPolicy 资源类型
description: 表示可控制 Azure Active Directory 的授权设置的策略。
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e9ad1a67a2aae2c1af4ffa45dcd85228a4c95f25
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433171"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="90406-103">authorizationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="90406-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="90406-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90406-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90406-105">表示可控制 Azure Active Directory 授权设置的策略。</span><span class="sxs-lookup"><span data-stu-id="90406-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="90406-106">它是从基本策略类型继承的单一对象，并且始终存在于租户中。</span><span class="sxs-lookup"><span data-stu-id="90406-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span> 

## <a name="methods"></a><span data-ttu-id="90406-107">Methods</span><span class="sxs-lookup"><span data-stu-id="90406-107">Methods</span></span>

| <span data-ttu-id="90406-108">方法</span><span class="sxs-lookup"><span data-stu-id="90406-108">Method</span></span>       | <span data-ttu-id="90406-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="90406-109">Return Type</span></span> | <span data-ttu-id="90406-110">说明</span><span class="sxs-lookup"><span data-stu-id="90406-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="90406-111">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="90406-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="90406-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="90406-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="90406-113">读取 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="90406-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="90406-114">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="90406-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="90406-115">无</span><span class="sxs-lookup"><span data-stu-id="90406-115">None</span></span> | <span data-ttu-id="90406-116">更新 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="90406-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="90406-117">属性</span><span class="sxs-lookup"><span data-stu-id="90406-117">Properties</span></span>  
| <span data-ttu-id="90406-118">属性</span><span class="sxs-lookup"><span data-stu-id="90406-118">Property</span></span> | <span data-ttu-id="90406-119">类型</span><span class="sxs-lookup"><span data-stu-id="90406-119">Type</span></span> | <span data-ttu-id="90406-120">说明</span><span class="sxs-lookup"><span data-stu-id="90406-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="90406-121">id</span><span class="sxs-lookup"><span data-stu-id="90406-121">id</span></span>|<span data-ttu-id="90406-122">String</span><span class="sxs-lookup"><span data-stu-id="90406-122">String</span></span>| <span data-ttu-id="90406-123">授权策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="90406-123">ID of the authorization policy.</span></span> <span data-ttu-id="90406-124">必需。</span><span class="sxs-lookup"><span data-stu-id="90406-124">Required.</span></span> <span data-ttu-id="90406-125">只读。</span><span class="sxs-lookup"><span data-stu-id="90406-125">Read-only.</span></span>| 
|<span data-ttu-id="90406-126">displayName</span><span class="sxs-lookup"><span data-stu-id="90406-126">displayName</span></span>|<span data-ttu-id="90406-127">String</span><span class="sxs-lookup"><span data-stu-id="90406-127">String</span></span>| <span data-ttu-id="90406-128">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="90406-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="90406-129">说明</span><span class="sxs-lookup"><span data-stu-id="90406-129">description</span></span>|<span data-ttu-id="90406-130">String</span><span class="sxs-lookup"><span data-stu-id="90406-130">String</span></span>| <span data-ttu-id="90406-131">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="90406-131">Description of this policy.</span></span>|  
|<span data-ttu-id="90406-132">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="90406-132">guestUserRoleId</span></span>|<span data-ttu-id="90406-133">Guid</span><span class="sxs-lookup"><span data-stu-id="90406-133">Guid</span></span>| <span data-ttu-id="90406-134">表示应授予来宾用户的角色的角色 templateId。</span><span class="sxs-lookup"><span data-stu-id="90406-134">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="90406-135">请参阅 [List unifiedRoleDefinitions](../api/rbacapplication-list-roledefinitions.md) 查找可用角色模板的列表。</span><span class="sxs-lookup"><span data-stu-id="90406-135">Refer to [List unifiedRoleDefinitions](../api/rbacapplication-list-roledefinitions.md) to find the list of available role templates.</span></span> <span data-ttu-id="90406-136">当前支持以下角色：用户 (a0b1b346-4d3e-4e8b-98f8-753987be4970) ， 来宾用户 (10dae51f-b6af-4016-8d66-8c2a99b929b3) 和受限来宾用户 (2af84b1e-32c8-42b7-82bc-daa82404023b) 。</span><span class="sxs-lookup"><span data-stu-id="90406-136">Currently following roles are supported: User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="90406-137">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="90406-137">enabledPreviewFeatures</span></span>|<span data-ttu-id="90406-138">字符串集合</span><span class="sxs-lookup"><span data-stu-id="90406-138">String collection</span></span>| <span data-ttu-id="90406-139">为租户上的专用预览启用的功能列表。</span><span class="sxs-lookup"><span data-stu-id="90406-139">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="90406-140">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="90406-140">blockMsolPowerShell</span></span>|<span data-ttu-id="90406-141">布尔</span><span class="sxs-lookup"><span data-stu-id="90406-141">Boolean</span></span>| <span data-ttu-id="90406-142">若要禁止使用 MSOL PowerShell，请设置此属性为 true。</span><span class="sxs-lookup"><span data-stu-id="90406-142">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="90406-143">设置为 true 还将禁用对 MSOL PowerShell 使用的旧服务终结点的基于用户的访问。</span><span class="sxs-lookup"><span data-stu-id="90406-143">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="90406-144">这不会影响 Azure AD Connect 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="90406-144">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="90406-145">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="90406-145">defaultUserRolePermissions</span></span>|[<span data-ttu-id="90406-146">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="90406-146">defaultUserRolePermissions</span></span>](defaultUserRolePermissions.md)| <span data-ttu-id="90406-147">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="90406-147">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="90406-148">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="90406-148">allowedToUseSSPR</span></span>|<span data-ttu-id="90406-149">布尔</span><span class="sxs-lookup"><span data-stu-id="90406-149">Boolean</span></span>| <span data-ttu-id="90406-150">指示租户Self-Serve密码重置功能是否可以使用。</span><span class="sxs-lookup"><span data-stu-id="90406-150">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="90406-151">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="90406-151">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="90406-152">布尔</span><span class="sxs-lookup"><span data-stu-id="90406-152">Boolean</span></span>| <span data-ttu-id="90406-153">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="90406-153">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="90406-154">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="90406-154">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="90406-155">布尔</span><span class="sxs-lookup"><span data-stu-id="90406-155">Boolean</span></span>| <span data-ttu-id="90406-156">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="90406-156">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="90406-157">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="90406-157">allowInvitesFrom</span></span>|<span data-ttu-id="90406-158">String</span><span class="sxs-lookup"><span data-stu-id="90406-158">String</span></span>|<span data-ttu-id="90406-159">指示可以邀请外部用户加入组织的用户。</span><span class="sxs-lookup"><span data-stu-id="90406-159">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="90406-160">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="90406-160">Possible values are:</span></span><ul><li><span data-ttu-id="90406-161">`none` - 阻止包括管理员在内的所有人邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="90406-161">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="90406-162">美国政府的默认设置。</span><span class="sxs-lookup"><span data-stu-id="90406-162">Default setting for US Government.</span></span></li><li><span data-ttu-id="90406-163">`adminsAndGuestInviters` - 允许全局管理员、用户管理员和来宾邀请者角色的成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="90406-163">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="90406-164">`adminsGuestInvitersAndAllMembers` - 允许上述管理员角色和所有其他用户角色成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="90406-164">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="90406-165">`everyone` - 允许组织中的每个人（包括来宾用户）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="90406-165">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="90406-166">除美国政府以外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="90406-166">Default setting for all cloud environments except US Government.</span></span></li></ul> |
|<span data-ttu-id="90406-167">permissionGrantPolicyIdsAssignedToDefaultUserRole</span><span class="sxs-lookup"><span data-stu-id="90406-167">permissionGrantPolicyIdsAssignedToDefaultUserRole</span></span>|<span data-ttu-id="90406-168">字符串集合</span><span class="sxs-lookup"><span data-stu-id="90406-168">String collection</span></span>|<span data-ttu-id="90406-169">指示是否允许用户同意应用，如果是，则哪个应用同意策略 (permissionGrantPolicy) 管理用户授予同意的权限。</span><span class="sxs-lookup"><span data-stu-id="90406-169">Indicates if user consent to apps is allowed, and if it is, which app consent policy (permissionGrantPolicy) governs the permission for users to grant consent.</span></span> <span data-ttu-id="90406-170">值的格式应为，其中是内置或自定义应用同意策略 `managePermissionGrantsForSelf.{id}` `{id}` 的[ID。](/azure/active-directory/manage-apps/manage-app-consent-policies) </span><span class="sxs-lookup"><span data-stu-id="90406-170">Values should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="90406-171">空列表表示已禁用用户对应用的同意。</span><span class="sxs-lookup"><span data-stu-id="90406-171">An empty list indicates user consent to apps is disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="90406-172">关系</span><span class="sxs-lookup"><span data-stu-id="90406-172">Relationships</span></span>

<span data-ttu-id="90406-173">无。</span><span class="sxs-lookup"><span data-stu-id="90406-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="90406-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90406-174">JSON representation</span></span>

<span data-ttu-id="90406-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90406-175">The following is a JSON representation of the resource.</span></span>

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
