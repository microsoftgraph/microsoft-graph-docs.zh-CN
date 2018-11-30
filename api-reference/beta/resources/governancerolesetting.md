---
title: governanceRoleSetting 资源类型
description: " 规则，依此类推。"
ms.openlocfilehash: 64245b2d6f0aa9e0ea3ffda4a5eaebfb9fd205df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045763"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="ecb75-103">governanceRoleSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="ecb75-103">governanceRoleSetting resource type</span></span>

> <span data-ttu-id="ecb75-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ecb75-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecb75-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ecb75-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ecb75-106">代表一组在需要时创建或修改角色分配评估针对每个角色定义的配置。</span><span class="sxs-lookup"><span data-stu-id="ecb75-106">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="ecb75-107">例如，角色设置可能包括"最大工作分配持续时间"规则"MFA 上激活需要"规则，以及等。</span><span class="sxs-lookup"><span data-stu-id="ecb75-107">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="ecb75-108">方法</span><span class="sxs-lookup"><span data-stu-id="ecb75-108">Methods</span></span>

| <span data-ttu-id="ecb75-109">方法</span><span class="sxs-lookup"><span data-stu-id="ecb75-109">Method</span></span>          | <span data-ttu-id="ecb75-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ecb75-110">Return Type</span></span> |<span data-ttu-id="ecb75-111">说明</span><span class="sxs-lookup"><span data-stu-id="ecb75-111">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="ecb75-112">List</span><span class="sxs-lookup"><span data-stu-id="ecb75-112">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="ecb75-113">[governanceRoleSetting](../resources/governancerolesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="ecb75-113">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="ecb75-114">列出角色设置对资源的集合。</span><span class="sxs-lookup"><span data-stu-id="ecb75-114">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="ecb75-115">Get</span><span class="sxs-lookup"><span data-stu-id="ecb75-115">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="ecb75-116">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="ecb75-116">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="ecb75-117">读取属性和角色设置的关系。</span><span class="sxs-lookup"><span data-stu-id="ecb75-117">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="ecb75-118">Update</span><span class="sxs-lookup"><span data-stu-id="ecb75-118">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="ecb75-119">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="ecb75-119">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="ecb75-120">更新角色设置对象。</span><span class="sxs-lookup"><span data-stu-id="ecb75-120">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ecb75-121">属性</span><span class="sxs-lookup"><span data-stu-id="ecb75-121">Properties</span></span>
|<span data-ttu-id="ecb75-122">属性</span><span class="sxs-lookup"><span data-stu-id="ecb75-122">Property</span></span>               |<span data-ttu-id="ecb75-123">类型</span><span class="sxs-lookup"><span data-stu-id="ecb75-123">Type</span></span>                                      |<span data-ttu-id="ecb75-124">说明</span><span class="sxs-lookup"><span data-stu-id="ecb75-124">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="ecb75-125">id</span><span class="sxs-lookup"><span data-stu-id="ecb75-125">id</span></span>                   |<span data-ttu-id="ecb75-126">字符串</span><span class="sxs-lookup"><span data-stu-id="ecb75-126">String</span></span>                                  |<span data-ttu-id="ecb75-127">RoleSetting 的 id。</span><span class="sxs-lookup"><span data-stu-id="ecb75-127">The id of the roleSetting.</span></span>|
|<span data-ttu-id="ecb75-128">resourceId</span><span class="sxs-lookup"><span data-stu-id="ecb75-128">resourceId</span></span>           |<span data-ttu-id="ecb75-129">String</span><span class="sxs-lookup"><span data-stu-id="ecb75-129">String</span></span>                                  |<span data-ttu-id="ecb75-130">必需项。</span><span class="sxs-lookup"><span data-stu-id="ecb75-130">Required.</span></span> <span data-ttu-id="ecb75-131">与关联的角色设置资源的 id。</span><span class="sxs-lookup"><span data-stu-id="ecb75-131">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="ecb75-132">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ecb75-132">roleDefinitionId</span></span>     |<span data-ttu-id="ecb75-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ecb75-133">String</span></span>                                  |<span data-ttu-id="ecb75-134">必需项。</span><span class="sxs-lookup"><span data-stu-id="ecb75-134">Required.</span></span> <span data-ttu-id="ecb75-135">角色设置相关联的角色定义 id。</span><span class="sxs-lookup"><span data-stu-id="ecb75-135">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="ecb75-136">isDefault</span><span class="sxs-lookup"><span data-stu-id="ecb75-136">isDefault</span></span>            |<span data-ttu-id="ecb75-137">布尔</span><span class="sxs-lookup"><span data-stu-id="ecb75-137">Boolean</span></span>                                 |<span data-ttu-id="ecb75-138">只读。</span><span class="sxs-lookup"><span data-stu-id="ecb75-138">Read-only.</span></span> <span data-ttu-id="ecb75-139">指示 roleSetting 是否是默认 roleSetting</span><span class="sxs-lookup"><span data-stu-id="ecb75-139">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="ecb75-140">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ecb75-140">lastUpdatedDateTime</span></span>  |<span data-ttu-id="ecb75-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecb75-141">DateTimeOffset</span></span>                          |<span data-ttu-id="ecb75-142">只读。</span><span class="sxs-lookup"><span data-stu-id="ecb75-142">Read-only.</span></span> <span data-ttu-id="ecb75-143">上次更新时间角色设置的时间。</span><span class="sxs-lookup"><span data-stu-id="ecb75-143">The time when the role setting was last updated.</span></span> <span data-ttu-id="ecb75-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ecb75-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ecb75-145">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ecb75-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ecb75-146">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="ecb75-146">lastUpdatedBy</span></span>        |<span data-ttu-id="ecb75-147">String</span><span class="sxs-lookup"><span data-stu-id="ecb75-147">String</span></span>                                  |<span data-ttu-id="ecb75-148">只读。</span><span class="sxs-lookup"><span data-stu-id="ecb75-148">Read-only.</span></span> <span data-ttu-id="ecb75-149">显示上次更新时间 roleSetting 的管理员名称。</span><span class="sxs-lookup"><span data-stu-id="ecb75-149">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="ecb75-150">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="ecb75-150">adminEligibleSettings</span></span>|<span data-ttu-id="ecb75-151">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="ecb75-151">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="ecb75-152">管理员尝试添加合格的角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="ecb75-152">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="ecb75-153">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="ecb75-153">adminMemberSettings</span></span>  |<span data-ttu-id="ecb75-154">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="ecb75-154">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="ecb75-155">管理员尝试添加直接成员角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="ecb75-155">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="ecb75-156">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="ecb75-156">userEligibleSettings</span></span> |<span data-ttu-id="ecb75-157">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="ecb75-157">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="ecb75-158">当用户尝试添加合格的角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="ecb75-158">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="ecb75-159">此时不支持的设置。</span><span class="sxs-lookup"><span data-stu-id="ecb75-159">The setting is not supported for now.</span></span>|
|<span data-ttu-id="ecb75-160">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="ecb75-160">userMemberSettings</span></span>   |<span data-ttu-id="ecb75-161">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="ecb75-161">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="ecb75-162">当用户尝试激活其角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="ecb75-162">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecb75-163">Relationships</span><span class="sxs-lookup"><span data-stu-id="ecb75-163">Relationships</span></span>
| <span data-ttu-id="ecb75-164">关系</span><span class="sxs-lookup"><span data-stu-id="ecb75-164">Relationship</span></span> | <span data-ttu-id="ecb75-165">类型</span><span class="sxs-lookup"><span data-stu-id="ecb75-165">Type</span></span>   |<span data-ttu-id="ecb75-166">说明</span><span class="sxs-lookup"><span data-stu-id="ecb75-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecb75-167">资源</span><span class="sxs-lookup"><span data-stu-id="ecb75-167">resource</span></span>|[<span data-ttu-id="ecb75-168">governanceResource</span><span class="sxs-lookup"><span data-stu-id="ecb75-168">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="ecb75-169">只读。</span><span class="sxs-lookup"><span data-stu-id="ecb75-169">Read-only.</span></span> <span data-ttu-id="ecb75-170">此角色设置关联的资源。</span><span class="sxs-lookup"><span data-stu-id="ecb75-170">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="ecb75-171">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="ecb75-171">roleDefinition</span></span>|[<span data-ttu-id="ecb75-172">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ecb75-172">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="ecb75-173">只读。</span><span class="sxs-lookup"><span data-stu-id="ecb75-173">Read-only.</span></span> <span data-ttu-id="ecb75-174">角色定义的强制执行与此角色设置。</span><span class="sxs-lookup"><span data-stu-id="ecb75-174">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ecb75-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ecb75-175">JSON representation</span></span>

<span data-ttu-id="ecb75-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ecb75-176">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
