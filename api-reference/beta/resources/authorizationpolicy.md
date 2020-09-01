---
title: authorizationPolicy 资源类型
description: 表示可控制 Azure Active Directory 的授权设置的策略。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: be8fb874dfd05a1e337bd9189e6542cade2e0a16
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319582"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="a1192-103">authorizationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1192-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="a1192-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1192-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1192-105">表示可控制 Azure Active Directory 授权设置的策略。</span><span class="sxs-lookup"><span data-stu-id="a1192-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="a1192-106">它是从基本策略类型继承的单一实例，并且对于租户始终存在。</span><span class="sxs-lookup"><span data-stu-id="a1192-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span> 

## <a name="methods"></a><span data-ttu-id="a1192-107">方法</span><span class="sxs-lookup"><span data-stu-id="a1192-107">Methods</span></span>

| <span data-ttu-id="a1192-108">方法</span><span class="sxs-lookup"><span data-stu-id="a1192-108">Method</span></span>       | <span data-ttu-id="a1192-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a1192-109">Return Type</span></span> | <span data-ttu-id="a1192-110">说明</span><span class="sxs-lookup"><span data-stu-id="a1192-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a1192-111">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="a1192-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="a1192-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="a1192-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="a1192-113">读取 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="a1192-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="a1192-114">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="a1192-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="a1192-115">无</span><span class="sxs-lookup"><span data-stu-id="a1192-115">None</span></span> | <span data-ttu-id="a1192-116">更新 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="a1192-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a1192-117">属性</span><span class="sxs-lookup"><span data-stu-id="a1192-117">Properties</span></span>  
| <span data-ttu-id="a1192-118">属性</span><span class="sxs-lookup"><span data-stu-id="a1192-118">Property</span></span> | <span data-ttu-id="a1192-119">类型</span><span class="sxs-lookup"><span data-stu-id="a1192-119">Type</span></span> | <span data-ttu-id="a1192-120">说明</span><span class="sxs-lookup"><span data-stu-id="a1192-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="a1192-121">id</span><span class="sxs-lookup"><span data-stu-id="a1192-121">id</span></span>|<span data-ttu-id="a1192-122">String</span><span class="sxs-lookup"><span data-stu-id="a1192-122">String</span></span>| <span data-ttu-id="a1192-123">授权策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="a1192-123">ID of the authorization policy.</span></span> <span data-ttu-id="a1192-124">必需。</span><span class="sxs-lookup"><span data-stu-id="a1192-124">Required.</span></span> <span data-ttu-id="a1192-125">只读。</span><span class="sxs-lookup"><span data-stu-id="a1192-125">Read-only.</span></span>| 
|<span data-ttu-id="a1192-126">displayName</span><span class="sxs-lookup"><span data-stu-id="a1192-126">displayName</span></span>|<span data-ttu-id="a1192-127">String</span><span class="sxs-lookup"><span data-stu-id="a1192-127">String</span></span>| <span data-ttu-id="a1192-128">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a1192-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="a1192-129">说明</span><span class="sxs-lookup"><span data-stu-id="a1192-129">description</span></span>|<span data-ttu-id="a1192-130">String</span><span class="sxs-lookup"><span data-stu-id="a1192-130">String</span></span>| <span data-ttu-id="a1192-131">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="a1192-131">Description of this policy.</span></span>|  
|<span data-ttu-id="a1192-132">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="a1192-132">guestUserRoleId</span></span>|<span data-ttu-id="a1192-133">Guid</span><span class="sxs-lookup"><span data-stu-id="a1192-133">Guid</span></span>| <span data-ttu-id="a1192-134">表示应向来宾用户授予的角色的角色 templateId。</span><span class="sxs-lookup"><span data-stu-id="a1192-134">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="a1192-135">若要查找可用角色模板的列表，请参阅 [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) 。</span><span class="sxs-lookup"><span data-stu-id="a1192-135">Refer to [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) to find the list of available role templates.</span></span> <span data-ttu-id="a1192-136">当前以下角色受支持： User (a0b1b346-4d3e-4e8b-98f8-753987be4970) 、Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3) 和受限制的来宾用户 (2af84b1e-32c8-42b7-82bc-daa82404023b) 。</span><span class="sxs-lookup"><span data-stu-id="a1192-136">Currently following roles are supported: User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="a1192-137">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="a1192-137">enabledPreviewFeatures</span></span>|<span data-ttu-id="a1192-138">集合 (字符串) </span><span class="sxs-lookup"><span data-stu-id="a1192-138">Collection(string)</span></span>| <span data-ttu-id="a1192-139">租户上启用了专用预览的功能列表。</span><span class="sxs-lookup"><span data-stu-id="a1192-139">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="a1192-140">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="a1192-140">blockMsolPowerShell</span></span>|<span data-ttu-id="a1192-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1192-141">Boolean</span></span>| <span data-ttu-id="a1192-142">若要禁用 MSOL PowerShell 的使用，请将此属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="a1192-142">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="a1192-143">如果设置为 true，则还将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。</span><span class="sxs-lookup"><span data-stu-id="a1192-143">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="a1192-144">这不会影响 Azure AD Connect 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="a1192-144">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="a1192-145">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="a1192-145">defaultUserRolePermissions</span></span>|[<span data-ttu-id="a1192-146">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="a1192-146">defaultUserRolePermissions</span></span>](defaultUserRolePermissions.md)| <span data-ttu-id="a1192-147">指定默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="a1192-147">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="a1192-148">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="a1192-148">allowedToUseSSPR</span></span>|<span data-ttu-id="a1192-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1192-149">Boolean</span></span>| <span data-ttu-id="a1192-150">指示租户上的用户是否可以使用自助服务密码重置功能。</span><span class="sxs-lookup"><span data-stu-id="a1192-150">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="a1192-151">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="a1192-151">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="a1192-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1192-152">Boolean</span></span>| <span data-ttu-id="a1192-153">指示用户是否可以注册基于电子邮件的订阅。</span><span class="sxs-lookup"><span data-stu-id="a1192-153">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="a1192-154">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="a1192-154">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="a1192-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1192-155">Boolean</span></span>| <span data-ttu-id="a1192-156">指示用户是否可以通过电子邮件验证加入租户。</span><span class="sxs-lookup"><span data-stu-id="a1192-156">Indicates whether a user can join the tenant by email validation.</span></span> | 


## <a name="relationships"></a><span data-ttu-id="a1192-157">关系</span><span class="sxs-lookup"><span data-stu-id="a1192-157">Relationships</span></span>
<span data-ttu-id="a1192-158">无。</span><span class="sxs-lookup"><span data-stu-id="a1192-158">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1192-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1192-159">JSON representation</span></span>

<span data-ttu-id="a1192-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1192-160">The following is a JSON representation of the resource.</span></span>

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
  "allowEmailVerifiedUsersToJoinOrganization": true
}
```
