---
title: conditionalAccessPolicy 资源类型
description: 表示 Azure Active Directory 条件访问策略。 条件访问策略是定义访问方案的自定义规则。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 578d7cfcab984922d0c98f7cc8971daf9b10a2fa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958813"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="31ad3-104">conditionalAccessPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="31ad3-104">conditionalAccessPolicy resource type</span></span>

<span data-ttu-id="31ad3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31ad3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31ad3-106">表示 Azure Active Directory 条件访问策略。</span><span class="sxs-lookup"><span data-stu-id="31ad3-106">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="31ad3-107">条件访问策略是定义访问方案的自定义规则。</span><span class="sxs-lookup"><span data-stu-id="31ad3-107">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="31ad3-108">有关详细信息，请参阅条件 [访问文档](/azure/active-directory/conditional-access/)。</span><span class="sxs-lookup"><span data-stu-id="31ad3-108">For more information, see the [Conditional access documentation](/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="31ad3-109">Methods</span><span class="sxs-lookup"><span data-stu-id="31ad3-109">Methods</span></span>

| <span data-ttu-id="31ad3-110">方法</span><span class="sxs-lookup"><span data-stu-id="31ad3-110">Method</span></span>       | <span data-ttu-id="31ad3-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="31ad3-111">Return Type</span></span> | <span data-ttu-id="31ad3-112">说明</span><span class="sxs-lookup"><span data-stu-id="31ad3-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="31ad3-113">列出 conditionalAccessPolicies</span><span class="sxs-lookup"><span data-stu-id="31ad3-113">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="31ad3-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31ad3-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="31ad3-115">获取组织的所有 conditionalAccessPolicies 对象。</span><span class="sxs-lookup"><span data-stu-id="31ad3-115">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="31ad3-116">创建 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="31ad3-116">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="31ad3-117">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="31ad3-117">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="31ad3-118">创建新的 conditionalAccessPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="31ad3-118">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="31ad3-119">获取 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="31ad3-119">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="31ad3-120">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="31ad3-120">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="31ad3-121">读取 conditionalAccessPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="31ad3-121">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="31ad3-122">更新 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="31ad3-122">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="31ad3-123">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="31ad3-123">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="31ad3-124">更新 conditionalAccessPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="31ad3-124">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="31ad3-125">删除 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="31ad3-125">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="31ad3-126">无</span><span class="sxs-lookup"><span data-stu-id="31ad3-126">None</span></span> | <span data-ttu-id="31ad3-127">删除 conditionalAccessPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="31ad3-127">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="31ad3-128">属性</span><span class="sxs-lookup"><span data-stu-id="31ad3-128">Properties</span></span>

| <span data-ttu-id="31ad3-129">属性</span><span class="sxs-lookup"><span data-stu-id="31ad3-129">Property</span></span>     | <span data-ttu-id="31ad3-130">类型</span><span class="sxs-lookup"><span data-stu-id="31ad3-130">Type</span></span>        | <span data-ttu-id="31ad3-131">说明</span><span class="sxs-lookup"><span data-stu-id="31ad3-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="31ad3-132">conditions</span><span class="sxs-lookup"><span data-stu-id="31ad3-132">conditions</span></span>|[<span data-ttu-id="31ad3-133">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="31ad3-133">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="31ad3-134">指定应用策略时必须满足的规则。</span><span class="sxs-lookup"><span data-stu-id="31ad3-134">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="31ad3-135">必填。</span><span class="sxs-lookup"><span data-stu-id="31ad3-135">Required.</span></span> |
|<span data-ttu-id="31ad3-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31ad3-136">createdDateTime</span></span>|<span data-ttu-id="31ad3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31ad3-137">DateTimeOffset</span></span>| <span data-ttu-id="31ad3-138">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="31ad3-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="31ad3-139">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="31ad3-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="31ad3-140">只读。</span><span class="sxs-lookup"><span data-stu-id="31ad3-140">Readonly.</span></span> |
|<span data-ttu-id="31ad3-141">说明</span><span class="sxs-lookup"><span data-stu-id="31ad3-141">description</span></span>|<span data-ttu-id="31ad3-142">String</span><span class="sxs-lookup"><span data-stu-id="31ad3-142">String</span></span>| <span data-ttu-id="31ad3-143">未使用。</span><span class="sxs-lookup"><span data-stu-id="31ad3-143">Not used.</span></span> |
|<span data-ttu-id="31ad3-144">displayName</span><span class="sxs-lookup"><span data-stu-id="31ad3-144">displayName</span></span>|<span data-ttu-id="31ad3-145">String</span><span class="sxs-lookup"><span data-stu-id="31ad3-145">String</span></span>| <span data-ttu-id="31ad3-146">为 conditionalAccessPolicy 显示名称指定一个属性。</span><span class="sxs-lookup"><span data-stu-id="31ad3-146">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="31ad3-147">grantControls</span><span class="sxs-lookup"><span data-stu-id="31ad3-147">grantControls</span></span>|[<span data-ttu-id="31ad3-148">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="31ad3-148">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="31ad3-149">指定必须通过此策略而必须实现的授予控制。</span><span class="sxs-lookup"><span data-stu-id="31ad3-149">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="31ad3-150">id</span><span class="sxs-lookup"><span data-stu-id="31ad3-150">id</span></span>|<span data-ttu-id="31ad3-151">String</span><span class="sxs-lookup"><span data-stu-id="31ad3-151">String</span></span>| <span data-ttu-id="31ad3-152">指定 conditionalAccessPolicy 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="31ad3-152">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="31ad3-153">只读。</span><span class="sxs-lookup"><span data-stu-id="31ad3-153">Read-only.</span></span>|
|<span data-ttu-id="31ad3-154">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31ad3-154">modifiedDateTime</span></span>| <span data-ttu-id="31ad3-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31ad3-155">DateTimeOffset</span></span>|<span data-ttu-id="31ad3-156">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="31ad3-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="31ad3-157">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="31ad3-157">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="31ad3-158">只读。</span><span class="sxs-lookup"><span data-stu-id="31ad3-158">Readonly.</span></span> |
|<span data-ttu-id="31ad3-159">sessionControls</span><span class="sxs-lookup"><span data-stu-id="31ad3-159">sessionControls</span></span>|[<span data-ttu-id="31ad3-160">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="31ad3-160">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="31ad3-161">指定登录后强制执行的会话控件。</span><span class="sxs-lookup"><span data-stu-id="31ad3-161">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="31ad3-162">state</span><span class="sxs-lookup"><span data-stu-id="31ad3-162">state</span></span>|<span data-ttu-id="31ad3-163">conditionalAccessPolicyState</span><span class="sxs-lookup"><span data-stu-id="31ad3-163">conditionalAccessPolicyState</span></span>| <span data-ttu-id="31ad3-164">指定 conditionalAccessPolicy 对象的状态。</span><span class="sxs-lookup"><span data-stu-id="31ad3-164">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="31ad3-165">可取值为：`enabled`、`disabled`、`enabledForReportingButNotEnforced`。</span><span class="sxs-lookup"><span data-stu-id="31ad3-165">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="31ad3-166">必填。</span><span class="sxs-lookup"><span data-stu-id="31ad3-166">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="31ad3-167">关系</span><span class="sxs-lookup"><span data-stu-id="31ad3-167">Relationships</span></span>

<span data-ttu-id="31ad3-168">无。</span><span class="sxs-lookup"><span data-stu-id="31ad3-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31ad3-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31ad3-169">JSON representation</span></span>

<span data-ttu-id="31ad3-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31ad3-170">The following is a JSON representation of the resource.</span></span>

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
