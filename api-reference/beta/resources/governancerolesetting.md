---
title: governanceRoleSetting 资源类型
description: " 规则，依此类推。"
localization_priority: Normal
ms.openlocfilehash: a52769d4714608df11bdde826ca37907d7942e4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508165"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="7e64a-103">governanceRoleSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e64a-103">governanceRoleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e64a-104">代表一组在需要时创建或修改角色分配评估针对每个角色定义的配置。</span><span class="sxs-lookup"><span data-stu-id="7e64a-104">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="7e64a-105">例如，角色设置可能包括"最大工作分配持续时间"规则"MFA 上激活需要"规则，以及等。</span><span class="sxs-lookup"><span data-stu-id="7e64a-105">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="7e64a-106">方法</span><span class="sxs-lookup"><span data-stu-id="7e64a-106">Methods</span></span>

| <span data-ttu-id="7e64a-107">方法</span><span class="sxs-lookup"><span data-stu-id="7e64a-107">Method</span></span>          | <span data-ttu-id="7e64a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="7e64a-108">Return Type</span></span> |<span data-ttu-id="7e64a-109">说明</span><span class="sxs-lookup"><span data-stu-id="7e64a-109">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="7e64a-110">List</span><span class="sxs-lookup"><span data-stu-id="7e64a-110">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="7e64a-111">[governanceRoleSetting](../resources/governancerolesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="7e64a-111">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="7e64a-112">列出角色设置对资源的集合。</span><span class="sxs-lookup"><span data-stu-id="7e64a-112">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="7e64a-113">Get</span><span class="sxs-lookup"><span data-stu-id="7e64a-113">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="7e64a-114">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="7e64a-114">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="7e64a-115">读取属性和角色设置的关系。</span><span class="sxs-lookup"><span data-stu-id="7e64a-115">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="7e64a-116">Update</span><span class="sxs-lookup"><span data-stu-id="7e64a-116">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="7e64a-117">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="7e64a-117">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="7e64a-118">更新角色设置对象。</span><span class="sxs-lookup"><span data-stu-id="7e64a-118">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7e64a-119">属性</span><span class="sxs-lookup"><span data-stu-id="7e64a-119">Properties</span></span>
|<span data-ttu-id="7e64a-120">属性</span><span class="sxs-lookup"><span data-stu-id="7e64a-120">Property</span></span>               |<span data-ttu-id="7e64a-121">类型</span><span class="sxs-lookup"><span data-stu-id="7e64a-121">Type</span></span>                                      |<span data-ttu-id="7e64a-122">说明</span><span class="sxs-lookup"><span data-stu-id="7e64a-122">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="7e64a-123">id</span><span class="sxs-lookup"><span data-stu-id="7e64a-123">id</span></span>                   |<span data-ttu-id="7e64a-124">String</span><span class="sxs-lookup"><span data-stu-id="7e64a-124">String</span></span>                                  |<span data-ttu-id="7e64a-125">RoleSetting 的 id。</span><span class="sxs-lookup"><span data-stu-id="7e64a-125">The id of the roleSetting.</span></span>|
|<span data-ttu-id="7e64a-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="7e64a-126">resourceId</span></span>           |<span data-ttu-id="7e64a-127">String</span><span class="sxs-lookup"><span data-stu-id="7e64a-127">String</span></span>                                  |<span data-ttu-id="7e64a-128">必需。</span><span class="sxs-lookup"><span data-stu-id="7e64a-128">Required.</span></span> <span data-ttu-id="7e64a-129">与关联的角色设置资源的 id。</span><span class="sxs-lookup"><span data-stu-id="7e64a-129">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="7e64a-130">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7e64a-130">roleDefinitionId</span></span>     |<span data-ttu-id="7e64a-131">String</span><span class="sxs-lookup"><span data-stu-id="7e64a-131">String</span></span>                                  |<span data-ttu-id="7e64a-132">必需。</span><span class="sxs-lookup"><span data-stu-id="7e64a-132">Required.</span></span> <span data-ttu-id="7e64a-133">角色设置相关联的角色定义 id。</span><span class="sxs-lookup"><span data-stu-id="7e64a-133">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="7e64a-134">isDefault</span><span class="sxs-lookup"><span data-stu-id="7e64a-134">isDefault</span></span>            |<span data-ttu-id="7e64a-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e64a-135">Boolean</span></span>                                 |<span data-ttu-id="7e64a-136">只读。</span><span class="sxs-lookup"><span data-stu-id="7e64a-136">Read-only.</span></span> <span data-ttu-id="7e64a-137">指示 roleSetting 是否是默认 roleSetting</span><span class="sxs-lookup"><span data-stu-id="7e64a-137">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="7e64a-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e64a-138">lastUpdatedDateTime</span></span>  |<span data-ttu-id="7e64a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e64a-139">DateTimeOffset</span></span>                          |<span data-ttu-id="7e64a-140">只读。</span><span class="sxs-lookup"><span data-stu-id="7e64a-140">Read-only.</span></span> <span data-ttu-id="7e64a-141">上次更新时间角色设置的时间。</span><span class="sxs-lookup"><span data-stu-id="7e64a-141">The time when the role setting was last updated.</span></span> <span data-ttu-id="7e64a-142">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="7e64a-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7e64a-143">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7e64a-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7e64a-144">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="7e64a-144">lastUpdatedBy</span></span>        |<span data-ttu-id="7e64a-145">String</span><span class="sxs-lookup"><span data-stu-id="7e64a-145">String</span></span>                                  |<span data-ttu-id="7e64a-146">只读。</span><span class="sxs-lookup"><span data-stu-id="7e64a-146">Read-only.</span></span> <span data-ttu-id="7e64a-147">显示上次更新时间 roleSetting 的管理员名称。</span><span class="sxs-lookup"><span data-stu-id="7e64a-147">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="7e64a-148">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="7e64a-148">adminEligibleSettings</span></span>|<span data-ttu-id="7e64a-149">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="7e64a-149">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="7e64a-150">管理员尝试添加合格的角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="7e64a-150">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="7e64a-151">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="7e64a-151">adminMemberSettings</span></span>  |<span data-ttu-id="7e64a-152">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="7e64a-152">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="7e64a-153">管理员尝试添加直接成员角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="7e64a-153">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="7e64a-154">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="7e64a-154">userEligibleSettings</span></span> |<span data-ttu-id="7e64a-155">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="7e64a-155">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="7e64a-156">当用户尝试添加合格的角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="7e64a-156">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="7e64a-157">此时不支持的设置。</span><span class="sxs-lookup"><span data-stu-id="7e64a-157">The setting is not supported for now.</span></span>|
|<span data-ttu-id="7e64a-158">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="7e64a-158">userMemberSettings</span></span>   |<span data-ttu-id="7e64a-159">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="7e64a-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="7e64a-160">当用户尝试激活其角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="7e64a-160">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e64a-161">关系</span><span class="sxs-lookup"><span data-stu-id="7e64a-161">Relationships</span></span>
| <span data-ttu-id="7e64a-162">关系</span><span class="sxs-lookup"><span data-stu-id="7e64a-162">Relationship</span></span> | <span data-ttu-id="7e64a-163">类型</span><span class="sxs-lookup"><span data-stu-id="7e64a-163">Type</span></span>   |<span data-ttu-id="7e64a-164">说明</span><span class="sxs-lookup"><span data-stu-id="7e64a-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e64a-165">资源</span><span class="sxs-lookup"><span data-stu-id="7e64a-165">resource</span></span>|[<span data-ttu-id="7e64a-166">governanceResource</span><span class="sxs-lookup"><span data-stu-id="7e64a-166">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="7e64a-167">只读。</span><span class="sxs-lookup"><span data-stu-id="7e64a-167">Read-only.</span></span> <span data-ttu-id="7e64a-168">此角色设置关联的资源。</span><span class="sxs-lookup"><span data-stu-id="7e64a-168">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="7e64a-169">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7e64a-169">roleDefinition</span></span>|[<span data-ttu-id="7e64a-170">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7e64a-170">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="7e64a-171">只读。</span><span class="sxs-lookup"><span data-stu-id="7e64a-171">Read-only.</span></span> <span data-ttu-id="7e64a-172">角色定义的强制执行与此角色设置。</span><span class="sxs-lookup"><span data-stu-id="7e64a-172">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7e64a-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e64a-173">JSON representation</span></span>

<span data-ttu-id="7e64a-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e64a-174">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerolesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
