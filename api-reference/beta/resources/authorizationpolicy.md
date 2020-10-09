---
title: authorizationPolicy 资源类型
description: 表示可控制 Azure Active Directory 的授权设置的策略。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1b12c026c38d5292de707b3a324746b77f38fe8f
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402623"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="beb65-103">authorizationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="beb65-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="beb65-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beb65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="beb65-105">表示可控制 Azure Active Directory 授权设置的策略。</span><span class="sxs-lookup"><span data-stu-id="beb65-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="beb65-106">它是从基本策略类型继承的单一实例，并且对于租户始终存在。</span><span class="sxs-lookup"><span data-stu-id="beb65-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span> 

## <a name="methods"></a><span data-ttu-id="beb65-107">方法</span><span class="sxs-lookup"><span data-stu-id="beb65-107">Methods</span></span>

| <span data-ttu-id="beb65-108">方法</span><span class="sxs-lookup"><span data-stu-id="beb65-108">Method</span></span>       | <span data-ttu-id="beb65-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="beb65-109">Return Type</span></span> | <span data-ttu-id="beb65-110">说明</span><span class="sxs-lookup"><span data-stu-id="beb65-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="beb65-111">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="beb65-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="beb65-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="beb65-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="beb65-113">读取 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="beb65-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="beb65-114">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="beb65-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="beb65-115">无</span><span class="sxs-lookup"><span data-stu-id="beb65-115">None</span></span> | <span data-ttu-id="beb65-116">更新 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="beb65-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="beb65-117">属性</span><span class="sxs-lookup"><span data-stu-id="beb65-117">Properties</span></span>  
| <span data-ttu-id="beb65-118">属性</span><span class="sxs-lookup"><span data-stu-id="beb65-118">Property</span></span> | <span data-ttu-id="beb65-119">类型</span><span class="sxs-lookup"><span data-stu-id="beb65-119">Type</span></span> | <span data-ttu-id="beb65-120">说明</span><span class="sxs-lookup"><span data-stu-id="beb65-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="beb65-121">id</span><span class="sxs-lookup"><span data-stu-id="beb65-121">id</span></span>|<span data-ttu-id="beb65-122">字符串</span><span class="sxs-lookup"><span data-stu-id="beb65-122">String</span></span>| <span data-ttu-id="beb65-123">授权策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="beb65-123">ID of the authorization policy.</span></span> <span data-ttu-id="beb65-124">必需。</span><span class="sxs-lookup"><span data-stu-id="beb65-124">Required.</span></span> <span data-ttu-id="beb65-125">只读。</span><span class="sxs-lookup"><span data-stu-id="beb65-125">Read-only.</span></span>| 
|<span data-ttu-id="beb65-126">displayName</span><span class="sxs-lookup"><span data-stu-id="beb65-126">displayName</span></span>|<span data-ttu-id="beb65-127">字符串</span><span class="sxs-lookup"><span data-stu-id="beb65-127">String</span></span>| <span data-ttu-id="beb65-128">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="beb65-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="beb65-129">说明</span><span class="sxs-lookup"><span data-stu-id="beb65-129">description</span></span>|<span data-ttu-id="beb65-130">字符串</span><span class="sxs-lookup"><span data-stu-id="beb65-130">String</span></span>| <span data-ttu-id="beb65-131">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="beb65-131">Description of this policy.</span></span>|  
|<span data-ttu-id="beb65-132">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="beb65-132">guestUserRoleId</span></span>|<span data-ttu-id="beb65-133">Guid</span><span class="sxs-lookup"><span data-stu-id="beb65-133">Guid</span></span>| <span data-ttu-id="beb65-134">表示应向来宾用户授予的角色的角色 templateId。</span><span class="sxs-lookup"><span data-stu-id="beb65-134">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="beb65-135">若要查找可用角色模板的列表，请参阅 [List unifiedRoleDefinitions](../api/rbacapplication-list-roledefinitions.md) 。</span><span class="sxs-lookup"><span data-stu-id="beb65-135">Refer to [List unifiedRoleDefinitions](../api/rbacapplication-list-roledefinitions.md) to find the list of available role templates.</span></span> <span data-ttu-id="beb65-136">当前以下角色受支持： User (a0b1b346-4d3e-4e8b-98f8-753987be4970) 、Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3) 和受限制的来宾用户 (2af84b1e-32c8-42b7-82bc-daa82404023b) 。</span><span class="sxs-lookup"><span data-stu-id="beb65-136">Currently following roles are supported: User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="beb65-137">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="beb65-137">enabledPreviewFeatures</span></span>|<span data-ttu-id="beb65-138">字符串集合</span><span class="sxs-lookup"><span data-stu-id="beb65-138">String collection</span></span>| <span data-ttu-id="beb65-139">租户上启用了专用预览的功能列表。</span><span class="sxs-lookup"><span data-stu-id="beb65-139">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="beb65-140">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="beb65-140">blockMsolPowerShell</span></span>|<span data-ttu-id="beb65-141">布尔</span><span class="sxs-lookup"><span data-stu-id="beb65-141">Boolean</span></span>| <span data-ttu-id="beb65-142">若要禁用 MSOL PowerShell 的使用，请将此属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="beb65-142">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="beb65-143">如果设置为 true，则还将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。</span><span class="sxs-lookup"><span data-stu-id="beb65-143">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="beb65-144">这不会影响 Azure AD Connect 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="beb65-144">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="beb65-145">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="beb65-145">defaultUserRolePermissions</span></span>|[<span data-ttu-id="beb65-146">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="beb65-146">defaultUserRolePermissions</span></span>](defaultUserRolePermissions.md)| <span data-ttu-id="beb65-147">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="beb65-147">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="beb65-148">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="beb65-148">allowedToUseSSPR</span></span>|<span data-ttu-id="beb65-149">布尔</span><span class="sxs-lookup"><span data-stu-id="beb65-149">Boolean</span></span>| <span data-ttu-id="beb65-150">指示租户上的用户是否可以使用 Self-Serve 密码重置功能。</span><span class="sxs-lookup"><span data-stu-id="beb65-150">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="beb65-151">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="beb65-151">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="beb65-152">布尔</span><span class="sxs-lookup"><span data-stu-id="beb65-152">Boolean</span></span>| <span data-ttu-id="beb65-153">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="beb65-153">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="beb65-154">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="beb65-154">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="beb65-155">布尔</span><span class="sxs-lookup"><span data-stu-id="beb65-155">Boolean</span></span>| <span data-ttu-id="beb65-156">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="beb65-156">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="beb65-157">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="beb65-157">allowInvitesFrom</span></span>|<span data-ttu-id="beb65-158">字符串</span><span class="sxs-lookup"><span data-stu-id="beb65-158">String</span></span>|<span data-ttu-id="beb65-159">指示谁可以邀请外部用户加入组织。</span><span class="sxs-lookup"><span data-stu-id="beb65-159">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="beb65-160">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="beb65-160">Possible values are:</span></span><ul><li><span data-ttu-id="beb65-161">`none` -防止用户（包括管理员）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="beb65-161">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="beb65-162">美国政府版的默认设置。</span><span class="sxs-lookup"><span data-stu-id="beb65-162">Default setting for US Government.</span></span></li><li><span data-ttu-id="beb65-163">`adminsAndGuestInviters` -允许全局管理员、用户管理员和来宾邀请者角色的成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="beb65-163">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="beb65-164">`adminsGuestInvitersAndAllMembers` -允许上述管理员角色和所有其他用户角色成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="beb65-164">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="beb65-165">`everyone` -允许组织中的每个人（包括来宾用户）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="beb65-165">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="beb65-166">除美国政府之外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="beb65-166">Default setting for all cloud environments except US Government.</span></span></li></ul> |
|<span data-ttu-id="beb65-167">permissionGrantPolicyIdsAssignedToDefaultUserRole</span><span class="sxs-lookup"><span data-stu-id="beb65-167">permissionGrantPolicyIdsAssignedToDefaultUserRole</span></span>|<span data-ttu-id="beb65-168">字符串集合</span><span class="sxs-lookup"><span data-stu-id="beb65-168">String collection</span></span>|<span data-ttu-id="beb65-169">指示是否允许用户同意应用程序，如果是，则 (permissionGrantPolicy) 的应用程序许可策略控制授予许可的用户的权限。</span><span class="sxs-lookup"><span data-stu-id="beb65-169">Indicates if user consent to apps is allowed, and if it is, which app consent policy (permissionGrantPolicy) governs the permission for users to grant consent.</span></span> <span data-ttu-id="beb65-170">值的格式应为 `managePermissionGrantsForSelf.{id}` ，其中 `{id}` 是内置或自定义[应用程序许可策略](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-app-consent-policies)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="beb65-170">Values should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="beb65-171">空列表指示用户同意应用程序已被禁用。</span><span class="sxs-lookup"><span data-stu-id="beb65-171">An empty list indicates user consent to apps is disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="beb65-172">关系</span><span class="sxs-lookup"><span data-stu-id="beb65-172">Relationships</span></span>

<span data-ttu-id="beb65-173">无。</span><span class="sxs-lookup"><span data-stu-id="beb65-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="beb65-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="beb65-174">JSON representation</span></span>

<span data-ttu-id="beb65-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="beb65-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authorizationPolicy",
  "baseType": "",
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
