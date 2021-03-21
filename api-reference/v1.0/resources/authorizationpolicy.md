---
title: authorizationPolicy 资源类型
description: 表示可以控制 Azure Active Directory 的授权设置的策略。
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 85af4636f52e49717e864f2ccb9d710fea313eb2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962516"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="e4694-103">authorizationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4694-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="e4694-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4694-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4694-105">表示可以控制 Azure Active Directory 授权设置的策略。</span><span class="sxs-lookup"><span data-stu-id="e4694-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="e4694-106">它是从基本策略类型继承的单一对象，并且始终存在于租户中。</span><span class="sxs-lookup"><span data-stu-id="e4694-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="e4694-107">Methods</span><span class="sxs-lookup"><span data-stu-id="e4694-107">Methods</span></span>

| <span data-ttu-id="e4694-108">方法</span><span class="sxs-lookup"><span data-stu-id="e4694-108">Method</span></span>       | <span data-ttu-id="e4694-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e4694-109">Return Type</span></span> | <span data-ttu-id="e4694-110">说明</span><span class="sxs-lookup"><span data-stu-id="e4694-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e4694-111">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="e4694-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="e4694-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="e4694-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="e4694-113">读取 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="e4694-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="e4694-114">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="e4694-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="e4694-115">无</span><span class="sxs-lookup"><span data-stu-id="e4694-115">None</span></span> | <span data-ttu-id="e4694-116">更新 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="e4694-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e4694-117">属性</span><span class="sxs-lookup"><span data-stu-id="e4694-117">Properties</span></span>  
| <span data-ttu-id="e4694-118">属性</span><span class="sxs-lookup"><span data-stu-id="e4694-118">Property</span></span> | <span data-ttu-id="e4694-119">类型</span><span class="sxs-lookup"><span data-stu-id="e4694-119">Type</span></span> | <span data-ttu-id="e4694-120">说明</span><span class="sxs-lookup"><span data-stu-id="e4694-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="e4694-121">id</span><span class="sxs-lookup"><span data-stu-id="e4694-121">id</span></span>|<span data-ttu-id="e4694-122">String</span><span class="sxs-lookup"><span data-stu-id="e4694-122">String</span></span>| <span data-ttu-id="e4694-123">授权策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="e4694-123">ID of the authorization policy.</span></span> <span data-ttu-id="e4694-124">必填。</span><span class="sxs-lookup"><span data-stu-id="e4694-124">Required.</span></span> <span data-ttu-id="e4694-125">只读。</span><span class="sxs-lookup"><span data-stu-id="e4694-125">Read-only.</span></span>| 
|<span data-ttu-id="e4694-126">displayName</span><span class="sxs-lookup"><span data-stu-id="e4694-126">displayName</span></span>|<span data-ttu-id="e4694-127">String</span><span class="sxs-lookup"><span data-stu-id="e4694-127">String</span></span>| <span data-ttu-id="e4694-128">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e4694-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="e4694-129">说明</span><span class="sxs-lookup"><span data-stu-id="e4694-129">description</span></span>|<span data-ttu-id="e4694-130">String</span><span class="sxs-lookup"><span data-stu-id="e4694-130">String</span></span>| <span data-ttu-id="e4694-131">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="e4694-131">Description of this policy.</span></span>|  
|<span data-ttu-id="e4694-132">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="e4694-132">blockMsolPowerShell</span></span>|<span data-ttu-id="e4694-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4694-133">Boolean</span></span>| <span data-ttu-id="e4694-134">若要禁止使用 MSOL PowerShell，请设置此属性为 true。</span><span class="sxs-lookup"><span data-stu-id="e4694-134">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="e4694-135">设置为 true 还将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。</span><span class="sxs-lookup"><span data-stu-id="e4694-135">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="e4694-136">这不会影响 Azure AD Connect 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="e4694-136">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="e4694-137">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="e4694-137">defaultUserRolePermissions</span></span>|[<span data-ttu-id="e4694-138">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="e4694-138">defaultUserRolePermissions</span></span>](defaultuserrolepermissions.md)| <span data-ttu-id="e4694-139">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="e4694-139">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="e4694-140">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="e4694-140">allowedToUseSSPR</span></span>|<span data-ttu-id="e4694-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4694-141">Boolean</span></span>| <span data-ttu-id="e4694-142">指示租户Self-Serve是否可以使用密码重置功能。</span><span class="sxs-lookup"><span data-stu-id="e4694-142">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="e4694-143">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="e4694-143">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="e4694-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4694-144">Boolean</span></span>| <span data-ttu-id="e4694-145">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="e4694-145">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="e4694-146">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="e4694-146">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="e4694-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4694-147">Boolean</span></span>| <span data-ttu-id="e4694-148">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="e4694-148">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="e4694-149">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="e4694-149">allowInvitesFrom</span></span>|<span data-ttu-id="e4694-150">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="e4694-150">allowInvitesFrom</span></span>|<span data-ttu-id="e4694-151">指示谁可以邀请外部用户加入组织。</span><span class="sxs-lookup"><span data-stu-id="e4694-151">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="e4694-152">可取值为：`none`、`adminsAndGuestInviters`、`adminsGuestInvitersAndAllMembers`、`everyone`。</span><span class="sxs-lookup"><span data-stu-id="e4694-152">Possible values are: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span></span>  <span data-ttu-id="e4694-153">`everyone` 是除美国政府以外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="e4694-153">`everyone` is the default setting for all cloud environments except US Government.</span></span> <span data-ttu-id="e4694-154">请参阅下表 [中的更多内容](#allowinvitesfrom-values)。</span><span class="sxs-lookup"><span data-stu-id="e4694-154">See more in the [table below](#allowinvitesfrom-values).</span></span> |

### <a name="allowinvitesfrom-values"></a><span data-ttu-id="e4694-155">allowInvitesFrom 值</span><span class="sxs-lookup"><span data-stu-id="e4694-155">allowInvitesFrom values</span></span>

|<span data-ttu-id="e4694-156">成员</span><span class="sxs-lookup"><span data-stu-id="e4694-156">Member</span></span>|<span data-ttu-id="e4694-157">说明</span><span class="sxs-lookup"><span data-stu-id="e4694-157">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e4694-158">无</span><span class="sxs-lookup"><span data-stu-id="e4694-158">none</span></span>|<span data-ttu-id="e4694-159">阻止包括管理员在内的所有人邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="e4694-159">Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="e4694-160">美国政府的默认设置。</span><span class="sxs-lookup"><span data-stu-id="e4694-160">Default setting for US Government.</span></span>|
|<span data-ttu-id="e4694-161">adminsAndGuestInviters</span><span class="sxs-lookup"><span data-stu-id="e4694-161">adminsAndGuestInviters</span></span>|<span data-ttu-id="e4694-162">允许全局管理员、用户管理员和来宾邀请者角色的成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="e4694-162">Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span>|
|<span data-ttu-id="e4694-163">adminsGuestInvitersAndAllMembers</span><span class="sxs-lookup"><span data-stu-id="e4694-163">adminsGuestInvitersAndAllMembers</span></span>|<span data-ttu-id="e4694-164">允许上述管理员角色和所有其他用户角色成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="e4694-164">Allow the above admin roles and all other User role members to invite external users.</span></span>|
|<span data-ttu-id="e4694-165">everyone</span><span class="sxs-lookup"><span data-stu-id="e4694-165">everyone</span></span>|<span data-ttu-id="e4694-166">允许组织中的每个人（包括来宾用户）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="e4694-166">Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="e4694-167">除美国政府以外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="e4694-167">The default setting for all cloud environments except US Government.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4694-168">关系</span><span class="sxs-lookup"><span data-stu-id="e4694-168">Relationships</span></span>

<span data-ttu-id="e4694-169">无。</span><span class="sxs-lookup"><span data-stu-id="e4694-169">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4694-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4694-170">JSON representation</span></span>

<span data-ttu-id="e4694-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4694-171">The following is a JSON representation of the resource.</span></span>

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
  "allowInvitesFrom": "String"
}
```
