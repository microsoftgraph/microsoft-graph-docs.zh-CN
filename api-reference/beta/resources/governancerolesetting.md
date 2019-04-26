---
title: governanceRoleSetting 资源类型
description: " 规则等。"
localization_priority: Normal
ms.openlocfilehash: 09e8cb65f8318294d483a2ad66a7119d7b48822a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340216"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="97d38-103">governanceRoleSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="97d38-103">governanceRoleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97d38-104">表示在创建或修改角色分配时需要评估的每个角色定义上的一组配置。</span><span class="sxs-lookup"><span data-stu-id="97d38-104">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="97d38-105">例如, 角色设置可能包括 "最大分配持续时间" 规则、"激活时需要 MFA" 规则等。</span><span class="sxs-lookup"><span data-stu-id="97d38-105">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="97d38-106">方法</span><span class="sxs-lookup"><span data-stu-id="97d38-106">Methods</span></span>

| <span data-ttu-id="97d38-107">方法</span><span class="sxs-lookup"><span data-stu-id="97d38-107">Method</span></span>          | <span data-ttu-id="97d38-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="97d38-108">Return Type</span></span> |<span data-ttu-id="97d38-109">说明</span><span class="sxs-lookup"><span data-stu-id="97d38-109">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="97d38-110">List</span><span class="sxs-lookup"><span data-stu-id="97d38-110">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="97d38-111">[governanceRoleSetting](../resources/governancerolesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="97d38-111">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="97d38-112">列出资源的角色设置的集合。</span><span class="sxs-lookup"><span data-stu-id="97d38-112">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="97d38-113">Get</span><span class="sxs-lookup"><span data-stu-id="97d38-113">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="97d38-114">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="97d38-114">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="97d38-115">读取角色设置的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="97d38-115">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="97d38-116">更新</span><span class="sxs-lookup"><span data-stu-id="97d38-116">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="97d38-117">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="97d38-117">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="97d38-118">更新角色设置对象。</span><span class="sxs-lookup"><span data-stu-id="97d38-118">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="97d38-119">属性</span><span class="sxs-lookup"><span data-stu-id="97d38-119">Properties</span></span>
|<span data-ttu-id="97d38-120">属性</span><span class="sxs-lookup"><span data-stu-id="97d38-120">Property</span></span>               |<span data-ttu-id="97d38-121">类型</span><span class="sxs-lookup"><span data-stu-id="97d38-121">Type</span></span>                                      |<span data-ttu-id="97d38-122">说明</span><span class="sxs-lookup"><span data-stu-id="97d38-122">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="97d38-123">id</span><span class="sxs-lookup"><span data-stu-id="97d38-123">id</span></span>                   |<span data-ttu-id="97d38-124">字符串</span><span class="sxs-lookup"><span data-stu-id="97d38-124">String</span></span>                                  |<span data-ttu-id="97d38-125">roleSetting 的 id。</span><span class="sxs-lookup"><span data-stu-id="97d38-125">The id of the roleSetting.</span></span>|
|<span data-ttu-id="97d38-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="97d38-126">resourceId</span></span>           |<span data-ttu-id="97d38-127">String</span><span class="sxs-lookup"><span data-stu-id="97d38-127">String</span></span>                                  |<span data-ttu-id="97d38-128">必需。</span><span class="sxs-lookup"><span data-stu-id="97d38-128">Required.</span></span> <span data-ttu-id="97d38-129">与角色设置相关联的资源的 id。</span><span class="sxs-lookup"><span data-stu-id="97d38-129">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="97d38-130">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="97d38-130">roleDefinitionId</span></span>     |<span data-ttu-id="97d38-131">String</span><span class="sxs-lookup"><span data-stu-id="97d38-131">String</span></span>                                  |<span data-ttu-id="97d38-132">必需。</span><span class="sxs-lookup"><span data-stu-id="97d38-132">Required.</span></span> <span data-ttu-id="97d38-133">与角色设置相关联的角色定义的 id。</span><span class="sxs-lookup"><span data-stu-id="97d38-133">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="97d38-134">isDefault</span><span class="sxs-lookup"><span data-stu-id="97d38-134">isDefault</span></span>            |<span data-ttu-id="97d38-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="97d38-135">Boolean</span></span>                                 |<span data-ttu-id="97d38-136">只读。</span><span class="sxs-lookup"><span data-stu-id="97d38-136">Read-only.</span></span> <span data-ttu-id="97d38-137">指示 roleSetting 是否为默认 roleSetting</span><span class="sxs-lookup"><span data-stu-id="97d38-137">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="97d38-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="97d38-138">lastUpdatedDateTime</span></span>  |<span data-ttu-id="97d38-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97d38-139">DateTimeOffset</span></span>                          |<span data-ttu-id="97d38-140">只读。</span><span class="sxs-lookup"><span data-stu-id="97d38-140">Read-only.</span></span> <span data-ttu-id="97d38-141">上次更新角色设置的时间。</span><span class="sxs-lookup"><span data-stu-id="97d38-141">The time when the role setting was last updated.</span></span> <span data-ttu-id="97d38-142">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="97d38-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97d38-143">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="97d38-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="97d38-144">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="97d38-144">lastUpdatedBy</span></span>        |<span data-ttu-id="97d38-145">String</span><span class="sxs-lookup"><span data-stu-id="97d38-145">String</span></span>                                  |<span data-ttu-id="97d38-146">只读。</span><span class="sxs-lookup"><span data-stu-id="97d38-146">Read-only.</span></span> <span data-ttu-id="97d38-147">上次更新 roleSetting 的管理员的显示名称。</span><span class="sxs-lookup"><span data-stu-id="97d38-147">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="97d38-148">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="97d38-148">adminEligibleSettings</span></span>|<span data-ttu-id="97d38-149">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="97d38-149">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="97d38-150">在管理员尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="97d38-150">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="97d38-151">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="97d38-151">adminMemberSettings</span></span>  |<span data-ttu-id="97d38-152">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="97d38-152">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="97d38-153">在管理员尝试添加直接成员角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="97d38-153">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="97d38-154">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="97d38-154">userEligibleSettings</span></span> |<span data-ttu-id="97d38-155">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="97d38-155">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="97d38-156">用户尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="97d38-156">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="97d38-157">目前不支持该设置。</span><span class="sxs-lookup"><span data-stu-id="97d38-157">The setting is not supported for now.</span></span>|
|<span data-ttu-id="97d38-158">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="97d38-158">userMemberSettings</span></span>   |<span data-ttu-id="97d38-159">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="97d38-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="97d38-160">用户尝试激活他的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="97d38-160">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97d38-161">关系</span><span class="sxs-lookup"><span data-stu-id="97d38-161">Relationships</span></span>
| <span data-ttu-id="97d38-162">关系</span><span class="sxs-lookup"><span data-stu-id="97d38-162">Relationship</span></span> | <span data-ttu-id="97d38-163">类型</span><span class="sxs-lookup"><span data-stu-id="97d38-163">Type</span></span>   |<span data-ttu-id="97d38-164">说明</span><span class="sxs-lookup"><span data-stu-id="97d38-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97d38-165">资源</span><span class="sxs-lookup"><span data-stu-id="97d38-165">resource</span></span>|[<span data-ttu-id="97d38-166">governanceResource</span><span class="sxs-lookup"><span data-stu-id="97d38-166">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="97d38-167">只读。</span><span class="sxs-lookup"><span data-stu-id="97d38-167">Read-only.</span></span> <span data-ttu-id="97d38-168">此角色设置的关联资源。</span><span class="sxs-lookup"><span data-stu-id="97d38-168">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="97d38-169">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="97d38-169">roleDefinition</span></span>|[<span data-ttu-id="97d38-170">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="97d38-170">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="97d38-171">只读。</span><span class="sxs-lookup"><span data-stu-id="97d38-171">Read-only.</span></span> <span data-ttu-id="97d38-172">使用此角色设置强制实施的角色定义。</span><span class="sxs-lookup"><span data-stu-id="97d38-172">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="97d38-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97d38-173">JSON representation</span></span>

<span data-ttu-id="97d38-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97d38-174">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleSetting"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": true,
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "adminMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
