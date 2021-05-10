---
title: unifiedRoleManagementPolicy 资源类型
description: unifiedRoleManagementPolicy 指定与作用域和角色定义关联的各种策略。 它派生自 microsoft.graph.policyBase。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 73510f928fa4a32e92ff0a50b3439ab60dfb95f8
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299177"
---
# <a name="unifiedrolemanagementpolicy-resource-type"></a><span data-ttu-id="a55a4-104">unifiedRoleManagementPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="a55a4-104">unifiedRoleManagementPolicy resource type</span></span>

<span data-ttu-id="a55a4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a55a4-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a55a4-106">unifiedRoleManagementPolicy 指定与作用域和角色定义关联的各种策略。</span><span class="sxs-lookup"><span data-stu-id="a55a4-106">A unifiedRoleManagementPolicy specifies the various policies associated with a scope and role definition.</span></span> <span data-ttu-id="a55a4-107">它派生自 microsoft.graph.policyBase。</span><span class="sxs-lookup"><span data-stu-id="a55a4-107">It is derived from microsoft.graph.policyBase.</span></span>

## <a name="methods"></a><span data-ttu-id="a55a4-108">方法</span><span class="sxs-lookup"><span data-stu-id="a55a4-108">Methods</span></span>
|<span data-ttu-id="a55a4-109">方法</span><span class="sxs-lookup"><span data-stu-id="a55a4-109">Method</span></span>|<span data-ttu-id="a55a4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a55a4-110">Return type</span></span>|<span data-ttu-id="a55a4-111">说明</span><span class="sxs-lookup"><span data-stu-id="a55a4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a55a4-112">列出 unifiedRoleManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="a55a4-112">List unifiedRoleManagementPolicies</span></span>](../api/unifiedrolemanagementpolicy-list.md)|<span data-ttu-id="a55a4-113">[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a55a4-113">[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection</span></span>|<span data-ttu-id="a55a4-114">获取 [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="a55a4-114">Get a list of the [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) objects and their properties.</span></span>|
|[<span data-ttu-id="a55a4-115">获取 unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a55a4-115">Get unifiedRoleManagementPolicy</span></span>](../api/unifiedrolemanagementpolicy-get.md)|[<span data-ttu-id="a55a4-116">unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a55a4-116">unifiedRoleManagementPolicy</span></span>](../resources/unifiedrolemanagementpolicy.md)|<span data-ttu-id="a55a4-117">读取 [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a55a4-117">Read the properties and relationships of an [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) object.</span></span>|
|[<span data-ttu-id="a55a4-118">列出 effectiveRules</span><span class="sxs-lookup"><span data-stu-id="a55a4-118">List effectiveRules</span></span>](../api/unifiedrolemanagementpolicy-list-effectiverules.md)|<span data-ttu-id="a55a4-119">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a55a4-119">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="a55a4-120">从 effectiveRules 导航属性获取 unifiedRoleManagementPolicyRule 资源。</span><span class="sxs-lookup"><span data-stu-id="a55a4-120">Get the unifiedRoleManagementPolicyRule resources from the effectiveRules navigation property.</span></span>|
|[<span data-ttu-id="a55a4-121">List rules</span><span class="sxs-lookup"><span data-stu-id="a55a4-121">List rules</span></span>](../api/unifiedrolemanagementpolicy-list-rules.md)|<span data-ttu-id="a55a4-122">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a55a4-122">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="a55a4-123">从 rules 导航属性获取 unifiedRoleManagementPolicyRule 资源。</span><span class="sxs-lookup"><span data-stu-id="a55a4-123">Get the unifiedRoleManagementPolicyRule resources from the rules navigation property.</span></span>|

## <a name="properties"></a><span data-ttu-id="a55a4-124">属性</span><span class="sxs-lookup"><span data-stu-id="a55a4-124">Properties</span></span>
|<span data-ttu-id="a55a4-125">属性</span><span class="sxs-lookup"><span data-stu-id="a55a4-125">Property</span></span>|<span data-ttu-id="a55a4-126">类型</span><span class="sxs-lookup"><span data-stu-id="a55a4-126">Type</span></span>|<span data-ttu-id="a55a4-127">说明</span><span class="sxs-lookup"><span data-stu-id="a55a4-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a55a4-128">说明</span><span class="sxs-lookup"><span data-stu-id="a55a4-128">description</span></span>|<span data-ttu-id="a55a4-129">String</span><span class="sxs-lookup"><span data-stu-id="a55a4-129">String</span></span>|<span data-ttu-id="a55a4-130">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="a55a4-130">Description for the policy.</span></span>|
|<span data-ttu-id="a55a4-131">displayName</span><span class="sxs-lookup"><span data-stu-id="a55a4-131">displayName</span></span>|<span data-ttu-id="a55a4-132">String</span><span class="sxs-lookup"><span data-stu-id="a55a4-132">String</span></span>|<span data-ttu-id="a55a4-133">策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a55a4-133">Display name for the policy.</span></span>|
|<span data-ttu-id="a55a4-134">id</span><span class="sxs-lookup"><span data-stu-id="a55a4-134">id</span></span>|<span data-ttu-id="a55a4-135">String</span><span class="sxs-lookup"><span data-stu-id="a55a4-135">String</span></span>|<span data-ttu-id="a55a4-136">策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a55a4-136">Unique identifier for the policy.</span></span>|
|<span data-ttu-id="a55a4-137">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="a55a4-137">isOrganizationDefault</span></span>|<span data-ttu-id="a55a4-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="a55a4-138">Boolean</span></span>|<span data-ttu-id="a55a4-139">对于将适用于所有作用域和角色的单个租户范围策略，这只能设置为 true。</span><span class="sxs-lookup"><span data-stu-id="a55a4-139">This can only be set to true for a single tenant wide policy which will apply to all scopes and roles.</span></span> <span data-ttu-id="a55a4-140">将 scopeId 设置为"/"，将 scopeType 设置为 Directory。</span><span class="sxs-lookup"><span data-stu-id="a55a4-140">Set the scopeId to "/" and scopeType to Directory.</span></span>|
|<span data-ttu-id="a55a4-141">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a55a4-141">lastModifiedBy</span></span>|[<span data-ttu-id="a55a4-142">identity</span><span class="sxs-lookup"><span data-stu-id="a55a4-142">identity</span></span>](../resources/identity.md)|<span data-ttu-id="a55a4-143">上次修改角色设置的标识。</span><span class="sxs-lookup"><span data-stu-id="a55a4-143">The identity who last modified the role setting.</span></span>|
|<span data-ttu-id="a55a4-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a55a4-144">lastModifiedDateTime</span></span>|<span data-ttu-id="a55a4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a55a4-145">DateTimeOffset</span></span>|<span data-ttu-id="a55a4-146">上次修改角色设置的时间。</span><span class="sxs-lookup"><span data-stu-id="a55a4-146">The time when the role setting was last modified.</span></span>|
|<span data-ttu-id="a55a4-147">scopeId</span><span class="sxs-lookup"><span data-stu-id="a55a4-147">scopeId</span></span>|<span data-ttu-id="a55a4-148">String</span><span class="sxs-lookup"><span data-stu-id="a55a4-148">String</span></span>|<span data-ttu-id="a55a4-149">创建策略的范围的 ID。</span><span class="sxs-lookup"><span data-stu-id="a55a4-149">The id of the scope where the policy is created.</span></span> <span data-ttu-id="a55a4-150">例如，</span><span class="sxs-lookup"><span data-stu-id="a55a4-150">E.g.</span></span> <span data-ttu-id="a55a4-151">"/"、groupId 等。</span><span class="sxs-lookup"><span data-stu-id="a55a4-151">"/", groupId, etc.</span></span>|
|<span data-ttu-id="a55a4-152">scopeType</span><span class="sxs-lookup"><span data-stu-id="a55a4-152">scopeType</span></span>|<span data-ttu-id="a55a4-153">String</span><span class="sxs-lookup"><span data-stu-id="a55a4-153">String</span></span>|<span data-ttu-id="a55a4-154">创建策略的范围类型。</span><span class="sxs-lookup"><span data-stu-id="a55a4-154">The type of the scope where the policy is created.</span></span> <span data-ttu-id="a55a4-155">Directory、DirectoryRole、Group 之一。</span><span class="sxs-lookup"><span data-stu-id="a55a4-155">One of Directory, DirectoryRole, Group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a55a4-156">关系</span><span class="sxs-lookup"><span data-stu-id="a55a4-156">Relationships</span></span>
|<span data-ttu-id="a55a4-157">关系</span><span class="sxs-lookup"><span data-stu-id="a55a4-157">Relationship</span></span>|<span data-ttu-id="a55a4-158">类型</span><span class="sxs-lookup"><span data-stu-id="a55a4-158">Type</span></span>|<span data-ttu-id="a55a4-159">说明</span><span class="sxs-lookup"><span data-stu-id="a55a4-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a55a4-160">effectiveRules</span><span class="sxs-lookup"><span data-stu-id="a55a4-160">effectiveRules</span></span>|<span data-ttu-id="a55a4-161">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a55a4-161">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="a55a4-162">根据继承的引用规则评估的有效规则（如审批规则、过期规则等）的列表。</span><span class="sxs-lookup"><span data-stu-id="a55a4-162">The list of effective rules like approval rule, expiration rule, etc. evaluated based on inherited referenced rules.</span></span> <span data-ttu-id="a55a4-163">例如，</span><span class="sxs-lookup"><span data-stu-id="a55a4-163">E.g.</span></span> <span data-ttu-id="a55a4-164">如果存在用于强制执行启用审批规则的租户范围策略，则有效规则将为启用审批，即使该 polcy 具有禁用审批的规则。</span><span class="sxs-lookup"><span data-stu-id="a55a4-164">If there is a tenant wide policy to enforce enabling approval rule, the effective rule will be to enable approval even if the polcy has a rule to disable approval.</span></span>|
|<span data-ttu-id="a55a4-165">规则</span><span class="sxs-lookup"><span data-stu-id="a55a4-165">rules</span></span>|<span data-ttu-id="a55a4-166">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a55a4-166">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="a55a4-167">审批规则、过期规则等规则的集合。</span><span class="sxs-lookup"><span data-stu-id="a55a4-167">The collection of rules like approval rule, expiration rule, etc.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a55a4-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a55a4-168">JSON representation</span></span>
<span data-ttu-id="a55a4-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a55a4-169">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isOrganizationDefault": "Boolean",
  "scopeId": "String",
  "scopeType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

