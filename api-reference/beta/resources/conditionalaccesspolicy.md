---
title: conditionalAccessPolicy 资源类型
description: 表示 Azure Active Directory 条件访问策略。 条件访问策略是定义访问方案的自定义规则。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 74270d2362bdfd6bbda567c17a45353eda7c319e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031732"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="892be-104">conditionalAccessPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="892be-104">conditionalAccessPolicy resource type</span></span>

<span data-ttu-id="892be-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="892be-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="892be-106">表示 Azure Active Directory 条件访问策略。</span><span class="sxs-lookup"><span data-stu-id="892be-106">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="892be-107">条件访问策略是定义访问方案的自定义规则。</span><span class="sxs-lookup"><span data-stu-id="892be-107">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="892be-108">有关详细信息，请参阅 [条件访问文档](https://docs.microsoft.com/azure/active-directory/conditional-access/)。</span><span class="sxs-lookup"><span data-stu-id="892be-108">For more information, see the [Conditional access documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="892be-109">方法</span><span class="sxs-lookup"><span data-stu-id="892be-109">Methods</span></span>

| <span data-ttu-id="892be-110">方法</span><span class="sxs-lookup"><span data-stu-id="892be-110">Method</span></span>       | <span data-ttu-id="892be-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="892be-111">Return Type</span></span> | <span data-ttu-id="892be-112">说明</span><span class="sxs-lookup"><span data-stu-id="892be-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="892be-113">列出 conditionalAccessPolicies</span><span class="sxs-lookup"><span data-stu-id="892be-113">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="892be-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="892be-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="892be-115">获取组织中的所有 conditionalAccessPolicies 对象。</span><span class="sxs-lookup"><span data-stu-id="892be-115">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="892be-116">创建 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="892be-116">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="892be-117">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="892be-117">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="892be-118">创建新的 conditionalAccessPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="892be-118">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="892be-119">获取 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="892be-119">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="892be-120">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="892be-120">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="892be-121">读取 conditionalAccessPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="892be-121">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="892be-122">更新 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="892be-122">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="892be-123">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="892be-123">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="892be-124">更新 conditionalAccessPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="892be-124">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="892be-125">删除 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="892be-125">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="892be-126">无</span><span class="sxs-lookup"><span data-stu-id="892be-126">None</span></span> | <span data-ttu-id="892be-127">删除 conditionalAccessPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="892be-127">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="892be-128">属性</span><span class="sxs-lookup"><span data-stu-id="892be-128">Properties</span></span>

| <span data-ttu-id="892be-129">属性</span><span class="sxs-lookup"><span data-stu-id="892be-129">Property</span></span>     | <span data-ttu-id="892be-130">类型</span><span class="sxs-lookup"><span data-stu-id="892be-130">Type</span></span>        | <span data-ttu-id="892be-131">说明</span><span class="sxs-lookup"><span data-stu-id="892be-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="892be-132">conditions</span><span class="sxs-lookup"><span data-stu-id="892be-132">conditions</span></span>|[<span data-ttu-id="892be-133">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="892be-133">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="892be-134">指定应用策略必须满足的规则。</span><span class="sxs-lookup"><span data-stu-id="892be-134">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="892be-135">必需。</span><span class="sxs-lookup"><span data-stu-id="892be-135">Required.</span></span> |
|<span data-ttu-id="892be-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="892be-136">createdDateTime</span></span>|<span data-ttu-id="892be-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="892be-137">DateTimeOffset</span></span>| <span data-ttu-id="892be-138">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="892be-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="892be-139">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="892be-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="892be-140">只读.</span><span class="sxs-lookup"><span data-stu-id="892be-140">Readonly.</span></span> |
|<span data-ttu-id="892be-141">description</span><span class="sxs-lookup"><span data-stu-id="892be-141">description</span></span>|<span data-ttu-id="892be-142">String</span><span class="sxs-lookup"><span data-stu-id="892be-142">String</span></span>| <span data-ttu-id="892be-143">未使用。</span><span class="sxs-lookup"><span data-stu-id="892be-143">Not used.</span></span> |
|<span data-ttu-id="892be-144">displayName</span><span class="sxs-lookup"><span data-stu-id="892be-144">displayName</span></span>|<span data-ttu-id="892be-145">String</span><span class="sxs-lookup"><span data-stu-id="892be-145">String</span></span>| <span data-ttu-id="892be-146">指定 conditionalAccessPolicy 对象的显示名称。</span><span class="sxs-lookup"><span data-stu-id="892be-146">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="892be-147">grantControls</span><span class="sxs-lookup"><span data-stu-id="892be-147">grantControls</span></span>|[<span data-ttu-id="892be-148">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="892be-148">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="892be-149">指定必须满足的授予控制以通过策略。</span><span class="sxs-lookup"><span data-stu-id="892be-149">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="892be-150">id</span><span class="sxs-lookup"><span data-stu-id="892be-150">id</span></span>|<span data-ttu-id="892be-151">String</span><span class="sxs-lookup"><span data-stu-id="892be-151">String</span></span>| <span data-ttu-id="892be-152">指定 conditionalAccessPolicy 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="892be-152">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="892be-153">只读。</span><span class="sxs-lookup"><span data-stu-id="892be-153">Read-only.</span></span>|
|<span data-ttu-id="892be-154">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="892be-154">modifiedDateTime</span></span>| <span data-ttu-id="892be-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="892be-155">DateTimeOffset</span></span>|<span data-ttu-id="892be-156">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="892be-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="892be-157">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="892be-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="892be-158">只读.</span><span class="sxs-lookup"><span data-stu-id="892be-158">Readonly.</span></span> |
|<span data-ttu-id="892be-159">sessionControls</span><span class="sxs-lookup"><span data-stu-id="892be-159">sessionControls</span></span>|[<span data-ttu-id="892be-160">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="892be-160">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="892be-161">指定登录后强制实施的会话控制。</span><span class="sxs-lookup"><span data-stu-id="892be-161">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="892be-162">state</span><span class="sxs-lookup"><span data-stu-id="892be-162">state</span></span>|<span data-ttu-id="892be-163">string</span><span class="sxs-lookup"><span data-stu-id="892be-163">string</span></span>| <span data-ttu-id="892be-164">指定 conditionalAccessPolicy 对象的状态。</span><span class="sxs-lookup"><span data-stu-id="892be-164">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="892be-165">可取值为：`enabled`、`disabled`、`enabledForReportingButNotEnforced`。</span><span class="sxs-lookup"><span data-stu-id="892be-165">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="892be-166">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="892be-166">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="892be-167">关系</span><span class="sxs-lookup"><span data-stu-id="892be-167">Relationships</span></span>

<span data-ttu-id="892be-168">无。</span><span class="sxs-lookup"><span data-stu-id="892be-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="892be-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="892be-169">JSON representation</span></span>

<span data-ttu-id="892be-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="892be-170">The following is a JSON representation of the resource.</span></span>

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


