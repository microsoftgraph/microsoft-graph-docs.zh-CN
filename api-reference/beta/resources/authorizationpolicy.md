---
title: authorizationPolicy 资源类型
description: 表示可控制 Azure Active Directory 的授权设置的策略。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 20b7d1f9813873bb7233a8e3c8c35fe88e1c460c
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364304"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="517dc-103">authorizationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="517dc-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="517dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="517dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="517dc-105">表示可控制 Azure Active Directory 授权设置的策略。</span><span class="sxs-lookup"><span data-stu-id="517dc-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="517dc-106">它是从基本策略类型继承的单一实例，并且对于租户始终存在。</span><span class="sxs-lookup"><span data-stu-id="517dc-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span> 

## <a name="methods"></a><span data-ttu-id="517dc-107">方法</span><span class="sxs-lookup"><span data-stu-id="517dc-107">Methods</span></span>

| <span data-ttu-id="517dc-108">方法</span><span class="sxs-lookup"><span data-stu-id="517dc-108">Method</span></span>       | <span data-ttu-id="517dc-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="517dc-109">Return Type</span></span> | <span data-ttu-id="517dc-110">说明</span><span class="sxs-lookup"><span data-stu-id="517dc-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="517dc-111">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="517dc-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="517dc-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="517dc-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="517dc-113">读取 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="517dc-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="517dc-114">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="517dc-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="517dc-115">无</span><span class="sxs-lookup"><span data-stu-id="517dc-115">None</span></span> | <span data-ttu-id="517dc-116">更新 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="517dc-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="517dc-117">属性</span><span class="sxs-lookup"><span data-stu-id="517dc-117">Properties</span></span>  
| <span data-ttu-id="517dc-118">属性</span><span class="sxs-lookup"><span data-stu-id="517dc-118">Property</span></span> | <span data-ttu-id="517dc-119">类型</span><span class="sxs-lookup"><span data-stu-id="517dc-119">Type</span></span> | <span data-ttu-id="517dc-120">说明</span><span class="sxs-lookup"><span data-stu-id="517dc-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="517dc-121">id</span><span class="sxs-lookup"><span data-stu-id="517dc-121">id</span></span>|<span data-ttu-id="517dc-122">字符串</span><span class="sxs-lookup"><span data-stu-id="517dc-122">String</span></span>| <span data-ttu-id="517dc-123">授权策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="517dc-123">ID of the authorization policy.</span></span> <span data-ttu-id="517dc-124">必需。</span><span class="sxs-lookup"><span data-stu-id="517dc-124">Required.</span></span> <span data-ttu-id="517dc-125">只读。</span><span class="sxs-lookup"><span data-stu-id="517dc-125">Read-only.</span></span>| 
|<span data-ttu-id="517dc-126">displayName</span><span class="sxs-lookup"><span data-stu-id="517dc-126">displayName</span></span>|<span data-ttu-id="517dc-127">字符串</span><span class="sxs-lookup"><span data-stu-id="517dc-127">String</span></span>| <span data-ttu-id="517dc-128">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="517dc-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="517dc-129">说明</span><span class="sxs-lookup"><span data-stu-id="517dc-129">description</span></span>|<span data-ttu-id="517dc-130">字符串</span><span class="sxs-lookup"><span data-stu-id="517dc-130">String</span></span>| <span data-ttu-id="517dc-131">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="517dc-131">Description of this policy.</span></span>|  
|<span data-ttu-id="517dc-132">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="517dc-132">guestUserRoleId</span></span>|<span data-ttu-id="517dc-133">Guid</span><span class="sxs-lookup"><span data-stu-id="517dc-133">Guid</span></span>| <span data-ttu-id="517dc-134">表示应向来宾用户授予的角色的角色 templateId。</span><span class="sxs-lookup"><span data-stu-id="517dc-134">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="517dc-135">若要查找可用角色模板的列表，请参阅 [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) 。</span><span class="sxs-lookup"><span data-stu-id="517dc-135">Refer to [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) to find the list of available role templates.</span></span> <span data-ttu-id="517dc-136">当前以下角色受支持： User (a0b1b346-4d3e-4e8b-98f8-753987be4970) 、Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3) 和受限制的来宾用户 (2af84b1e-32c8-42b7-82bc-daa82404023b) 。</span><span class="sxs-lookup"><span data-stu-id="517dc-136">Currently following roles are supported: User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="517dc-137">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="517dc-137">enabledPreviewFeatures</span></span>|<span data-ttu-id="517dc-138">集合 (字符串) </span><span class="sxs-lookup"><span data-stu-id="517dc-138">Collection(string)</span></span>| <span data-ttu-id="517dc-139">租户上启用了专用预览的功能列表。</span><span class="sxs-lookup"><span data-stu-id="517dc-139">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="517dc-140">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="517dc-140">blockMsolPowerShell</span></span>|<span data-ttu-id="517dc-141">布尔</span><span class="sxs-lookup"><span data-stu-id="517dc-141">Boolean</span></span>| <span data-ttu-id="517dc-142">若要禁用 MSOL PowerShell 的使用，请将此属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="517dc-142">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="517dc-143">如果设置为 true，则还将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。</span><span class="sxs-lookup"><span data-stu-id="517dc-143">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="517dc-144">这不会影响 Azure AD Connect 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="517dc-144">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="517dc-145">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="517dc-145">defaultUserRolePermissions</span></span>|[<span data-ttu-id="517dc-146">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="517dc-146">defaultUserRolePermissions</span></span>](defaultUserRolePermissions.md)| <span data-ttu-id="517dc-147">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="517dc-147">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="517dc-148">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="517dc-148">allowedToUseSSPR</span></span>|<span data-ttu-id="517dc-149">布尔</span><span class="sxs-lookup"><span data-stu-id="517dc-149">Boolean</span></span>| <span data-ttu-id="517dc-150">指示租户上的用户是否可以使用自助服务密码重置功能。</span><span class="sxs-lookup"><span data-stu-id="517dc-150">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="517dc-151">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="517dc-151">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="517dc-152">布尔</span><span class="sxs-lookup"><span data-stu-id="517dc-152">Boolean</span></span>| <span data-ttu-id="517dc-153">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="517dc-153">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="517dc-154">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="517dc-154">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="517dc-155">布尔</span><span class="sxs-lookup"><span data-stu-id="517dc-155">Boolean</span></span>| <span data-ttu-id="517dc-156">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="517dc-156">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="517dc-157">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="517dc-157">allowInvitesFrom</span></span>|<span data-ttu-id="517dc-158">字符串</span><span class="sxs-lookup"><span data-stu-id="517dc-158">String</span></span>|<span data-ttu-id="517dc-159">指示谁可以邀请外部用户加入组织。</span><span class="sxs-lookup"><span data-stu-id="517dc-159">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="517dc-160">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="517dc-160">Possible values are:</span></span><br/><span data-ttu-id="517dc-161">`none` -防止用户（包括管理员）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="517dc-161">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="517dc-162">美国政府版的默认设置。</span><span class="sxs-lookup"><span data-stu-id="517dc-162">Default setting for US Government.</span></span><br/><span data-ttu-id="517dc-163">`adminsAndGuestInviters` -允许全局管理员、用户管理员和来宾邀请者角色的成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="517dc-163">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span><br/><span data-ttu-id="517dc-164">`adminsGuestInvitersAndAllMembers` -允许上述管理员角色和所有其他用户角色成员邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="517dc-164">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span><br/><span data-ttu-id="517dc-165">`everyone` -允许组织中的每个人（包括来宾用户）邀请外部用户。</span><span class="sxs-lookup"><span data-stu-id="517dc-165">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="517dc-166">除美国政府之外的所有云环境的默认设置。</span><span class="sxs-lookup"><span data-stu-id="517dc-166">Default setting for all cloud environments except US Government.</span></span><br/><span data-ttu-id="517dc-167">`unknownFutureValue` -evolvable 枚举的占位符。</span><span class="sxs-lookup"><span data-stu-id="517dc-167">`unknownFutureValue` - placeholder for evolvable enums.</span></span> |

## <a name="relationships"></a><span data-ttu-id="517dc-168">关系</span><span class="sxs-lookup"><span data-stu-id="517dc-168">Relationships</span></span>
<span data-ttu-id="517dc-169">无。</span><span class="sxs-lookup"><span data-stu-id="517dc-169">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="517dc-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="517dc-170">JSON representation</span></span>

<span data-ttu-id="517dc-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="517dc-171">The following is a JSON representation of the resource.</span></span>

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
  "allowInvitesFrom": "String"
}
```


