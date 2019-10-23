---
title: conditionalAccessPolicy 资源类型
description: 表示 Azure Active Directory 条件访问策略。 条件访问策略是定义访问方案的自定义规则。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8187e98d1ddc5a096dea469bea22681fd5df78e7
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637758"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="ffe54-104">conditionalAccessPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="ffe54-104">conditionalAccessPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffe54-105">表示 Azure Active Directory 条件访问策略。</span><span class="sxs-lookup"><span data-stu-id="ffe54-105">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="ffe54-106">条件访问策略是定义访问方案的自定义规则。</span><span class="sxs-lookup"><span data-stu-id="ffe54-106">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="ffe54-107">有关详细信息，请参阅[条件访问文档](https://docs.microsoft.com/azure/active-directory/conditional-access/)。</span><span class="sxs-lookup"><span data-stu-id="ffe54-107">For more information, see the [Conditional access documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="ffe54-108">方法</span><span class="sxs-lookup"><span data-stu-id="ffe54-108">Methods</span></span>

| <span data-ttu-id="ffe54-109">方法</span><span class="sxs-lookup"><span data-stu-id="ffe54-109">Method</span></span>       | <span data-ttu-id="ffe54-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ffe54-110">Return Type</span></span> | <span data-ttu-id="ffe54-111">说明</span><span class="sxs-lookup"><span data-stu-id="ffe54-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ffe54-112">列出 conditionalAccessPolicies</span><span class="sxs-lookup"><span data-stu-id="ffe54-112">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="ffe54-113">[conditionalAccessPolicy](conditionalaccesspolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ffe54-113">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="ffe54-114">获取组织中的所有 conditionalAccessPolicies 对象。</span><span class="sxs-lookup"><span data-stu-id="ffe54-114">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="ffe54-115">创建 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ffe54-115">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="ffe54-116">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ffe54-116">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="ffe54-117">创建新的 conditionalAccessPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="ffe54-117">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="ffe54-118">获取 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ffe54-118">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="ffe54-119">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ffe54-119">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="ffe54-120">读取 conditionalAccessPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ffe54-120">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="ffe54-121">更新 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ffe54-121">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="ffe54-122">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ffe54-122">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="ffe54-123">更新 conditionalAccessPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="ffe54-123">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="ffe54-124">删除 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ffe54-124">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="ffe54-125">无</span><span class="sxs-lookup"><span data-stu-id="ffe54-125">None</span></span> | <span data-ttu-id="ffe54-126">删除 conditionalAccessPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="ffe54-126">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ffe54-127">属性</span><span class="sxs-lookup"><span data-stu-id="ffe54-127">Properties</span></span>

| <span data-ttu-id="ffe54-128">属性</span><span class="sxs-lookup"><span data-stu-id="ffe54-128">Property</span></span>     | <span data-ttu-id="ffe54-129">类型</span><span class="sxs-lookup"><span data-stu-id="ffe54-129">Type</span></span>        | <span data-ttu-id="ffe54-130">说明</span><span class="sxs-lookup"><span data-stu-id="ffe54-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ffe54-131">conditions</span><span class="sxs-lookup"><span data-stu-id="ffe54-131">conditions</span></span>|[<span data-ttu-id="ffe54-132">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="ffe54-132">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="ffe54-133">指定应用策略必须满足的规则。</span><span class="sxs-lookup"><span data-stu-id="ffe54-133">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="ffe54-134">必需。</span><span class="sxs-lookup"><span data-stu-id="ffe54-134">Required.</span></span> |
|<span data-ttu-id="ffe54-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffe54-135">createdDateTime</span></span>|<span data-ttu-id="ffe54-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffe54-136">DateTimeOffset</span></span>| <span data-ttu-id="ffe54-137">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ffe54-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ffe54-138">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="ffe54-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="ffe54-139">只读.</span><span class="sxs-lookup"><span data-stu-id="ffe54-139">Readonly.</span></span> |
|<span data-ttu-id="ffe54-140">说明</span><span class="sxs-lookup"><span data-stu-id="ffe54-140">description</span></span>|<span data-ttu-id="ffe54-141">String</span><span class="sxs-lookup"><span data-stu-id="ffe54-141">String</span></span>| <span data-ttu-id="ffe54-142">未使用。</span><span class="sxs-lookup"><span data-stu-id="ffe54-142">Not used.</span></span> |
|<span data-ttu-id="ffe54-143">displayName</span><span class="sxs-lookup"><span data-stu-id="ffe54-143">displayName</span></span>|<span data-ttu-id="ffe54-144">String</span><span class="sxs-lookup"><span data-stu-id="ffe54-144">String</span></span>| <span data-ttu-id="ffe54-145">指定 conditionalAccessPolicy 对象的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ffe54-145">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="ffe54-146">grantControls</span><span class="sxs-lookup"><span data-stu-id="ffe54-146">grantControls</span></span>|[<span data-ttu-id="ffe54-147">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="ffe54-147">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="ffe54-148">指定必须满足的授予控制以通过策略。</span><span class="sxs-lookup"><span data-stu-id="ffe54-148">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="ffe54-149">id</span><span class="sxs-lookup"><span data-stu-id="ffe54-149">id</span></span>|<span data-ttu-id="ffe54-150">字符串</span><span class="sxs-lookup"><span data-stu-id="ffe54-150">String</span></span>| <span data-ttu-id="ffe54-151">指定 conditionalAccessPolicy 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="ffe54-151">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="ffe54-152">只读。</span><span class="sxs-lookup"><span data-stu-id="ffe54-152">Read-only.</span></span>|
|<span data-ttu-id="ffe54-153">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffe54-153">modifiedDateTime</span></span>| <span data-ttu-id="ffe54-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffe54-154">DateTimeOffset</span></span>|<span data-ttu-id="ffe54-155">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ffe54-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ffe54-156">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="ffe54-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="ffe54-157">只读.</span><span class="sxs-lookup"><span data-stu-id="ffe54-157">Readonly.</span></span> |
|<span data-ttu-id="ffe54-158">sessionControls</span><span class="sxs-lookup"><span data-stu-id="ffe54-158">sessionControls</span></span>|[<span data-ttu-id="ffe54-159">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="ffe54-159">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="ffe54-160">指定登录后强制实施的会话控制。</span><span class="sxs-lookup"><span data-stu-id="ffe54-160">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="ffe54-161">state</span><span class="sxs-lookup"><span data-stu-id="ffe54-161">state</span></span>|<span data-ttu-id="ffe54-162">string</span><span class="sxs-lookup"><span data-stu-id="ffe54-162">string</span></span>| <span data-ttu-id="ffe54-163">指定 conditionalAccessPolicy 对象的状态。</span><span class="sxs-lookup"><span data-stu-id="ffe54-163">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="ffe54-164">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="ffe54-164">Possible values are: `enabled`, `disabled`.</span></span> <span data-ttu-id="ffe54-165">必填。</span><span class="sxs-lookup"><span data-stu-id="ffe54-165">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ffe54-166">关系</span><span class="sxs-lookup"><span data-stu-id="ffe54-166">Relationships</span></span>

<span data-ttu-id="ffe54-167">无。</span><span class="sxs-lookup"><span data-stu-id="ffe54-167">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ffe54-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ffe54-168">JSON representation</span></span>

<span data-ttu-id="ffe54-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffe54-169">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "description",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy",
  "baseType": "",
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
