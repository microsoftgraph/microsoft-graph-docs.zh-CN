---
title: authorizationPolicy 资源类型
description: 表示可控制 Azure Active Directory 的授权设置的策略。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c20f4dad0263e9d4c931e43da99870ed022f1e58
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492206"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="0bf04-103">authorizationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="0bf04-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="0bf04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bf04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bf04-105">表示可控制 Azure Active Directory 授权设置的策略。</span><span class="sxs-lookup"><span data-stu-id="0bf04-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="0bf04-106">它是从基本策略类型继承的单一实例，并且对于租户始终存在。</span><span class="sxs-lookup"><span data-stu-id="0bf04-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span> 

## <a name="methods"></a><span data-ttu-id="0bf04-107">Methods</span><span class="sxs-lookup"><span data-stu-id="0bf04-107">Methods</span></span>

| <span data-ttu-id="0bf04-108">方法</span><span class="sxs-lookup"><span data-stu-id="0bf04-108">Method</span></span>       | <span data-ttu-id="0bf04-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0bf04-109">Return Type</span></span> | <span data-ttu-id="0bf04-110">说明</span><span class="sxs-lookup"><span data-stu-id="0bf04-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0bf04-111">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="0bf04-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="0bf04-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="0bf04-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="0bf04-113">读取 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="0bf04-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="0bf04-114">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="0bf04-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="0bf04-115">无</span><span class="sxs-lookup"><span data-stu-id="0bf04-115">None</span></span> | <span data-ttu-id="0bf04-116">更新 authorizationPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="0bf04-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0bf04-117">属性</span><span class="sxs-lookup"><span data-stu-id="0bf04-117">Properties</span></span>  
| <span data-ttu-id="0bf04-118">属性</span><span class="sxs-lookup"><span data-stu-id="0bf04-118">Property</span></span> | <span data-ttu-id="0bf04-119">类型</span><span class="sxs-lookup"><span data-stu-id="0bf04-119">Type</span></span> | <span data-ttu-id="0bf04-120">说明</span><span class="sxs-lookup"><span data-stu-id="0bf04-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="0bf04-121">id</span><span class="sxs-lookup"><span data-stu-id="0bf04-121">id</span></span>|<span data-ttu-id="0bf04-122">字符串</span><span class="sxs-lookup"><span data-stu-id="0bf04-122">String</span></span>| <span data-ttu-id="0bf04-123">授权策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="0bf04-123">ID of the authorization policy.</span></span> <span data-ttu-id="0bf04-124">必填。</span><span class="sxs-lookup"><span data-stu-id="0bf04-124">Required.</span></span> <span data-ttu-id="0bf04-125">只读。</span><span class="sxs-lookup"><span data-stu-id="0bf04-125">Read-only.</span></span>| 
|<span data-ttu-id="0bf04-126">displayName</span><span class="sxs-lookup"><span data-stu-id="0bf04-126">displayName</span></span>|<span data-ttu-id="0bf04-127">String</span><span class="sxs-lookup"><span data-stu-id="0bf04-127">String</span></span>| <span data-ttu-id="0bf04-128">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0bf04-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="0bf04-129">说明</span><span class="sxs-lookup"><span data-stu-id="0bf04-129">description</span></span>|<span data-ttu-id="0bf04-130">String</span><span class="sxs-lookup"><span data-stu-id="0bf04-130">String</span></span>| <span data-ttu-id="0bf04-131">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="0bf04-131">Description of this policy.</span></span>|  
|<span data-ttu-id="0bf04-132">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="0bf04-132">guestUserRoleId</span></span>|<span data-ttu-id="0bf04-133">Guid</span><span class="sxs-lookup"><span data-stu-id="0bf04-133">Guid</span></span>| <span data-ttu-id="0bf04-134">表示应向来宾用户授予的角色的角色 templateId。</span><span class="sxs-lookup"><span data-stu-id="0bf04-134">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="0bf04-135">若要查找可用角色模板的列表，请参阅[List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) 。</span><span class="sxs-lookup"><span data-stu-id="0bf04-135">Refer to [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) to find the list of available role templates.</span></span> <span data-ttu-id="0bf04-136">当前以下角色受支持： User （a0b1b346-4d3e-4e8b-98f8-753987be4970）、Guest User （10dae51f-b6af-4016-8d66-8c2a99b929b3）和受限制的来宾用户（2af84b1e-32c8-42b7-82bc-daa82404023b）。</span><span class="sxs-lookup"><span data-stu-id="0bf04-136">Currently following roles are supported: User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="0bf04-137">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="0bf04-137">enabledPreviewFeatures</span></span>|<span data-ttu-id="0bf04-138">集合（string）</span><span class="sxs-lookup"><span data-stu-id="0bf04-138">Collection(string)</span></span>| <span data-ttu-id="0bf04-139">租户上启用了专用预览的功能列表。</span><span class="sxs-lookup"><span data-stu-id="0bf04-139">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="0bf04-140">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="0bf04-140">blockMsolPowerShell</span></span>|<span data-ttu-id="0bf04-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bf04-141">Boolean</span></span>| <span data-ttu-id="0bf04-142">若要禁用 MSOL PowerShell 的使用，请将此属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="0bf04-142">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="0bf04-143">如果设置为 true，则还将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。</span><span class="sxs-lookup"><span data-stu-id="0bf04-143">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="0bf04-144">这不会影响 Azure AD Connect 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="0bf04-144">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 


## <a name="relationships"></a><span data-ttu-id="0bf04-145">关系</span><span class="sxs-lookup"><span data-stu-id="0bf04-145">Relationships</span></span>
<span data-ttu-id="0bf04-146">无。</span><span class="sxs-lookup"><span data-stu-id="0bf04-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bf04-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0bf04-147">JSON representation</span></span>

<span data-ttu-id="0bf04-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0bf04-148">The following is a JSON representation of the resource.</span></span>

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
  "blockMsolPowerShell": true 
}
```
