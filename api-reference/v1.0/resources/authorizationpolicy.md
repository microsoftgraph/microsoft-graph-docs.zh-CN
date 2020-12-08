---
title: authorizationPolicy 资源类型
description: 表示可控制 Azure Active Directory 的授权设置的策略。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c71e4d01ba54c9043ff827b3749be63442d06ac
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581198"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="31975-103">authorizationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="31975-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="31975-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31975-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="31975-105">表示可控制 Azure Active Directory 授权设置的策略。</span><span class="sxs-lookup"><span data-stu-id="31975-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="31975-106">它是从基本策略类型继承的单一实例，并且对于租户始终存在。</span><span class="sxs-lookup"><span data-stu-id="31975-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="31975-107">方法</span><span class="sxs-lookup"><span data-stu-id="31975-107">Methods</span></span>

| <span data-ttu-id="31975-108">方法</span><span class="sxs-lookup"><span data-stu-id="31975-108">Method</span></span>       | <span data-ttu-id="31975-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="31975-109">Return Type</span></span> | <span data-ttu-id="31975-110">Description</span><span class="sxs-lookup"><span data-stu-id="31975-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="31975-111">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="31975-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="31975-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="31975-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="31975-113">读取 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="31975-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="31975-114">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="31975-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="31975-115">无</span><span class="sxs-lookup"><span data-stu-id="31975-115">None</span></span> | <span data-ttu-id="31975-116">更新 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="31975-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="31975-117">属性</span><span class="sxs-lookup"><span data-stu-id="31975-117">Properties</span></span>  
| <span data-ttu-id="31975-118">属性</span><span class="sxs-lookup"><span data-stu-id="31975-118">Property</span></span> | <span data-ttu-id="31975-119">类型</span><span class="sxs-lookup"><span data-stu-id="31975-119">Type</span></span> | <span data-ttu-id="31975-120">说明</span><span class="sxs-lookup"><span data-stu-id="31975-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="31975-121">id</span><span class="sxs-lookup"><span data-stu-id="31975-121">id</span></span>|<span data-ttu-id="31975-122">String</span><span class="sxs-lookup"><span data-stu-id="31975-122">String</span></span>| <span data-ttu-id="31975-123">授权策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="31975-123">ID of the authorization policy.</span></span> <span data-ttu-id="31975-124">必需。</span><span class="sxs-lookup"><span data-stu-id="31975-124">Required.</span></span> <span data-ttu-id="31975-125">只读。</span><span class="sxs-lookup"><span data-stu-id="31975-125">Read-only.</span></span>| 
|<span data-ttu-id="31975-126">displayName</span><span class="sxs-lookup"><span data-stu-id="31975-126">displayName</span></span>|<span data-ttu-id="31975-127">String</span><span class="sxs-lookup"><span data-stu-id="31975-127">String</span></span>| <span data-ttu-id="31975-128">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="31975-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="31975-129">说明</span><span class="sxs-lookup"><span data-stu-id="31975-129">description</span></span>|<span data-ttu-id="31975-130">String</span><span class="sxs-lookup"><span data-stu-id="31975-130">String</span></span>| <span data-ttu-id="31975-131">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="31975-131">Description of this policy.</span></span>|  
|<span data-ttu-id="31975-132">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="31975-132">blockMsolPowerShell</span></span>|<span data-ttu-id="31975-133">布尔值</span><span class="sxs-lookup"><span data-stu-id="31975-133">Boolean</span></span>| <span data-ttu-id="31975-134">若要禁用 MSOL PowerShell 的使用，请将此属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="31975-134">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="31975-135">如果设置为 true，则还将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。</span><span class="sxs-lookup"><span data-stu-id="31975-135">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="31975-136">这不会影响 Azure AD Connect 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="31975-136">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="31975-137">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="31975-137">defaultUserRolePermissions</span></span>|[<span data-ttu-id="31975-138">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="31975-138">defaultUserRolePermissions</span></span>](defaultuserrolepermissions.md)| <span data-ttu-id="31975-139">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="31975-139">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="31975-140">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="31975-140">allowedToUseSSPR</span></span>|<span data-ttu-id="31975-141">布尔值</span><span class="sxs-lookup"><span data-stu-id="31975-141">Boolean</span></span>| <span data-ttu-id="31975-142">指示租户上的用户是否可以使用 Self-Serve 密码重置功能。</span><span class="sxs-lookup"><span data-stu-id="31975-142">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="31975-143">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="31975-143">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="31975-144">布尔值</span><span class="sxs-lookup"><span data-stu-id="31975-144">Boolean</span></span>| <span data-ttu-id="31975-145">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="31975-145">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="31975-146">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="31975-146">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="31975-147">布尔值</span><span class="sxs-lookup"><span data-stu-id="31975-147">Boolean</span></span>| <span data-ttu-id="31975-148">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="31975-148">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="31975-149">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="31975-149">allowInvitesFrom</span></span>|<span data-ttu-id="31975-150">String</span><span class="sxs-lookup"><span data-stu-id="31975-150">String</span></span>|<span data-ttu-id="31975-151">指示谁可以邀请外部用户加入组织。</span><span class="sxs-lookup"><span data-stu-id="31975-151">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="31975-152">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="31975-152">Possible values are:</span></span><ul><li><span data-ttu-id="31975-153">`none` -防止用户（包括管理员）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="31975-153">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="31975-154">美国政府版的默认设置。</span><span class="sxs-lookup"><span data-stu-id="31975-154">Default setting for US Government.</span></span></li><li><span data-ttu-id="31975-155">`adminsAndGuestInviters` -允许全局管理员、用户管理员和来宾邀请者角色的成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="31975-155">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="31975-156">`adminsGuestInvitersAndAllMembers` -允许上述管理员角色和所有其他用户角色成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="31975-156">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="31975-157">`everyone` -允许组织中的每个人（包括来宾用户）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="31975-157">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="31975-158">除美国政府之外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="31975-158">Default setting for all cloud environments except US Government.</span></span></li></ul> |

## <a name="relationships"></a><span data-ttu-id="31975-159">关系</span><span class="sxs-lookup"><span data-stu-id="31975-159">Relationships</span></span>

<span data-ttu-id="31975-160">无。</span><span class="sxs-lookup"><span data-stu-id="31975-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31975-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31975-161">JSON representation</span></span>

<span data-ttu-id="31975-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31975-162">The following is a JSON representation of the resource.</span></span>

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
  "blockMsolPowerShell": true,
  "defaultUserRolePermissions": {"@odata.type": "microsoft.graph.defaultUserRolePermissions"},
  "allowedToUseSSPR": true,
  "allowedToSignUpEmailBasedSubscriptions": true,
  "allowEmailVerifiedUsersToJoinOrganization": true,
  "allowInvitesFrom": "String"
}
```
