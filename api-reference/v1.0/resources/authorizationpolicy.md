---
title: authorizationPolicy 资源类型
description: 表示可以控制用户授权设置Azure Active Directory。
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b08284d99d88ffbfa38c950062986ba72da900d5
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231925"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="bec12-103">authorizationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="bec12-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="bec12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bec12-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bec12-105">表示可以控制授权Azure Active Directory的策略。</span><span class="sxs-lookup"><span data-stu-id="bec12-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="bec12-106">它是从基本策略类型继承的单一对象，并且始终存在于租户中。</span><span class="sxs-lookup"><span data-stu-id="bec12-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="bec12-107">方法</span><span class="sxs-lookup"><span data-stu-id="bec12-107">Methods</span></span>

| <span data-ttu-id="bec12-108">方法</span><span class="sxs-lookup"><span data-stu-id="bec12-108">Method</span></span>       | <span data-ttu-id="bec12-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="bec12-109">Return Type</span></span> | <span data-ttu-id="bec12-110">说明</span><span class="sxs-lookup"><span data-stu-id="bec12-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bec12-111">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="bec12-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="bec12-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="bec12-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="bec12-113">读取 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="bec12-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="bec12-114">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="bec12-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="bec12-115">无</span><span class="sxs-lookup"><span data-stu-id="bec12-115">None</span></span> | <span data-ttu-id="bec12-116">更新 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="bec12-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bec12-117">属性</span><span class="sxs-lookup"><span data-stu-id="bec12-117">Properties</span></span>  
| <span data-ttu-id="bec12-118">属性</span><span class="sxs-lookup"><span data-stu-id="bec12-118">Property</span></span> | <span data-ttu-id="bec12-119">类型</span><span class="sxs-lookup"><span data-stu-id="bec12-119">Type</span></span> | <span data-ttu-id="bec12-120">说明</span><span class="sxs-lookup"><span data-stu-id="bec12-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="bec12-121">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="bec12-121">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="bec12-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="bec12-122">Boolean</span></span>| <span data-ttu-id="bec12-123">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="bec12-123">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="bec12-124">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="bec12-124">allowedToUseSSPR</span></span>|<span data-ttu-id="bec12-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="bec12-125">Boolean</span></span>| <span data-ttu-id="bec12-126">指示租户Self-Serve是否可以使用密码重置功能。</span><span class="sxs-lookup"><span data-stu-id="bec12-126">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="bec12-127">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="bec12-127">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="bec12-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="bec12-128">Boolean</span></span>| <span data-ttu-id="bec12-129">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="bec12-129">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="bec12-130">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="bec12-130">allowInvitesFrom</span></span>|<span data-ttu-id="bec12-131">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="bec12-131">allowInvitesFrom</span></span>|<span data-ttu-id="bec12-132">指示谁可以邀请外部用户加入组织。</span><span class="sxs-lookup"><span data-stu-id="bec12-132">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="bec12-133">可取值为：`none`、`adminsAndGuestInviters`、`adminsGuestInvitersAndAllMembers`、`everyone`。</span><span class="sxs-lookup"><span data-stu-id="bec12-133">Possible values are: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span></span>  <span data-ttu-id="bec12-134">`everyone` 是除美国政府以外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="bec12-134">`everyone` is the default setting for all cloud environments except US Government.</span></span> <span data-ttu-id="bec12-135">请参阅下表中的 [，了解](#allowinvitesfrom-values)。</span><span class="sxs-lookup"><span data-stu-id="bec12-135">See more in the [table below](#allowinvitesfrom-values).</span></span> |
|<span data-ttu-id="bec12-136">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="bec12-136">blockMsolPowerShell</span></span>|<span data-ttu-id="bec12-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="bec12-137">Boolean</span></span>| <span data-ttu-id="bec12-138">若要禁止使用 MSOL PowerShell，将此属性设置为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="bec12-138">To disable the use of MSOL PowerShell set this property to `true`.</span></span> <span data-ttu-id="bec12-139">这还将禁止基于用户对 MSOL PowerShell 使用的旧服务终结点的访问。</span><span class="sxs-lookup"><span data-stu-id="bec12-139">This will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="bec12-140">这不会影响 Azure AD 连接 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="bec12-140">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="bec12-141">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="bec12-141">defaultUserRolePermissions</span></span>|[<span data-ttu-id="bec12-142">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="bec12-142">defaultUserRolePermissions</span></span>](defaultuserrolepermissions.md)| <span data-ttu-id="bec12-143">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="bec12-143">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="bec12-144">说明</span><span class="sxs-lookup"><span data-stu-id="bec12-144">description</span></span>|<span data-ttu-id="bec12-145">String</span><span class="sxs-lookup"><span data-stu-id="bec12-145">String</span></span>| <span data-ttu-id="bec12-146">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="bec12-146">Description of this policy.</span></span>|
|<span data-ttu-id="bec12-147">displayName</span><span class="sxs-lookup"><span data-stu-id="bec12-147">displayName</span></span>|<span data-ttu-id="bec12-148">String</span><span class="sxs-lookup"><span data-stu-id="bec12-148">String</span></span>| <span data-ttu-id="bec12-149">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bec12-149">Display name for this policy.</span></span> |    
|<span data-ttu-id="bec12-150">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="bec12-150">guestUserRoleId</span></span>|<span data-ttu-id="bec12-151">Guid</span><span class="sxs-lookup"><span data-stu-id="bec12-151">Guid</span></span>| <span data-ttu-id="bec12-152">表示应授予来宾用户的角色的角色 templateId。</span><span class="sxs-lookup"><span data-stu-id="bec12-152">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="bec12-153">当前支持以下角色：用户角色 () 、来宾用户 `a0b1b346-4d3e-4e8b-98f8-753987be4970` `10dae51f-b6af-4016-8d66-8c2a99b929b3` () 和受限来宾 `2af84b1e-32c8-42b7-82bc-daa82404023b` () 。</span><span class="sxs-lookup"><span data-stu-id="bec12-153">Currently following roles are supported:  User (`a0b1b346-4d3e-4e8b-98f8-753987be4970`), Guest User (`10dae51f-b6af-4016-8d66-8c2a99b929b3`), and Restricted Guest User (`2af84b1e-32c8-42b7-82bc-daa82404023b`).</span></span> |
|<span data-ttu-id="bec12-154">id</span><span class="sxs-lookup"><span data-stu-id="bec12-154">id</span></span>|<span data-ttu-id="bec12-155">String</span><span class="sxs-lookup"><span data-stu-id="bec12-155">String</span></span>| <span data-ttu-id="bec12-156">授权策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="bec12-156">ID of the authorization policy.</span></span> <span data-ttu-id="bec12-157">必需。</span><span class="sxs-lookup"><span data-stu-id="bec12-157">Required.</span></span> <span data-ttu-id="bec12-158">只读。</span><span class="sxs-lookup"><span data-stu-id="bec12-158">Read-only.</span></span>| 

### <a name="allowinvitesfrom-values"></a><span data-ttu-id="bec12-159">allowInvitesFrom 值</span><span class="sxs-lookup"><span data-stu-id="bec12-159">allowInvitesFrom values</span></span>

|<span data-ttu-id="bec12-160">成员</span><span class="sxs-lookup"><span data-stu-id="bec12-160">Member</span></span>|<span data-ttu-id="bec12-161">说明</span><span class="sxs-lookup"><span data-stu-id="bec12-161">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bec12-162">无</span><span class="sxs-lookup"><span data-stu-id="bec12-162">none</span></span>|<span data-ttu-id="bec12-163">阻止包括管理员在内的所有人邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="bec12-163">Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="bec12-164">美国政府的默认设置。</span><span class="sxs-lookup"><span data-stu-id="bec12-164">Default setting for US Government.</span></span>|
|<span data-ttu-id="bec12-165">adminsAndGuestInviters</span><span class="sxs-lookup"><span data-stu-id="bec12-165">adminsAndGuestInviters</span></span>|<span data-ttu-id="bec12-166">允许全局管理员、用户管理员和来宾邀请者角色的成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="bec12-166">Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span>|
|<span data-ttu-id="bec12-167">adminsGuestInvitersAndAllMembers</span><span class="sxs-lookup"><span data-stu-id="bec12-167">adminsGuestInvitersAndAllMembers</span></span>|<span data-ttu-id="bec12-168">允许上述管理员角色和所有其他用户角色成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="bec12-168">Allow the above admin roles and all other User role members to invite external users.</span></span>|
|<span data-ttu-id="bec12-169">everyone</span><span class="sxs-lookup"><span data-stu-id="bec12-169">everyone</span></span>|<span data-ttu-id="bec12-170">允许组织中的每个人（包括来宾用户）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="bec12-170">Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="bec12-171">除美国政府以外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="bec12-171">The default setting for all cloud environments except US Government.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bec12-172">关系</span><span class="sxs-lookup"><span data-stu-id="bec12-172">Relationships</span></span>

<span data-ttu-id="bec12-173">无。</span><span class="sxs-lookup"><span data-stu-id="bec12-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bec12-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bec12-174">JSON representation</span></span>

<span data-ttu-id="bec12-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bec12-175">The following is a JSON representation of the resource.</span></span>

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
  "blockMsolPowerShell": true,
  "defaultUserRolePermissions": {"@odata.type": "microsoft.graph.defaultUserRolePermissions"},
  "allowedToUseSSPR": true,
  "allowedToSignUpEmailBasedSubscriptions": true,
  "allowEmailVerifiedUsersToJoinOrganization": true,
  "allowInvitesFrom": "String",
  "guestUserRoleId": "Guid"
}
```
