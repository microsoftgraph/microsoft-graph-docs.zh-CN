---
title: deviceCompliancePolicySettingStateSummary 资源类型
description: 表示给定托管租户的设备合规性策略设置状态摘要。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 02b69b5df1c6ae482c653960a0081bc078be815d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402067"
---
# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a><span data-ttu-id="98028-103">deviceCompliancePolicySettingStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="98028-103">deviceCompliancePolicySettingStateSummary resource type</span></span>

<span data-ttu-id="98028-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="98028-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98028-105">表示给定托管租户的设备合规性策略设置状态摘要。</span><span class="sxs-lookup"><span data-stu-id="98028-105">Represents a summary of device compliance policy setting states for a given managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="98028-106">方法</span><span class="sxs-lookup"><span data-stu-id="98028-106">Methods</span></span>
|<span data-ttu-id="98028-107">方法</span><span class="sxs-lookup"><span data-stu-id="98028-107">Method</span></span>|<span data-ttu-id="98028-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="98028-108">Return type</span></span>|<span data-ttu-id="98028-109">说明</span><span class="sxs-lookup"><span data-stu-id="98028-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="98028-110">列出 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="98028-110">List deviceCompliancePolicySettingStateSummary</span></span>](../api/managedtenants-managedtenant-list-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="98028-111">[microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="98028-111">[microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) collection</span></span>|<span data-ttu-id="98028-112">获取 [deviceCompliancePolicySettingStateSummary 对象](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="98028-112">Get a list of the [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) objects and their properties.</span></span>|
|[<span data-ttu-id="98028-113">获取 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="98028-113">Get deviceCompliancePolicySettingStateSummary</span></span>](../api/managedtenants-devicecompliancepolicysettingstatesummary-get.md)|[<span data-ttu-id="98028-114">microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="98028-114">microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary</span></span>](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)|<span data-ttu-id="98028-115">读取 [deviceCompliancePolicySettingStateSummary 对象的属性和](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="98028-115">Read the properties and relationships of a [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="98028-116">属性</span><span class="sxs-lookup"><span data-stu-id="98028-116">Properties</span></span>
|<span data-ttu-id="98028-117">属性</span><span class="sxs-lookup"><span data-stu-id="98028-117">Property</span></span>|<span data-ttu-id="98028-118">类型</span><span class="sxs-lookup"><span data-stu-id="98028-118">Type</span></span>|<span data-ttu-id="98028-119">说明</span><span class="sxs-lookup"><span data-stu-id="98028-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98028-120">id</span><span class="sxs-lookup"><span data-stu-id="98028-120">id</span></span>|<span data-ttu-id="98028-121">String</span><span class="sxs-lookup"><span data-stu-id="98028-121">String</span></span>|<span data-ttu-id="98028-122">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="98028-122">The unique identifier for this entity.</span></span> <span data-ttu-id="98028-123">必填。</span><span class="sxs-lookup"><span data-stu-id="98028-123">Required.</span></span> <span data-ttu-id="98028-124">只读。</span><span class="sxs-lookup"><span data-stu-id="98028-124">Read-only.</span></span>|
|<span data-ttu-id="98028-125">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98028-125">conflictDeviceCount</span></span>|<span data-ttu-id="98028-126">Int32</span><span class="sxs-lookup"><span data-stu-id="98028-126">Int32</span></span>|<span data-ttu-id="98028-127">冲突状态中的设备数。</span><span class="sxs-lookup"><span data-stu-id="98028-127">The number of devices in a conflict state.</span></span> <span data-ttu-id="98028-128">可选。</span><span class="sxs-lookup"><span data-stu-id="98028-128">Optional.</span></span> <span data-ttu-id="98028-129">只读。</span><span class="sxs-lookup"><span data-stu-id="98028-129">Read-only.</span></span>|
|<span data-ttu-id="98028-130">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98028-130">errorDeviceCount</span></span>|<span data-ttu-id="98028-131">Int32</span><span class="sxs-lookup"><span data-stu-id="98028-131">Int32</span></span>|<span data-ttu-id="98028-132">出现错误状态的设备数。</span><span class="sxs-lookup"><span data-stu-id="98028-132">The number of devices in an error state.</span></span> <span data-ttu-id="98028-133">可选。</span><span class="sxs-lookup"><span data-stu-id="98028-133">Optional.</span></span> <span data-ttu-id="98028-134">只读。</span><span class="sxs-lookup"><span data-stu-id="98028-134">Read-only.</span></span>|
|<span data-ttu-id="98028-135">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98028-135">failedDeviceCount</span></span>|<span data-ttu-id="98028-136">Int32</span><span class="sxs-lookup"><span data-stu-id="98028-136">Int32</span></span>|<span data-ttu-id="98028-137">故障状态中的设备数。</span><span class="sxs-lookup"><span data-stu-id="98028-137">The number of devices in a failed state.</span></span> <span data-ttu-id="98028-138">可选。</span><span class="sxs-lookup"><span data-stu-id="98028-138">Optional.</span></span> <span data-ttu-id="98028-139">只读。</span><span class="sxs-lookup"><span data-stu-id="98028-139">Read-only.</span></span>|
|<span data-ttu-id="98028-140">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="98028-140">intuneAccountId</span></span>|<span data-ttu-id="98028-141">String</span><span class="sxs-lookup"><span data-stu-id="98028-141">String</span></span>|<span data-ttu-id="98028-142">帐户标识Microsoft Intune标识。</span><span class="sxs-lookup"><span data-stu-id="98028-142">The identifer for the Microsoft Intune account.</span></span> <span data-ttu-id="98028-143">必填。</span><span class="sxs-lookup"><span data-stu-id="98028-143">Required.</span></span> <span data-ttu-id="98028-144">只读。</span><span class="sxs-lookup"><span data-stu-id="98028-144">Read-only.</span></span>|
|<span data-ttu-id="98028-145">intuneSettingId</span><span class="sxs-lookup"><span data-stu-id="98028-145">intuneSettingId</span></span>|<span data-ttu-id="98028-146">String</span><span class="sxs-lookup"><span data-stu-id="98028-146">String</span></span>|<span data-ttu-id="98028-147">Intune 设置的标识符。</span><span class="sxs-lookup"><span data-stu-id="98028-147">The identifier for the Intune setting.</span></span> <span data-ttu-id="98028-148">可选。</span><span class="sxs-lookup"><span data-stu-id="98028-148">Optional.</span></span> <span data-ttu-id="98028-149">只读。</span><span class="sxs-lookup"><span data-stu-id="98028-149">Read-only.</span></span>|
|<span data-ttu-id="98028-150">lastRefreshedDateTime</span><span class="sxs-lookup"><span data-stu-id="98028-150">lastRefreshedDateTime</span></span>|<span data-ttu-id="98028-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98028-151">DateTimeOffset</span></span>|<span data-ttu-id="98028-152">实体上次在多租户管理平台中更新的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="98028-152">Date and time the entity was last updated in the multi-tenant management platform.</span></span> <span data-ttu-id="98028-153">可选。</span><span class="sxs-lookup"><span data-stu-id="98028-153">Optional.</span></span> <span data-ttu-id="98028-154">只读。</span><span class="sxs-lookup"><span data-stu-id="98028-154">Read-only.</span></span>|
|<span data-ttu-id="98028-155">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98028-155">notApplicableDeviceCount</span></span>|<span data-ttu-id="98028-156">Int32</span><span class="sxs-lookup"><span data-stu-id="98028-156">Int32</span></span>|<span data-ttu-id="98028-157">状态不适用的设备数量。</span><span class="sxs-lookup"><span data-stu-id="98028-157">The number of devices in a not applicable state.</span></span> <span data-ttu-id="98028-158">可选。</span><span class="sxs-lookup"><span data-stu-id="98028-158">Optional.</span></span> <span data-ttu-id="98028-159">只读。</span><span class="sxs-lookup"><span data-stu-id="98028-159">Read-only.</span></span>|
|<span data-ttu-id="98028-160">pendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98028-160">pendingDeviceCount</span></span>|<span data-ttu-id="98028-161">Int32</span><span class="sxs-lookup"><span data-stu-id="98028-161">Int32</span></span>|<span data-ttu-id="98028-162">挂起状态的设备数。</span><span class="sxs-lookup"><span data-stu-id="98028-162">The number of devices in a pending state.</span></span> <span data-ttu-id="98028-163">可选。</span><span class="sxs-lookup"><span data-stu-id="98028-163">Optional.</span></span> <span data-ttu-id="98028-164">只读。</span><span class="sxs-lookup"><span data-stu-id="98028-164">Read-only.</span></span>|
|<span data-ttu-id="98028-165">policyType</span><span class="sxs-lookup"><span data-stu-id="98028-165">policyType</span></span>|<span data-ttu-id="98028-166">String</span><span class="sxs-lookup"><span data-stu-id="98028-166">String</span></span>|<span data-ttu-id="98028-167">设备合规性策略的类型。</span><span class="sxs-lookup"><span data-stu-id="98028-167">The type for the device compliance policy.</span></span> <span data-ttu-id="98028-168">可选。</span><span class="sxs-lookup"><span data-stu-id="98028-168">Optional.</span></span> <span data-ttu-id="98028-169">只读。</span><span class="sxs-lookup"><span data-stu-id="98028-169">Read-only.</span></span>|
|<span data-ttu-id="98028-170">settingName</span><span class="sxs-lookup"><span data-stu-id="98028-170">settingName</span></span>|<span data-ttu-id="98028-171">String</span><span class="sxs-lookup"><span data-stu-id="98028-171">String</span></span>|<span data-ttu-id="98028-172">设备合规性策略中设置的名称。</span><span class="sxs-lookup"><span data-stu-id="98028-172">The name for the setting within the device compliance policy.</span></span> <span data-ttu-id="98028-173">可选。</span><span class="sxs-lookup"><span data-stu-id="98028-173">Optional.</span></span> <span data-ttu-id="98028-174">只读。</span><span class="sxs-lookup"><span data-stu-id="98028-174">Read-only.</span></span>|
|<span data-ttu-id="98028-175">succeededDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98028-175">succeededDeviceCount</span></span>|<span data-ttu-id="98028-176">Int32</span><span class="sxs-lookup"><span data-stu-id="98028-176">Int32</span></span>|<span data-ttu-id="98028-177">状态成功的设备数。</span><span class="sxs-lookup"><span data-stu-id="98028-177">The number of devices in a succeeded state.</span></span> <span data-ttu-id="98028-178">可选。</span><span class="sxs-lookup"><span data-stu-id="98028-178">Optional.</span></span> <span data-ttu-id="98028-179">只读。</span><span class="sxs-lookup"><span data-stu-id="98028-179">Read-only.</span></span>|
|<span data-ttu-id="98028-180">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="98028-180">tenantDisplayName</span></span>|<span data-ttu-id="98028-181">String</span><span class="sxs-lookup"><span data-stu-id="98028-181">String</span></span>|<span data-ttu-id="98028-182">托管显示名称租户的租户。</span><span class="sxs-lookup"><span data-stu-id="98028-182">The display name for the managed tenant.</span></span> <span data-ttu-id="98028-183">必填。</span><span class="sxs-lookup"><span data-stu-id="98028-183">Required.</span></span> <span data-ttu-id="98028-184">只读。</span><span class="sxs-lookup"><span data-stu-id="98028-184">Read-only.</span></span>|
|<span data-ttu-id="98028-185">tenantId</span><span class="sxs-lookup"><span data-stu-id="98028-185">tenantId</span></span>|<span data-ttu-id="98028-186">String</span><span class="sxs-lookup"><span data-stu-id="98028-186">String</span></span>|<span data-ttu-id="98028-187">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="98028-187">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="98028-188">必填。</span><span class="sxs-lookup"><span data-stu-id="98028-188">Required.</span></span> <span data-ttu-id="98028-189">只读。</span><span class="sxs-lookup"><span data-stu-id="98028-189">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98028-190">关系</span><span class="sxs-lookup"><span data-stu-id="98028-190">Relationships</span></span>
<span data-ttu-id="98028-191">无。</span><span class="sxs-lookup"><span data-stu-id="98028-191">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="98028-192">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98028-192">JSON representation</span></span>
<span data-ttu-id="98028-193">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98028-193">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "conflictDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "failedDeviceCount": "Integer",
  "intuneAccountId": "String",
  "intuneSettingId": "String",
  "notApplicableDeviceCount": "Integer",
  "pendingDeviceCount": "Integer",
  "policyType": "String",
  "settingName": "String",
  "succeededDeviceCount": "Integer",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
