---
title: comanagedDevicesSummary 资源类型
description: Co 托管设备的摘要数据
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e12a946db3e568faa171fa53299e6ec3546d455
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791790"
---
# <a name="comanageddevicessummary-resource-type"></a><span data-ttu-id="c1db7-103">comanagedDevicesSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1db7-103">comanagedDevicesSummary resource type</span></span>

<span data-ttu-id="c1db7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1db7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1db7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c1db7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1db7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1db7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1db7-107">Co 托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="c1db7-107">Summary data for co managed devices</span></span>

## <a name="properties"></a><span data-ttu-id="c1db7-108">属性</span><span class="sxs-lookup"><span data-stu-id="c1db7-108">Properties</span></span>
|<span data-ttu-id="c1db7-109">属性</span><span class="sxs-lookup"><span data-stu-id="c1db7-109">Property</span></span>|<span data-ttu-id="c1db7-110">类型</span><span class="sxs-lookup"><span data-stu-id="c1db7-110">Type</span></span>|<span data-ttu-id="c1db7-111">说明</span><span class="sxs-lookup"><span data-stu-id="c1db7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1db7-112">inventoryCount</span><span class="sxs-lookup"><span data-stu-id="c1db7-112">inventoryCount</span></span>|<span data-ttu-id="c1db7-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c1db7-113">Int32</span></span>|<span data-ttu-id="c1db7-114">具有库存 swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="c1db7-114">Number of devices with Inventory swung-over.</span></span> <span data-ttu-id="c1db7-115">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c1db7-115">This property is read-only.</span></span>|
|<span data-ttu-id="c1db7-116">compliancePolicyCount</span><span class="sxs-lookup"><span data-stu-id="c1db7-116">compliancePolicyCount</span></span>|<span data-ttu-id="c1db7-117">Int32</span><span class="sxs-lookup"><span data-stu-id="c1db7-117">Int32</span></span>|<span data-ttu-id="c1db7-118">具有 CompliancePolicy swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="c1db7-118">Number of devices with CompliancePolicy swung-over.</span></span> <span data-ttu-id="c1db7-119">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c1db7-119">This property is read-only.</span></span>|
|<span data-ttu-id="c1db7-120">resourceAccessCount</span><span class="sxs-lookup"><span data-stu-id="c1db7-120">resourceAccessCount</span></span>|<span data-ttu-id="c1db7-121">Int32</span><span class="sxs-lookup"><span data-stu-id="c1db7-121">Int32</span></span>|<span data-ttu-id="c1db7-122">具有 ResourceAccess swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="c1db7-122">Number of devices with ResourceAccess swung-over.</span></span> <span data-ttu-id="c1db7-123">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c1db7-123">This property is read-only.</span></span>|
|<span data-ttu-id="c1db7-124">configurationSettingsCount</span><span class="sxs-lookup"><span data-stu-id="c1db7-124">configurationSettingsCount</span></span>|<span data-ttu-id="c1db7-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c1db7-125">Int32</span></span>|<span data-ttu-id="c1db7-126">具有 ConfigurationSettings swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="c1db7-126">Number of devices with ConfigurationSettings swung-over.</span></span> <span data-ttu-id="c1db7-127">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c1db7-127">This property is read-only.</span></span>|
|<span data-ttu-id="c1db7-128">windowsUpdateForBusinessCount</span><span class="sxs-lookup"><span data-stu-id="c1db7-128">windowsUpdateForBusinessCount</span></span>|<span data-ttu-id="c1db7-129">Int32</span><span class="sxs-lookup"><span data-stu-id="c1db7-129">Int32</span></span>|<span data-ttu-id="c1db7-130">具有 WindowsUpdateForBusiness swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="c1db7-130">Number of devices with WindowsUpdateForBusiness swung-over.</span></span> <span data-ttu-id="c1db7-131">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c1db7-131">This property is read-only.</span></span>|
|<span data-ttu-id="c1db7-132">endpointProtectionCount</span><span class="sxs-lookup"><span data-stu-id="c1db7-132">endpointProtectionCount</span></span>|<span data-ttu-id="c1db7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="c1db7-133">Int32</span></span>|<span data-ttu-id="c1db7-134">具有 EndpointProtection swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="c1db7-134">Number of devices with EndpointProtection swung-over.</span></span> <span data-ttu-id="c1db7-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c1db7-135">This property is read-only.</span></span>|
|<span data-ttu-id="c1db7-136">modernAppsCount</span><span class="sxs-lookup"><span data-stu-id="c1db7-136">modernAppsCount</span></span>|<span data-ttu-id="c1db7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c1db7-137">Int32</span></span>|<span data-ttu-id="c1db7-138">具有 ModernApps swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="c1db7-138">Number of devices with ModernApps swung-over.</span></span> <span data-ttu-id="c1db7-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c1db7-139">This property is read-only.</span></span>|
|<span data-ttu-id="c1db7-140">officeAppsCount</span><span class="sxs-lookup"><span data-stu-id="c1db7-140">officeAppsCount</span></span>|<span data-ttu-id="c1db7-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c1db7-141">Int32</span></span>|<span data-ttu-id="c1db7-142">具有 Officeoffice swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="c1db7-142">Number of devices with OfficeApps swung-over.</span></span> <span data-ttu-id="c1db7-143">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c1db7-143">This property is read-only.</span></span>|
|<span data-ttu-id="c1db7-144">totalComanagedCount</span><span class="sxs-lookup"><span data-stu-id="c1db7-144">totalComanagedCount</span></span>|<span data-ttu-id="c1db7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="c1db7-145">Int32</span></span>|<span data-ttu-id="c1db7-146">共同管理的设备的数量。</span><span class="sxs-lookup"><span data-stu-id="c1db7-146">Number of Co-Managed Devices.</span></span> <span data-ttu-id="c1db7-147">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c1db7-147">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1db7-148">关系</span><span class="sxs-lookup"><span data-stu-id="c1db7-148">Relationships</span></span>
<span data-ttu-id="c1db7-149">无</span><span class="sxs-lookup"><span data-stu-id="c1db7-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1db7-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1db7-150">JSON Representation</span></span>
<span data-ttu-id="c1db7-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1db7-151">Here is a JSON representation of the resource.</span></span>
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



