---
title: governanceRoleSetting 资源类型
description: " 规则等。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9cf027969fb6ae988fd3e57da9d6c3002a4b4da9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497326"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="96048-103">governanceRoleSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="96048-103">governanceRoleSetting resource type</span></span>

<span data-ttu-id="96048-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="96048-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96048-105">表示在创建或修改角色分配时需要评估的每个角色定义上的一组配置。</span><span class="sxs-lookup"><span data-stu-id="96048-105">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="96048-106">例如，角色设置可能包括 "最大分配持续时间" 规则、"激活时需要 MFA" 规则等。</span><span class="sxs-lookup"><span data-stu-id="96048-106">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="96048-107">方法</span><span class="sxs-lookup"><span data-stu-id="96048-107">Methods</span></span>

| <span data-ttu-id="96048-108">方法</span><span class="sxs-lookup"><span data-stu-id="96048-108">Method</span></span>          | <span data-ttu-id="96048-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="96048-109">Return Type</span></span> |<span data-ttu-id="96048-110">说明</span><span class="sxs-lookup"><span data-stu-id="96048-110">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="96048-111">List</span><span class="sxs-lookup"><span data-stu-id="96048-111">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="96048-112">[governanceRoleSetting](../resources/governancerolesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="96048-112">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="96048-113">列出资源的角色设置的集合。</span><span class="sxs-lookup"><span data-stu-id="96048-113">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="96048-114">获取</span><span class="sxs-lookup"><span data-stu-id="96048-114">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="96048-115">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="96048-115">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="96048-116">读取角色设置的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="96048-116">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="96048-117">更新</span><span class="sxs-lookup"><span data-stu-id="96048-117">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="96048-118">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="96048-118">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="96048-119">更新角色设置对象。</span><span class="sxs-lookup"><span data-stu-id="96048-119">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="96048-120">属性</span><span class="sxs-lookup"><span data-stu-id="96048-120">Properties</span></span>
|<span data-ttu-id="96048-121">属性</span><span class="sxs-lookup"><span data-stu-id="96048-121">Property</span></span>               |<span data-ttu-id="96048-122">类型</span><span class="sxs-lookup"><span data-stu-id="96048-122">Type</span></span>                                      |<span data-ttu-id="96048-123">说明</span><span class="sxs-lookup"><span data-stu-id="96048-123">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="96048-124">id</span><span class="sxs-lookup"><span data-stu-id="96048-124">id</span></span>                   |<span data-ttu-id="96048-125">字符串</span><span class="sxs-lookup"><span data-stu-id="96048-125">String</span></span>                                  |<span data-ttu-id="96048-126">RoleSetting 的 id。</span><span class="sxs-lookup"><span data-stu-id="96048-126">The id of the roleSetting.</span></span>|
|<span data-ttu-id="96048-127">resourceId</span><span class="sxs-lookup"><span data-stu-id="96048-127">resourceId</span></span>           |<span data-ttu-id="96048-128">String</span><span class="sxs-lookup"><span data-stu-id="96048-128">String</span></span>                                  |<span data-ttu-id="96048-129">必填。</span><span class="sxs-lookup"><span data-stu-id="96048-129">Required.</span></span> <span data-ttu-id="96048-130">与角色设置相关联的资源的 id。</span><span class="sxs-lookup"><span data-stu-id="96048-130">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="96048-131">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="96048-131">roleDefinitionId</span></span>     |<span data-ttu-id="96048-132">String</span><span class="sxs-lookup"><span data-stu-id="96048-132">String</span></span>                                  |<span data-ttu-id="96048-133">必填。</span><span class="sxs-lookup"><span data-stu-id="96048-133">Required.</span></span> <span data-ttu-id="96048-134">与角色设置相关联的角色定义的 id。</span><span class="sxs-lookup"><span data-stu-id="96048-134">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="96048-135">isDefault</span><span class="sxs-lookup"><span data-stu-id="96048-135">isDefault</span></span>            |<span data-ttu-id="96048-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="96048-136">Boolean</span></span>                                 |<span data-ttu-id="96048-137">只读。</span><span class="sxs-lookup"><span data-stu-id="96048-137">Read-only.</span></span> <span data-ttu-id="96048-138">指示 roleSetting 是否为默认 roleSetting</span><span class="sxs-lookup"><span data-stu-id="96048-138">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="96048-139">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="96048-139">lastUpdatedDateTime</span></span>  |<span data-ttu-id="96048-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96048-140">DateTimeOffset</span></span>                          |<span data-ttu-id="96048-141">只读。</span><span class="sxs-lookup"><span data-stu-id="96048-141">Read-only.</span></span> <span data-ttu-id="96048-142">上次更新角色设置的时间。</span><span class="sxs-lookup"><span data-stu-id="96048-142">The time when the role setting was last updated.</span></span> <span data-ttu-id="96048-143">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="96048-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="96048-144">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="96048-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="96048-145">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="96048-145">lastUpdatedBy</span></span>        |<span data-ttu-id="96048-146">字符串</span><span class="sxs-lookup"><span data-stu-id="96048-146">String</span></span>                                  |<span data-ttu-id="96048-147">只读。</span><span class="sxs-lookup"><span data-stu-id="96048-147">Read-only.</span></span> <span data-ttu-id="96048-148">上次更新 roleSetting 的管理员的显示名称。</span><span class="sxs-lookup"><span data-stu-id="96048-148">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="96048-149">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="96048-149">adminEligibleSettings</span></span>|<span data-ttu-id="96048-150">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="96048-150">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="96048-151">在管理员尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="96048-151">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="96048-152">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="96048-152">adminMemberSettings</span></span>  |<span data-ttu-id="96048-153">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="96048-153">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="96048-154">在管理员尝试添加直接成员角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="96048-154">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="96048-155">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="96048-155">userEligibleSettings</span></span> |<span data-ttu-id="96048-156">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="96048-156">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="96048-157">用户尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="96048-157">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="96048-158">目前不支持该设置。</span><span class="sxs-lookup"><span data-stu-id="96048-158">The setting is not supported for now.</span></span>|
|<span data-ttu-id="96048-159">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="96048-159">userMemberSettings</span></span>   |<span data-ttu-id="96048-160">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="96048-160">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="96048-161">用户尝试激活他的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="96048-161">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96048-162">关系</span><span class="sxs-lookup"><span data-stu-id="96048-162">Relationships</span></span>
| <span data-ttu-id="96048-163">关系</span><span class="sxs-lookup"><span data-stu-id="96048-163">Relationship</span></span> | <span data-ttu-id="96048-164">类型</span><span class="sxs-lookup"><span data-stu-id="96048-164">Type</span></span>   |<span data-ttu-id="96048-165">说明</span><span class="sxs-lookup"><span data-stu-id="96048-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96048-166">资源</span><span class="sxs-lookup"><span data-stu-id="96048-166">resource</span></span>|[<span data-ttu-id="96048-167">governanceResource</span><span class="sxs-lookup"><span data-stu-id="96048-167">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="96048-168">只读。</span><span class="sxs-lookup"><span data-stu-id="96048-168">Read-only.</span></span> <span data-ttu-id="96048-169">此角色设置的关联资源。</span><span class="sxs-lookup"><span data-stu-id="96048-169">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="96048-170">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="96048-170">roleDefinition</span></span>|[<span data-ttu-id="96048-171">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="96048-171">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="96048-172">只读。</span><span class="sxs-lookup"><span data-stu-id="96048-172">Read-only.</span></span> <span data-ttu-id="96048-173">使用此角色设置强制实施的角色定义。</span><span class="sxs-lookup"><span data-stu-id="96048-173">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="96048-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96048-174">JSON representation</span></span>

<span data-ttu-id="96048-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96048-175">Here is a JSON representation of the resource.</span></span>

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
