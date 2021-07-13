---
title: conditionalAccessPolicyCoverage 资源类型
description: 表示有关定义Azure Active Directory托管租户的资源访问规则的任何策略的信息。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a4bc4f336692166ff032727a6fb13222edd9d7d9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402069"
---
# <a name="conditionalaccesspolicycoverage-resource-type"></a><span data-ttu-id="81856-103">conditionalAccessPolicyCoverage 资源类型</span><span class="sxs-lookup"><span data-stu-id="81856-103">conditionalAccessPolicyCoverage resource type</span></span>

<span data-ttu-id="81856-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="81856-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81856-105">表示有关定义Azure Active Directory托管租户的资源访问规则的任何策略的信息。</span><span class="sxs-lookup"><span data-stu-id="81856-105">Represents information about any Azure Active Directory policy that defines access rules of a resource for a given managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="81856-106">方法</span><span class="sxs-lookup"><span data-stu-id="81856-106">Methods</span></span>
|<span data-ttu-id="81856-107">方法</span><span class="sxs-lookup"><span data-stu-id="81856-107">Method</span></span>|<span data-ttu-id="81856-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="81856-108">Return type</span></span>|<span data-ttu-id="81856-109">说明</span><span class="sxs-lookup"><span data-stu-id="81856-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81856-110">列出 conditionalAccessPolicyCoverages</span><span class="sxs-lookup"><span data-stu-id="81856-110">List conditionalAccessPolicyCoverages</span></span>](../api/managedtenants-managedtenant-list-conditionalaccesspolicycoverages.md)|<span data-ttu-id="81856-111">[microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81856-111">[microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) collection</span></span>|<span data-ttu-id="81856-112">获取 [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="81856-112">Get a list of the [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) objects and their properties.</span></span>|
|[<span data-ttu-id="81856-113">获取 conditionalAccessPolicyCoverage</span><span class="sxs-lookup"><span data-stu-id="81856-113">Get conditionalAccessPolicyCoverage</span></span>](../api/managedtenants-conditionalaccesspolicycoverage-get.md)|[<span data-ttu-id="81856-114">microsoft.graph.managedTenants.conditionalAccessPolicyCoverage</span><span class="sxs-lookup"><span data-stu-id="81856-114">microsoft.graph.managedTenants.conditionalAccessPolicyCoverage</span></span>](../resources/managedtenants-conditionalaccesspolicycoverage.md)|<span data-ttu-id="81856-115">读取 [conditionalAccessPolicyCoverage 对象的属性和](../resources/managedtenants-conditionalaccesspolicycoverage.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="81856-115">Read the properties and relationships of a [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81856-116">属性</span><span class="sxs-lookup"><span data-stu-id="81856-116">Properties</span></span>
|<span data-ttu-id="81856-117">属性</span><span class="sxs-lookup"><span data-stu-id="81856-117">Property</span></span>|<span data-ttu-id="81856-118">类型</span><span class="sxs-lookup"><span data-stu-id="81856-118">Type</span></span>|<span data-ttu-id="81856-119">说明</span><span class="sxs-lookup"><span data-stu-id="81856-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81856-120">conditionalAccessPolicyState</span><span class="sxs-lookup"><span data-stu-id="81856-120">conditionalAccessPolicyState</span></span>|<span data-ttu-id="81856-121">String</span><span class="sxs-lookup"><span data-stu-id="81856-121">String</span></span>|<span data-ttu-id="81856-122">条件访问策略的状态。</span><span class="sxs-lookup"><span data-stu-id="81856-122">The state for the conditional access policy.</span></span> <span data-ttu-id="81856-123">可取值为：`enabled`、`disabled`、`enabledForReportingButNotEnforced`。</span><span class="sxs-lookup"><span data-stu-id="81856-123">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="81856-124">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="81856-124">Required.</span></span> <span data-ttu-id="81856-125">只读。</span><span class="sxs-lookup"><span data-stu-id="81856-125">Read-only.</span></span>|
|<span data-ttu-id="81856-126">id</span><span class="sxs-lookup"><span data-stu-id="81856-126">id</span></span>|<span data-ttu-id="81856-127">String</span><span class="sxs-lookup"><span data-stu-id="81856-127">String</span></span>|<span data-ttu-id="81856-128">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="81856-128">The unique identifier for this entity.</span></span> <span data-ttu-id="81856-129">必填。</span><span class="sxs-lookup"><span data-stu-id="81856-129">Required.</span></span> <span data-ttu-id="81856-130">只读。</span><span class="sxs-lookup"><span data-stu-id="81856-130">Read-only.</span></span>|
|<span data-ttu-id="81856-131">latestPolicyModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81856-131">latestPolicyModifiedDateTime</span></span>|<span data-ttu-id="81856-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81856-132">DateTimeOffset</span></span>|<span data-ttu-id="81856-133">上次修改条件访问策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="81856-133">The date and time the conditional access policy was last modified.</span></span> <span data-ttu-id="81856-134">必填。</span><span class="sxs-lookup"><span data-stu-id="81856-134">Required.</span></span> <span data-ttu-id="81856-135">只读。</span><span class="sxs-lookup"><span data-stu-id="81856-135">Read-only.</span></span>|
|<span data-ttu-id="81856-136">requiresDeviceCompliance</span><span class="sxs-lookup"><span data-stu-id="81856-136">requiresDeviceCompliance</span></span>|<span data-ttu-id="81856-137">布尔</span><span class="sxs-lookup"><span data-stu-id="81856-137">Boolean</span></span>|<span data-ttu-id="81856-138">指示条件访问策略是否需要设备符合性的标志。</span><span class="sxs-lookup"><span data-stu-id="81856-138">A flag indicating whether the conditional access policy requires device compliance.</span></span> <span data-ttu-id="81856-139">必填。</span><span class="sxs-lookup"><span data-stu-id="81856-139">Required.</span></span> <span data-ttu-id="81856-140">只读。</span><span class="sxs-lookup"><span data-stu-id="81856-140">Read-only.</span></span>|
|<span data-ttu-id="81856-141">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="81856-141">tenantDisplayName</span></span>|<span data-ttu-id="81856-142">String</span><span class="sxs-lookup"><span data-stu-id="81856-142">String</span></span>|<span data-ttu-id="81856-143">托管显示名称租户的租户。</span><span class="sxs-lookup"><span data-stu-id="81856-143">The display name for the managed tenant.</span></span> <span data-ttu-id="81856-144">必填。</span><span class="sxs-lookup"><span data-stu-id="81856-144">Required.</span></span> <span data-ttu-id="81856-145">只读。</span><span class="sxs-lookup"><span data-stu-id="81856-145">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81856-146">关系</span><span class="sxs-lookup"><span data-stu-id="81856-146">Relationships</span></span>
<span data-ttu-id="81856-147">无。</span><span class="sxs-lookup"><span data-stu-id="81856-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="81856-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81856-148">JSON representation</span></span>
<span data-ttu-id="81856-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81856-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "id": "String (identifier)",
  "tenantDisplayName": "String",
  "conditionalAccessPolicyState": "String",
  "requiresDeviceCompliance": "Boolean",
  "latestPolicyModifiedDateTime": "String (timestamp)"
}
```
