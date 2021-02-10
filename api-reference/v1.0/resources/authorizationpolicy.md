---
title: authorizationPolicy 资源类型
description: 表示可以控制 Azure Active Directory 的授权设置的策略。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 12fe4ad670d2bb5056d05fde533d4b690068f7a5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154213"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="3e896-103">authorizationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e896-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="3e896-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e896-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e896-105">表示可控制 Azure Active Directory 授权设置的策略。</span><span class="sxs-lookup"><span data-stu-id="3e896-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="3e896-106">它是从基本策略类型继承的单一对象，并且始终存在于租户中。</span><span class="sxs-lookup"><span data-stu-id="3e896-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="3e896-107">方法</span><span class="sxs-lookup"><span data-stu-id="3e896-107">Methods</span></span>

| <span data-ttu-id="3e896-108">方法</span><span class="sxs-lookup"><span data-stu-id="3e896-108">Method</span></span>       | <span data-ttu-id="3e896-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3e896-109">Return Type</span></span> | <span data-ttu-id="3e896-110">说明</span><span class="sxs-lookup"><span data-stu-id="3e896-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3e896-111">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="3e896-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="3e896-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="3e896-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="3e896-113">读取 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="3e896-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="3e896-114">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="3e896-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="3e896-115">无</span><span class="sxs-lookup"><span data-stu-id="3e896-115">None</span></span> | <span data-ttu-id="3e896-116">更新 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="3e896-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3e896-117">属性</span><span class="sxs-lookup"><span data-stu-id="3e896-117">Properties</span></span>  
| <span data-ttu-id="3e896-118">属性</span><span class="sxs-lookup"><span data-stu-id="3e896-118">Property</span></span> | <span data-ttu-id="3e896-119">类型</span><span class="sxs-lookup"><span data-stu-id="3e896-119">Type</span></span> | <span data-ttu-id="3e896-120">说明</span><span class="sxs-lookup"><span data-stu-id="3e896-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="3e896-121">id</span><span class="sxs-lookup"><span data-stu-id="3e896-121">id</span></span>|<span data-ttu-id="3e896-122">String</span><span class="sxs-lookup"><span data-stu-id="3e896-122">String</span></span>| <span data-ttu-id="3e896-123">授权策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="3e896-123">ID of the authorization policy.</span></span> <span data-ttu-id="3e896-124">必需。</span><span class="sxs-lookup"><span data-stu-id="3e896-124">Required.</span></span> <span data-ttu-id="3e896-125">只读。</span><span class="sxs-lookup"><span data-stu-id="3e896-125">Read-only.</span></span>| 
|<span data-ttu-id="3e896-126">displayName</span><span class="sxs-lookup"><span data-stu-id="3e896-126">displayName</span></span>|<span data-ttu-id="3e896-127">String</span><span class="sxs-lookup"><span data-stu-id="3e896-127">String</span></span>| <span data-ttu-id="3e896-128">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3e896-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="3e896-129">说明</span><span class="sxs-lookup"><span data-stu-id="3e896-129">description</span></span>|<span data-ttu-id="3e896-130">String</span><span class="sxs-lookup"><span data-stu-id="3e896-130">String</span></span>| <span data-ttu-id="3e896-131">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="3e896-131">Description of this policy.</span></span>|  
|<span data-ttu-id="3e896-132">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="3e896-132">blockMsolPowerShell</span></span>|<span data-ttu-id="3e896-133">布尔值</span><span class="sxs-lookup"><span data-stu-id="3e896-133">Boolean</span></span>| <span data-ttu-id="3e896-134">若要禁止使用 MSOL PowerShell，请设置此属性为 true。</span><span class="sxs-lookup"><span data-stu-id="3e896-134">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="3e896-135">设置为 true 还将禁用对 MSOL PowerShell 使用的旧服务终结点的基于用户的访问。</span><span class="sxs-lookup"><span data-stu-id="3e896-135">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="3e896-136">这不会影响 Azure AD Connect 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="3e896-136">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="3e896-137">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="3e896-137">defaultUserRolePermissions</span></span>|[<span data-ttu-id="3e896-138">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="3e896-138">defaultUserRolePermissions</span></span>](defaultuserrolepermissions.md)| <span data-ttu-id="3e896-139">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="3e896-139">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="3e896-140">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="3e896-140">allowedToUseSSPR</span></span>|<span data-ttu-id="3e896-141">布尔值</span><span class="sxs-lookup"><span data-stu-id="3e896-141">Boolean</span></span>| <span data-ttu-id="3e896-142">指示租户Self-Serve密码重置功能是否可以使用。</span><span class="sxs-lookup"><span data-stu-id="3e896-142">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="3e896-143">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="3e896-143">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="3e896-144">布尔值</span><span class="sxs-lookup"><span data-stu-id="3e896-144">Boolean</span></span>| <span data-ttu-id="3e896-145">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="3e896-145">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="3e896-146">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="3e896-146">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="3e896-147">布尔值</span><span class="sxs-lookup"><span data-stu-id="3e896-147">Boolean</span></span>| <span data-ttu-id="3e896-148">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="3e896-148">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="3e896-149">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="3e896-149">allowInvitesFrom</span></span>|<span data-ttu-id="3e896-150">String</span><span class="sxs-lookup"><span data-stu-id="3e896-150">String</span></span>|<span data-ttu-id="3e896-151">指示谁可以邀请外部用户加入组织。</span><span class="sxs-lookup"><span data-stu-id="3e896-151">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="3e896-152">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="3e896-152">Possible values are:</span></span><ul><li><span data-ttu-id="3e896-153">`none` - 阻止任何人（包括管理员）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="3e896-153">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="3e896-154">美国政府的默认设置。</span><span class="sxs-lookup"><span data-stu-id="3e896-154">Default setting for US Government.</span></span></li><li><span data-ttu-id="3e896-155">`adminsAndGuestInviters` - 允许全局管理员、用户管理员和来宾邀请者角色的成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="3e896-155">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="3e896-156">`adminsGuestInvitersAndAllMembers` - 允许上述管理员角色和所有其他用户角色成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="3e896-156">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="3e896-157">`everyone` - 允许组织中的每个人（包括来宾用户）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="3e896-157">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="3e896-158">除美国政府以外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="3e896-158">Default setting for all cloud environments except US Government.</span></span></li></ul> |

## <a name="relationships"></a><span data-ttu-id="3e896-159">关系</span><span class="sxs-lookup"><span data-stu-id="3e896-159">Relationships</span></span>

<span data-ttu-id="3e896-160">无。</span><span class="sxs-lookup"><span data-stu-id="3e896-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e896-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e896-161">JSON representation</span></span>

<span data-ttu-id="3e896-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e896-162">The following is a JSON representation of the resource.</span></span>

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
