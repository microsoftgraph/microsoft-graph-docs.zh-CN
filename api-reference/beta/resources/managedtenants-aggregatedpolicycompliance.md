---
title: aggregatedPolicyCompliance 资源类型
description: 表示托管租户的设备合规性聚合视图。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 8b2c6ce85c0ec6df361ddfeb13a851740efb2acb
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402073"
---
# <a name="aggregatedpolicycompliance-resource-type"></a><span data-ttu-id="4abf9-103">aggregatedPolicyCompliance 资源类型</span><span class="sxs-lookup"><span data-stu-id="4abf9-103">aggregatedPolicyCompliance resource type</span></span>

<span data-ttu-id="4abf9-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="4abf9-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4abf9-105">表示托管租户的设备合规性聚合视图。</span><span class="sxs-lookup"><span data-stu-id="4abf9-105">Represents an aggregate view of device compliance for a managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="4abf9-106">方法</span><span class="sxs-lookup"><span data-stu-id="4abf9-106">Methods</span></span>
|<span data-ttu-id="4abf9-107">方法</span><span class="sxs-lookup"><span data-stu-id="4abf9-107">Method</span></span>|<span data-ttu-id="4abf9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4abf9-108">Return type</span></span>|<span data-ttu-id="4abf9-109">说明</span><span class="sxs-lookup"><span data-stu-id="4abf9-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4abf9-110">列出 aggregatedPolicyCompliances</span><span class="sxs-lookup"><span data-stu-id="4abf9-110">List aggregatedPolicyCompliances</span></span>](../api/managedtenants-managedtenant-list-aggregatedpolicycompliances.md)|<span data-ttu-id="4abf9-111">[microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4abf9-111">[microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) collection</span></span>|<span data-ttu-id="4abf9-112">获取聚合 [PolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="4abf9-112">Get a list of the [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) objects and their properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="4abf9-113">属性</span><span class="sxs-lookup"><span data-stu-id="4abf9-113">Properties</span></span>
|<span data-ttu-id="4abf9-114">属性</span><span class="sxs-lookup"><span data-stu-id="4abf9-114">Property</span></span>|<span data-ttu-id="4abf9-115">类型</span><span class="sxs-lookup"><span data-stu-id="4abf9-115">Type</span></span>|<span data-ttu-id="4abf9-116">说明</span><span class="sxs-lookup"><span data-stu-id="4abf9-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4abf9-117">compliancePolicyId</span><span class="sxs-lookup"><span data-stu-id="4abf9-117">compliancePolicyId</span></span>|<span data-ttu-id="4abf9-118">String</span><span class="sxs-lookup"><span data-stu-id="4abf9-118">String</span></span>|<span data-ttu-id="4abf9-119">设备合规性策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="4abf9-119">Identifier for the device compliance policy.</span></span> <span data-ttu-id="4abf9-120">可选。</span><span class="sxs-lookup"><span data-stu-id="4abf9-120">Optional.</span></span> <span data-ttu-id="4abf9-121">只读。</span><span class="sxs-lookup"><span data-stu-id="4abf9-121">Read-only.</span></span>|
|<span data-ttu-id="4abf9-122">compliancePolicyName</span><span class="sxs-lookup"><span data-stu-id="4abf9-122">compliancePolicyName</span></span>|<span data-ttu-id="4abf9-123">String</span><span class="sxs-lookup"><span data-stu-id="4abf9-123">String</span></span>|<span data-ttu-id="4abf9-124">设备合规性策略的名称。</span><span class="sxs-lookup"><span data-stu-id="4abf9-124">Name of the device compliance policy.</span></span> <span data-ttu-id="4abf9-125">可选。</span><span class="sxs-lookup"><span data-stu-id="4abf9-125">Optional.</span></span> <span data-ttu-id="4abf9-126">只读。</span><span class="sxs-lookup"><span data-stu-id="4abf9-126">Read-only.</span></span>|
|<span data-ttu-id="4abf9-127">compliancePolicyPlatform</span><span class="sxs-lookup"><span data-stu-id="4abf9-127">compliancePolicyPlatform</span></span>|<span data-ttu-id="4abf9-128">String</span><span class="sxs-lookup"><span data-stu-id="4abf9-128">String</span></span>|<span data-ttu-id="4abf9-129">设备合规性策略的平台。</span><span class="sxs-lookup"><span data-stu-id="4abf9-129">Platform for the device compliance policy.</span></span> <span data-ttu-id="4abf9-130">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`androidAOSP`、`all`。</span><span class="sxs-lookup"><span data-stu-id="4abf9-130">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidAOSP`, `all`.</span></span> <span data-ttu-id="4abf9-131">可选。</span><span class="sxs-lookup"><span data-stu-id="4abf9-131">Optional.</span></span> <span data-ttu-id="4abf9-132">只读。</span><span class="sxs-lookup"><span data-stu-id="4abf9-132">Read-only.</span></span>|
|<span data-ttu-id="4abf9-133">compliancePolicyType</span><span class="sxs-lookup"><span data-stu-id="4abf9-133">compliancePolicyType</span></span>|<span data-ttu-id="4abf9-134">String</span><span class="sxs-lookup"><span data-stu-id="4abf9-134">String</span></span>|<span data-ttu-id="4abf9-135">合规性策略的类型。</span><span class="sxs-lookup"><span data-stu-id="4abf9-135">The type of compliance policy.</span></span> <span data-ttu-id="4abf9-136">可选。</span><span class="sxs-lookup"><span data-stu-id="4abf9-136">Optional.</span></span> <span data-ttu-id="4abf9-137">只读。</span><span class="sxs-lookup"><span data-stu-id="4abf9-137">Read-only.</span></span>|
|<span data-ttu-id="4abf9-138">id</span><span class="sxs-lookup"><span data-stu-id="4abf9-138">id</span></span>|<span data-ttu-id="4abf9-139">String</span><span class="sxs-lookup"><span data-stu-id="4abf9-139">String</span></span>|<span data-ttu-id="4abf9-140">聚合设备合规性策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4abf9-140">Unique identifier for the aggregate device compliance policy.</span></span> <span data-ttu-id="4abf9-141">必填。</span><span class="sxs-lookup"><span data-stu-id="4abf9-141">Required.</span></span> <span data-ttu-id="4abf9-142">只读</span><span class="sxs-lookup"><span data-stu-id="4abf9-142">Read-only</span></span>|
|<span data-ttu-id="4abf9-143">lastRefreshedDateTime</span><span class="sxs-lookup"><span data-stu-id="4abf9-143">lastRefreshedDateTime</span></span>|<span data-ttu-id="4abf9-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4abf9-144">DateTimeOffset</span></span>|<span data-ttu-id="4abf9-145">实体上次在多租户管理平台中更新的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4abf9-145">Date and time the entity was last updated in the multi-tenant management platform.</span></span> <span data-ttu-id="4abf9-146">可选。</span><span class="sxs-lookup"><span data-stu-id="4abf9-146">Optional.</span></span> <span data-ttu-id="4abf9-147">只读。</span><span class="sxs-lookup"><span data-stu-id="4abf9-147">Read-only.</span></span>|
|<span data-ttu-id="4abf9-148">numberOfCompliantDevices</span><span class="sxs-lookup"><span data-stu-id="4abf9-148">numberOfCompliantDevices</span></span>|<span data-ttu-id="4abf9-149">Int64</span><span class="sxs-lookup"><span data-stu-id="4abf9-149">Int64</span></span>|<span data-ttu-id="4abf9-150">符合标准的设备数量。</span><span class="sxs-lookup"><span data-stu-id="4abf9-150">The number of devices that are in a compliant status.</span></span> <span data-ttu-id="4abf9-151">可选。</span><span class="sxs-lookup"><span data-stu-id="4abf9-151">Optional.</span></span> <span data-ttu-id="4abf9-152">只读。</span><span class="sxs-lookup"><span data-stu-id="4abf9-152">Read-only.</span></span>|
|<span data-ttu-id="4abf9-153">numberOfErrorDevices</span><span class="sxs-lookup"><span data-stu-id="4abf9-153">numberOfErrorDevices</span></span>|<span data-ttu-id="4abf9-154">Int64</span><span class="sxs-lookup"><span data-stu-id="4abf9-154">Int64</span></span>|<span data-ttu-id="4abf9-155">出现错误状态的设备数。</span><span class="sxs-lookup"><span data-stu-id="4abf9-155">The number of devices that are in an error status.</span></span> <span data-ttu-id="4abf9-156">可选。</span><span class="sxs-lookup"><span data-stu-id="4abf9-156">Optional.</span></span> <span data-ttu-id="4abf9-157">只读。</span><span class="sxs-lookup"><span data-stu-id="4abf9-157">Read-only.</span></span>|
|<span data-ttu-id="4abf9-158">numberOfNonCompliantDevices</span><span class="sxs-lookup"><span data-stu-id="4abf9-158">numberOfNonCompliantDevices</span></span>|<span data-ttu-id="4abf9-159">Int64</span><span class="sxs-lookup"><span data-stu-id="4abf9-159">Int64</span></span>|<span data-ttu-id="4abf9-160">不合规状态的设备数量。</span><span class="sxs-lookup"><span data-stu-id="4abf9-160">The number of device that are in a non-compliant status.</span></span> <span data-ttu-id="4abf9-161">可选。</span><span class="sxs-lookup"><span data-stu-id="4abf9-161">Optional.</span></span> <span data-ttu-id="4abf9-162">只读。</span><span class="sxs-lookup"><span data-stu-id="4abf9-162">Read-only.</span></span>|
|<span data-ttu-id="4abf9-163">policyModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4abf9-163">policyModifiedDateTime</span></span>|<span data-ttu-id="4abf9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4abf9-164">DateTimeOffset</span></span>|<span data-ttu-id="4abf9-165">上次修改设备策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4abf9-165">The date and time the device policy was last modified.</span></span> <span data-ttu-id="4abf9-166">可选。</span><span class="sxs-lookup"><span data-stu-id="4abf9-166">Optional.</span></span> <span data-ttu-id="4abf9-167">只读。</span><span class="sxs-lookup"><span data-stu-id="4abf9-167">Read-only.</span></span>|
|<span data-ttu-id="4abf9-168">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="4abf9-168">tenantDisplayName</span></span>|<span data-ttu-id="4abf9-169">String</span><span class="sxs-lookup"><span data-stu-id="4abf9-169">String</span></span>|<span data-ttu-id="4abf9-170">托管显示名称租户的租户。</span><span class="sxs-lookup"><span data-stu-id="4abf9-170">The display name for the managed tenant.</span></span> <span data-ttu-id="4abf9-171">可选。</span><span class="sxs-lookup"><span data-stu-id="4abf9-171">Optional.</span></span> <span data-ttu-id="4abf9-172">只读。</span><span class="sxs-lookup"><span data-stu-id="4abf9-172">Read-only.</span></span>|
|<span data-ttu-id="4abf9-173">tenantId</span><span class="sxs-lookup"><span data-stu-id="4abf9-173">tenantId</span></span>|<span data-ttu-id="4abf9-174">String</span><span class="sxs-lookup"><span data-stu-id="4abf9-174">String</span></span>|<span data-ttu-id="4abf9-175">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="4abf9-175">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="4abf9-176">可选。</span><span class="sxs-lookup"><span data-stu-id="4abf9-176">Optional.</span></span> <span data-ttu-id="4abf9-177">只读。</span><span class="sxs-lookup"><span data-stu-id="4abf9-177">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4abf9-178">关系</span><span class="sxs-lookup"><span data-stu-id="4abf9-178">Relationships</span></span>
<span data-ttu-id="4abf9-179">无。</span><span class="sxs-lookup"><span data-stu-id="4abf9-179">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4abf9-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4abf9-180">JSON representation</span></span>
<span data-ttu-id="4abf9-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4abf9-181">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.aggregatedPolicyCompliance",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.aggregatedPolicyCompliance",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "compliancePolicyId": "String",
  "compliancePolicyName": "String",
  "compliancePolicyType": "String",
  "compliancePolicyPlatform": "String",
  "numberOfCompliantDevices": "Integer",
  "numberOfNonCompliantDevices": "Integer",
  "numberOfErrorDevices": "Integer",
  "policyModifiedDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
