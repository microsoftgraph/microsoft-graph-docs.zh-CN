---
title: managedDeviceComplianceTrend 资源类型
description: 表示给定托管租户的兼容和不兼容设备的趋势。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 70c3c84c5da6ffb2660a6289bc55c6ab3eef64be
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402065"
---
# <a name="manageddevicecompliancetrend-resource-type"></a><span data-ttu-id="307f6-103">managedDeviceComplianceTrend 资源类型</span><span class="sxs-lookup"><span data-stu-id="307f6-103">managedDeviceComplianceTrend resource type</span></span>

<span data-ttu-id="307f6-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="307f6-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="307f6-105">表示给定托管租户的兼容和不兼容设备的趋势。</span><span class="sxs-lookup"><span data-stu-id="307f6-105">Represents a trend of compliant and non-compliant devices for a given managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="307f6-106">方法</span><span class="sxs-lookup"><span data-stu-id="307f6-106">Methods</span></span>
|<span data-ttu-id="307f6-107">方法</span><span class="sxs-lookup"><span data-stu-id="307f6-107">Method</span></span>|<span data-ttu-id="307f6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="307f6-108">Return type</span></span>|<span data-ttu-id="307f6-109">说明</span><span class="sxs-lookup"><span data-stu-id="307f6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="307f6-110">列出 managedDeviceComplianceTrends</span><span class="sxs-lookup"><span data-stu-id="307f6-110">List managedDeviceComplianceTrends</span></span>](../api/managedtenants-managedtenant-list-manageddevicecompliancetrends.md)|<span data-ttu-id="307f6-111">[microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) 集合</span><span class="sxs-lookup"><span data-stu-id="307f6-111">[microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) collection</span></span>|<span data-ttu-id="307f6-112">获取 [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="307f6-112">Get a list of the [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) objects and their properties.</span></span>|
|[<span data-ttu-id="307f6-113">获取 managedDeviceComplianceTrend</span><span class="sxs-lookup"><span data-stu-id="307f6-113">Get managedDeviceComplianceTrend</span></span>](../api/managedtenants-manageddevicecompliancetrend-get.md)|[<span data-ttu-id="307f6-114">microsoft.graph.managedTenants.managedDeviceComplianceTrend</span><span class="sxs-lookup"><span data-stu-id="307f6-114">microsoft.graph.managedTenants.managedDeviceComplianceTrend</span></span>](../resources/managedtenants-manageddevicecompliancetrend.md)|<span data-ttu-id="307f6-115">读取 [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="307f6-115">Read the properties and relationships of a [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="307f6-116">属性</span><span class="sxs-lookup"><span data-stu-id="307f6-116">Properties</span></span>
|<span data-ttu-id="307f6-117">属性</span><span class="sxs-lookup"><span data-stu-id="307f6-117">Property</span></span>|<span data-ttu-id="307f6-118">类型</span><span class="sxs-lookup"><span data-stu-id="307f6-118">Type</span></span>|<span data-ttu-id="307f6-119">说明</span><span class="sxs-lookup"><span data-stu-id="307f6-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="307f6-120">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="307f6-120">compliantDeviceCount</span></span>|<span data-ttu-id="307f6-121">Int32</span><span class="sxs-lookup"><span data-stu-id="307f6-121">Int32</span></span>|<span data-ttu-id="307f6-122">具有兼容状态的设备数量。</span><span class="sxs-lookup"><span data-stu-id="307f6-122">The number of devices with a compliant status.</span></span> <span data-ttu-id="307f6-123">必填。</span><span class="sxs-lookup"><span data-stu-id="307f6-123">Required.</span></span> <span data-ttu-id="307f6-124">只读。</span><span class="sxs-lookup"><span data-stu-id="307f6-124">Read-only.</span></span>|
|<span data-ttu-id="307f6-125">configManagerDeviceCount</span><span class="sxs-lookup"><span data-stu-id="307f6-125">configManagerDeviceCount</span></span>|<span data-ttu-id="307f6-126">Int32</span><span class="sxs-lookup"><span data-stu-id="307f6-126">Int32</span></span>|<span data-ttu-id="307f6-127">Configuration Manager 管理的设备数量。</span><span class="sxs-lookup"><span data-stu-id="307f6-127">The number of devices manged by Configuration Manager.</span></span> <span data-ttu-id="307f6-128">必填。</span><span class="sxs-lookup"><span data-stu-id="307f6-128">Required.</span></span> <span data-ttu-id="307f6-129">只读。</span><span class="sxs-lookup"><span data-stu-id="307f6-129">Read-only.</span></span>|
|<span data-ttu-id="307f6-130">countDateTime</span><span class="sxs-lookup"><span data-stu-id="307f6-130">countDateTime</span></span>|<span data-ttu-id="307f6-131">String</span><span class="sxs-lookup"><span data-stu-id="307f6-131">String</span></span>|<span data-ttu-id="307f6-132">执行合规性快照的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="307f6-132">The date and time compliance snapshot was performed.</span></span> <span data-ttu-id="307f6-133">必填。</span><span class="sxs-lookup"><span data-stu-id="307f6-133">Required.</span></span> <span data-ttu-id="307f6-134">只读。</span><span class="sxs-lookup"><span data-stu-id="307f6-134">Read-only.</span></span>|
|<span data-ttu-id="307f6-135">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="307f6-135">errorDeviceCount</span></span>|<span data-ttu-id="307f6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="307f6-136">Int32</span></span>|<span data-ttu-id="307f6-137">出现错误状态的设备数。</span><span class="sxs-lookup"><span data-stu-id="307f6-137">The number of devices with an error status.</span></span> <span data-ttu-id="307f6-138">必填。</span><span class="sxs-lookup"><span data-stu-id="307f6-138">Required.</span></span> <span data-ttu-id="307f6-139">只读。</span><span class="sxs-lookup"><span data-stu-id="307f6-139">Read-only.</span></span>|
|<span data-ttu-id="307f6-140">id</span><span class="sxs-lookup"><span data-stu-id="307f6-140">id</span></span>|<span data-ttu-id="307f6-141">String</span><span class="sxs-lookup"><span data-stu-id="307f6-141">String</span></span>|<span data-ttu-id="307f6-142">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="307f6-142">The unique identifier for this entity.</span></span> <span data-ttu-id="307f6-143">必填。</span><span class="sxs-lookup"><span data-stu-id="307f6-143">Required.</span></span> <span data-ttu-id="307f6-144">只读。</span><span class="sxs-lookup"><span data-stu-id="307f6-144">Read-only.</span></span>|
|<span data-ttu-id="307f6-145">inGracePeriodDeviceCount</span><span class="sxs-lookup"><span data-stu-id="307f6-145">inGracePeriodDeviceCount</span></span>|<span data-ttu-id="307f6-146">Int32</span><span class="sxs-lookup"><span data-stu-id="307f6-146">Int32</span></span>|<span data-ttu-id="307f6-147">宽限期状态的设备数量。</span><span class="sxs-lookup"><span data-stu-id="307f6-147">The number of devices that are in a grace period status.</span></span> <span data-ttu-id="307f6-148">必填。</span><span class="sxs-lookup"><span data-stu-id="307f6-148">Required.</span></span> <span data-ttu-id="307f6-149">只读。</span><span class="sxs-lookup"><span data-stu-id="307f6-149">Read-only.</span></span>|
|<span data-ttu-id="307f6-150">noncompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="307f6-150">noncompliantDeviceCount</span></span>|<span data-ttu-id="307f6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="307f6-151">Int32</span></span>|<span data-ttu-id="307f6-152">不合规状态的设备数量。</span><span class="sxs-lookup"><span data-stu-id="307f6-152">The number of devices that are in a non-compliant status.</span></span> <span data-ttu-id="307f6-153">必填。</span><span class="sxs-lookup"><span data-stu-id="307f6-153">Required.</span></span> <span data-ttu-id="307f6-154">只读。</span><span class="sxs-lookup"><span data-stu-id="307f6-154">Read-only.</span></span>|
|<span data-ttu-id="307f6-155">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="307f6-155">tenantDisplayName</span></span>|<span data-ttu-id="307f6-156">String</span><span class="sxs-lookup"><span data-stu-id="307f6-156">String</span></span>|<span data-ttu-id="307f6-157">托管显示名称租户的租户。</span><span class="sxs-lookup"><span data-stu-id="307f6-157">The display name for the managed tenant.</span></span> <span data-ttu-id="307f6-158">可选。</span><span class="sxs-lookup"><span data-stu-id="307f6-158">Optional.</span></span> <span data-ttu-id="307f6-159">只读。</span><span class="sxs-lookup"><span data-stu-id="307f6-159">Read-only.</span></span>|
|<span data-ttu-id="307f6-160">tenantId</span><span class="sxs-lookup"><span data-stu-id="307f6-160">tenantId</span></span>|<span data-ttu-id="307f6-161">String</span><span class="sxs-lookup"><span data-stu-id="307f6-161">String</span></span>|<span data-ttu-id="307f6-162">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="307f6-162">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="307f6-163">可选。</span><span class="sxs-lookup"><span data-stu-id="307f6-163">Optional.</span></span> <span data-ttu-id="307f6-164">只读。</span><span class="sxs-lookup"><span data-stu-id="307f6-164">Read-only.</span></span>|
|<span data-ttu-id="307f6-165">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="307f6-165">unknownDeviceCount</span></span>|<span data-ttu-id="307f6-166">Int32</span><span class="sxs-lookup"><span data-stu-id="307f6-166">Int32</span></span>|<span data-ttu-id="307f6-167">未知状态的设备数量。</span><span class="sxs-lookup"><span data-stu-id="307f6-167">The number of devices in an unknown status.</span></span> <span data-ttu-id="307f6-168">必填。</span><span class="sxs-lookup"><span data-stu-id="307f6-168">Required.</span></span> <span data-ttu-id="307f6-169">只读。</span><span class="sxs-lookup"><span data-stu-id="307f6-169">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="307f6-170">关系</span><span class="sxs-lookup"><span data-stu-id="307f6-170">Relationships</span></span>
<span data-ttu-id="307f6-171">无。</span><span class="sxs-lookup"><span data-stu-id="307f6-171">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="307f6-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="307f6-172">JSON representation</span></span>
<span data-ttu-id="307f6-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="307f6-173">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "unknownDeviceCount": "Integer",
  "compliantDeviceCount": "Integer",
  "noncompliantDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "inGracePeriodDeviceCount": "Integer",
  "configManagerDeviceCount": "Integer",
  "countDateTime": "String"
}
```
