---
title: authorizationPolicy 资源类型
description: 表示可控制 Azure Active Directory 的授权设置的策略。
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ce482195ce7921eb43f2e4d1845a95f750688f1a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448868"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="7c344-103">authorizationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c344-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="7c344-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c344-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c344-105">表示可控制 Azure Active Directory 授权设置的策略。</span><span class="sxs-lookup"><span data-stu-id="7c344-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="7c344-106">它是从基本策略类型继承的单一对象，并且始终存在于租户中。</span><span class="sxs-lookup"><span data-stu-id="7c344-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="7c344-107">Methods</span><span class="sxs-lookup"><span data-stu-id="7c344-107">Methods</span></span>

| <span data-ttu-id="7c344-108">方法</span><span class="sxs-lookup"><span data-stu-id="7c344-108">Method</span></span>       | <span data-ttu-id="7c344-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7c344-109">Return Type</span></span> | <span data-ttu-id="7c344-110">说明</span><span class="sxs-lookup"><span data-stu-id="7c344-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7c344-111">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="7c344-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="7c344-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="7c344-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="7c344-113">读取 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="7c344-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="7c344-114">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="7c344-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="7c344-115">无</span><span class="sxs-lookup"><span data-stu-id="7c344-115">None</span></span> | <span data-ttu-id="7c344-116">更新 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="7c344-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7c344-117">属性</span><span class="sxs-lookup"><span data-stu-id="7c344-117">Properties</span></span>  
| <span data-ttu-id="7c344-118">属性</span><span class="sxs-lookup"><span data-stu-id="7c344-118">Property</span></span> | <span data-ttu-id="7c344-119">类型</span><span class="sxs-lookup"><span data-stu-id="7c344-119">Type</span></span> | <span data-ttu-id="7c344-120">说明</span><span class="sxs-lookup"><span data-stu-id="7c344-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="7c344-121">id</span><span class="sxs-lookup"><span data-stu-id="7c344-121">id</span></span>|<span data-ttu-id="7c344-122">String</span><span class="sxs-lookup"><span data-stu-id="7c344-122">String</span></span>| <span data-ttu-id="7c344-123">授权策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="7c344-123">ID of the authorization policy.</span></span> <span data-ttu-id="7c344-124">必填。</span><span class="sxs-lookup"><span data-stu-id="7c344-124">Required.</span></span> <span data-ttu-id="7c344-125">只读。</span><span class="sxs-lookup"><span data-stu-id="7c344-125">Read-only.</span></span>| 
|<span data-ttu-id="7c344-126">displayName</span><span class="sxs-lookup"><span data-stu-id="7c344-126">displayName</span></span>|<span data-ttu-id="7c344-127">String</span><span class="sxs-lookup"><span data-stu-id="7c344-127">String</span></span>| <span data-ttu-id="7c344-128">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7c344-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="7c344-129">说明</span><span class="sxs-lookup"><span data-stu-id="7c344-129">description</span></span>|<span data-ttu-id="7c344-130">String</span><span class="sxs-lookup"><span data-stu-id="7c344-130">String</span></span>| <span data-ttu-id="7c344-131">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="7c344-131">Description of this policy.</span></span>|  
|<span data-ttu-id="7c344-132">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="7c344-132">blockMsolPowerShell</span></span>|<span data-ttu-id="7c344-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c344-133">Boolean</span></span>| <span data-ttu-id="7c344-134">若要禁止使用 MSOL PowerShell，请设置此属性为 true。</span><span class="sxs-lookup"><span data-stu-id="7c344-134">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="7c344-135">设置为 true 还将禁用对 MSOL PowerShell 使用的旧服务终结点的基于用户的访问。</span><span class="sxs-lookup"><span data-stu-id="7c344-135">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="7c344-136">这不会影响 Azure AD Connect 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="7c344-136">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="7c344-137">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="7c344-137">defaultUserRolePermissions</span></span>|[<span data-ttu-id="7c344-138">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="7c344-138">defaultUserRolePermissions</span></span>](defaultuserrolepermissions.md)| <span data-ttu-id="7c344-139">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="7c344-139">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="7c344-140">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="7c344-140">allowedToUseSSPR</span></span>|<span data-ttu-id="7c344-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c344-141">Boolean</span></span>| <span data-ttu-id="7c344-142">指示租户Self-Serve密码重置功能是否可以使用。</span><span class="sxs-lookup"><span data-stu-id="7c344-142">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="7c344-143">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="7c344-143">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="7c344-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c344-144">Boolean</span></span>| <span data-ttu-id="7c344-145">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="7c344-145">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="7c344-146">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="7c344-146">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="7c344-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c344-147">Boolean</span></span>| <span data-ttu-id="7c344-148">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="7c344-148">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="7c344-149">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="7c344-149">allowInvitesFrom</span></span>|<span data-ttu-id="7c344-150">String</span><span class="sxs-lookup"><span data-stu-id="7c344-150">String</span></span>|<span data-ttu-id="7c344-151">指示可以邀请外部用户加入组织的用户。</span><span class="sxs-lookup"><span data-stu-id="7c344-151">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="7c344-152">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="7c344-152">Possible values are:</span></span><ul><li><span data-ttu-id="7c344-153">`none` - 阻止包括管理员在内的所有人邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="7c344-153">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="7c344-154">美国政府的默认设置。</span><span class="sxs-lookup"><span data-stu-id="7c344-154">Default setting for US Government.</span></span></li><li><span data-ttu-id="7c344-155">`adminsAndGuestInviters` - 允许全局管理员、用户管理员和来宾邀请者角色的成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="7c344-155">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="7c344-156">`adminsGuestInvitersAndAllMembers` - 允许上述管理员角色和所有其他用户角色成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="7c344-156">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="7c344-157">`everyone` - 允许组织中的每个人（包括来宾用户）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="7c344-157">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="7c344-158">除美国政府以外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="7c344-158">Default setting for all cloud environments except US Government.</span></span></li></ul> |

## <a name="relationships"></a><span data-ttu-id="7c344-159">关系</span><span class="sxs-lookup"><span data-stu-id="7c344-159">Relationships</span></span>

<span data-ttu-id="7c344-160">无。</span><span class="sxs-lookup"><span data-stu-id="7c344-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c344-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c344-161">JSON representation</span></span>

<span data-ttu-id="7c344-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c344-162">The following is a JSON representation of the resource.</span></span>

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
