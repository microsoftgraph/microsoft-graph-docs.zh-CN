---
title: comanagedDevicesSummary 资源类型
description: Co 托管设备的摘要数据
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 42a92fd725c9f0b99037825c240dd017bf6c9c82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060774"
---
# <a name="comanageddevicessummary-resource-type"></a><span data-ttu-id="3b54e-103">comanagedDevicesSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b54e-103">comanagedDevicesSummary resource type</span></span>

<span data-ttu-id="3b54e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b54e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b54e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3b54e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b54e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3b54e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b54e-107">Co 托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="3b54e-107">Summary data for co managed devices</span></span>

## <a name="properties"></a><span data-ttu-id="3b54e-108">属性</span><span class="sxs-lookup"><span data-stu-id="3b54e-108">Properties</span></span>
|<span data-ttu-id="3b54e-109">属性</span><span class="sxs-lookup"><span data-stu-id="3b54e-109">Property</span></span>|<span data-ttu-id="3b54e-110">类型</span><span class="sxs-lookup"><span data-stu-id="3b54e-110">Type</span></span>|<span data-ttu-id="3b54e-111">说明</span><span class="sxs-lookup"><span data-stu-id="3b54e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b54e-112">inventoryCount</span><span class="sxs-lookup"><span data-stu-id="3b54e-112">inventoryCount</span></span>|<span data-ttu-id="3b54e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="3b54e-113">Int32</span></span>|<span data-ttu-id="3b54e-114">具有库存 swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="3b54e-114">Number of devices with Inventory swung-over.</span></span> <span data-ttu-id="3b54e-115">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3b54e-115">This property is read-only.</span></span>|
|<span data-ttu-id="3b54e-116">compliancePolicyCount</span><span class="sxs-lookup"><span data-stu-id="3b54e-116">compliancePolicyCount</span></span>|<span data-ttu-id="3b54e-117">Int32</span><span class="sxs-lookup"><span data-stu-id="3b54e-117">Int32</span></span>|<span data-ttu-id="3b54e-118">具有 CompliancePolicy swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="3b54e-118">Number of devices with CompliancePolicy swung-over.</span></span> <span data-ttu-id="3b54e-119">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3b54e-119">This property is read-only.</span></span>|
|<span data-ttu-id="3b54e-120">resourceAccessCount</span><span class="sxs-lookup"><span data-stu-id="3b54e-120">resourceAccessCount</span></span>|<span data-ttu-id="3b54e-121">Int32</span><span class="sxs-lookup"><span data-stu-id="3b54e-121">Int32</span></span>|<span data-ttu-id="3b54e-122">具有 ResourceAccess swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="3b54e-122">Number of devices with ResourceAccess swung-over.</span></span> <span data-ttu-id="3b54e-123">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3b54e-123">This property is read-only.</span></span>|
|<span data-ttu-id="3b54e-124">configurationSettingsCount</span><span class="sxs-lookup"><span data-stu-id="3b54e-124">configurationSettingsCount</span></span>|<span data-ttu-id="3b54e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="3b54e-125">Int32</span></span>|<span data-ttu-id="3b54e-126">具有 ConfigurationSettings swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="3b54e-126">Number of devices with ConfigurationSettings swung-over.</span></span> <span data-ttu-id="3b54e-127">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3b54e-127">This property is read-only.</span></span>|
|<span data-ttu-id="3b54e-128">windowsUpdateForBusinessCount</span><span class="sxs-lookup"><span data-stu-id="3b54e-128">windowsUpdateForBusinessCount</span></span>|<span data-ttu-id="3b54e-129">Int32</span><span class="sxs-lookup"><span data-stu-id="3b54e-129">Int32</span></span>|<span data-ttu-id="3b54e-130">具有 WindowsUpdateForBusiness swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="3b54e-130">Number of devices with WindowsUpdateForBusiness swung-over.</span></span> <span data-ttu-id="3b54e-131">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3b54e-131">This property is read-only.</span></span>|
|<span data-ttu-id="3b54e-132">endpointProtectionCount</span><span class="sxs-lookup"><span data-stu-id="3b54e-132">endpointProtectionCount</span></span>|<span data-ttu-id="3b54e-133">Int32</span><span class="sxs-lookup"><span data-stu-id="3b54e-133">Int32</span></span>|<span data-ttu-id="3b54e-134">具有 EndpointProtection swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="3b54e-134">Number of devices with EndpointProtection swung-over.</span></span> <span data-ttu-id="3b54e-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3b54e-135">This property is read-only.</span></span>|
|<span data-ttu-id="3b54e-136">modernAppsCount</span><span class="sxs-lookup"><span data-stu-id="3b54e-136">modernAppsCount</span></span>|<span data-ttu-id="3b54e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3b54e-137">Int32</span></span>|<span data-ttu-id="3b54e-138">具有 ModernApps swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="3b54e-138">Number of devices with ModernApps swung-over.</span></span> <span data-ttu-id="3b54e-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3b54e-139">This property is read-only.</span></span>|
|<span data-ttu-id="3b54e-140">officeAppsCount</span><span class="sxs-lookup"><span data-stu-id="3b54e-140">officeAppsCount</span></span>|<span data-ttu-id="3b54e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="3b54e-141">Int32</span></span>|<span data-ttu-id="3b54e-142">具有 Officeoffice swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="3b54e-142">Number of devices with OfficeApps swung-over.</span></span> <span data-ttu-id="3b54e-143">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3b54e-143">This property is read-only.</span></span>|
|<span data-ttu-id="3b54e-144">totalComanagedCount</span><span class="sxs-lookup"><span data-stu-id="3b54e-144">totalComanagedCount</span></span>|<span data-ttu-id="3b54e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="3b54e-145">Int32</span></span>|<span data-ttu-id="3b54e-146">共同管理的设备的数量。</span><span class="sxs-lookup"><span data-stu-id="3b54e-146">Number of Co-Managed Devices.</span></span> <span data-ttu-id="3b54e-147">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3b54e-147">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b54e-148">关系</span><span class="sxs-lookup"><span data-stu-id="3b54e-148">Relationships</span></span>
<span data-ttu-id="3b54e-149">无</span><span class="sxs-lookup"><span data-stu-id="3b54e-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b54e-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b54e-150">JSON Representation</span></span>
<span data-ttu-id="3b54e-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b54e-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagedDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagedDevicesSummary",
  "inventoryCount": 1024,
  "compliancePolicyCount": 1024,
  "resourceAccessCount": 1024,
  "configurationSettingsCount": 1024,
  "windowsUpdateForBusinessCount": 1024,
  "endpointProtectionCount": 1024,
  "modernAppsCount": 1024,
  "officeAppsCount": 1024,
  "totalComanagedCount": 1024
}
```






