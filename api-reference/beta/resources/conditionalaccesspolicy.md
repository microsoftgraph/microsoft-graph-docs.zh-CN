---
title: conditionalAccessPolicy 资源类型
description: 表示 Azure Active Directory 条件访问策略。 条件访问策略是定义访问方案的自定义规则。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a1ec10d2a64017eac4894d947b5da20802a38c96
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444306"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="6a4c2-104">conditionalAccessPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a4c2-104">conditionalAccessPolicy resource type</span></span>

<span data-ttu-id="6a4c2-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a4c2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a4c2-106">表示 Azure Active Directory 条件访问策略。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-106">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="6a4c2-107">条件访问策略是定义访问方案的自定义规则。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-107">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="6a4c2-108">有关详细信息，请参阅条件 [访问文档](/azure/active-directory/conditional-access/)。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-108">For more information, see the [Conditional access documentation](/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="6a4c2-109">Methods</span><span class="sxs-lookup"><span data-stu-id="6a4c2-109">Methods</span></span>

| <span data-ttu-id="6a4c2-110">方法</span><span class="sxs-lookup"><span data-stu-id="6a4c2-110">Method</span></span>       | <span data-ttu-id="6a4c2-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="6a4c2-111">Return Type</span></span> | <span data-ttu-id="6a4c2-112">说明</span><span class="sxs-lookup"><span data-stu-id="6a4c2-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6a4c2-113">列出 conditionalAccessPolicies</span><span class="sxs-lookup"><span data-stu-id="6a4c2-113">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="6a4c2-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6a4c2-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="6a4c2-115">获取组织的所有 conditionalAccessPolicies 对象。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-115">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="6a4c2-116">创建 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="6a4c2-116">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="6a4c2-117">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="6a4c2-117">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="6a4c2-118">创建新的 conditionalAccessPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-118">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="6a4c2-119">获取 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="6a4c2-119">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="6a4c2-120">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="6a4c2-120">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="6a4c2-121">读取 conditionalAccessPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-121">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="6a4c2-122">更新 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="6a4c2-122">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="6a4c2-123">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="6a4c2-123">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="6a4c2-124">更新 conditionalAccessPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-124">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="6a4c2-125">删除 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="6a4c2-125">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="6a4c2-126">无</span><span class="sxs-lookup"><span data-stu-id="6a4c2-126">None</span></span> | <span data-ttu-id="6a4c2-127">删除 conditionalAccessPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-127">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6a4c2-128">属性</span><span class="sxs-lookup"><span data-stu-id="6a4c2-128">Properties</span></span>

| <span data-ttu-id="6a4c2-129">属性</span><span class="sxs-lookup"><span data-stu-id="6a4c2-129">Property</span></span>     | <span data-ttu-id="6a4c2-130">类型</span><span class="sxs-lookup"><span data-stu-id="6a4c2-130">Type</span></span>        | <span data-ttu-id="6a4c2-131">说明</span><span class="sxs-lookup"><span data-stu-id="6a4c2-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6a4c2-132">conditions</span><span class="sxs-lookup"><span data-stu-id="6a4c2-132">conditions</span></span>|[<span data-ttu-id="6a4c2-133">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="6a4c2-133">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="6a4c2-134">指定应用策略时必须满足的规则。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-134">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="6a4c2-135">必需。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-135">Required.</span></span> |
|<span data-ttu-id="6a4c2-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a4c2-136">createdDateTime</span></span>|<span data-ttu-id="6a4c2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a4c2-137">DateTimeOffset</span></span>| <span data-ttu-id="6a4c2-138">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6a4c2-139">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="6a4c2-140">只读。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-140">Readonly.</span></span> |
|<span data-ttu-id="6a4c2-141">说明</span><span class="sxs-lookup"><span data-stu-id="6a4c2-141">description</span></span>|<span data-ttu-id="6a4c2-142">String</span><span class="sxs-lookup"><span data-stu-id="6a4c2-142">String</span></span>| <span data-ttu-id="6a4c2-143">未使用。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-143">Not used.</span></span> |
|<span data-ttu-id="6a4c2-144">displayName</span><span class="sxs-lookup"><span data-stu-id="6a4c2-144">displayName</span></span>|<span data-ttu-id="6a4c2-145">String</span><span class="sxs-lookup"><span data-stu-id="6a4c2-145">String</span></span>| <span data-ttu-id="6a4c2-146">指定显示名称AccessPolicy 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-146">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="6a4c2-147">grantControls</span><span class="sxs-lookup"><span data-stu-id="6a4c2-147">grantControls</span></span>|[<span data-ttu-id="6a4c2-148">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="6a4c2-148">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="6a4c2-149">指定传递策略必须实现的授予控制。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-149">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="6a4c2-150">id</span><span class="sxs-lookup"><span data-stu-id="6a4c2-150">id</span></span>|<span data-ttu-id="6a4c2-151">String</span><span class="sxs-lookup"><span data-stu-id="6a4c2-151">String</span></span>| <span data-ttu-id="6a4c2-152">指定 conditionalAccessPolicy 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-152">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="6a4c2-153">只读。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-153">Read-only.</span></span>|
|<span data-ttu-id="6a4c2-154">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a4c2-154">modifiedDateTime</span></span>| <span data-ttu-id="6a4c2-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a4c2-155">DateTimeOffset</span></span>|<span data-ttu-id="6a4c2-156">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6a4c2-157">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="6a4c2-158">只读。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-158">Readonly.</span></span> |
|<span data-ttu-id="6a4c2-159">sessionControls</span><span class="sxs-lookup"><span data-stu-id="6a4c2-159">sessionControls</span></span>|[<span data-ttu-id="6a4c2-160">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="6a4c2-160">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="6a4c2-161">指定登录后强制执行的会话控件。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-161">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="6a4c2-162">state</span><span class="sxs-lookup"><span data-stu-id="6a4c2-162">state</span></span>|<span data-ttu-id="6a4c2-163">string</span><span class="sxs-lookup"><span data-stu-id="6a4c2-163">string</span></span>| <span data-ttu-id="6a4c2-164">指定 conditionalAccessPolicy 对象的状态。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-164">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="6a4c2-165">可取值为：`enabled`、`disabled`、`enabledForReportingButNotEnforced`。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-165">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="6a4c2-166">必填。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-166">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6a4c2-167">关系</span><span class="sxs-lookup"><span data-stu-id="6a4c2-167">Relationships</span></span>

<span data-ttu-id="6a4c2-168">无。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a4c2-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a4c2-169">JSON representation</span></span>

<span data-ttu-id="6a4c2-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-170">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "description",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy",
  "keyProperty": "id"
}-->

```json
{
  "conditions": {"@odata.type": "microsoft.graph.conditionalAccessConditionSet"},
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "grantControls": {"@odata.type": "microsoft.graph.conditionalAccessGrantControls"},
  "id": "String (identifier)",
  "modifiedDateTime": "String (timestamp)",
  "sessionControls": {"@odata.type": "microsoft.graph.conditionalAccessSessionControls"},
  "state": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
