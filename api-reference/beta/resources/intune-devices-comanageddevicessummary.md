---
title: comanagedDevicesSummary 资源类型
description: Co 托管设备的摘要数据
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f592ba7900f0761a24b02495dc337046b615bb1
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793463"
---
# <a name="comanageddevicessummary-resource-type"></a><span data-ttu-id="f1e1a-103">comanagedDevicesSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1e1a-103">comanagedDevicesSummary resource type</span></span>

<span data-ttu-id="f1e1a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1e1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1e1a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1e1a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1e1a-107">Co 托管设备的摘要数据</span><span class="sxs-lookup"><span data-stu-id="f1e1a-107">Summary data for co managed devices</span></span>

## <a name="properties"></a><span data-ttu-id="f1e1a-108">属性</span><span class="sxs-lookup"><span data-stu-id="f1e1a-108">Properties</span></span>
|<span data-ttu-id="f1e1a-109">属性</span><span class="sxs-lookup"><span data-stu-id="f1e1a-109">Property</span></span>|<span data-ttu-id="f1e1a-110">类型</span><span class="sxs-lookup"><span data-stu-id="f1e1a-110">Type</span></span>|<span data-ttu-id="f1e1a-111">说明</span><span class="sxs-lookup"><span data-stu-id="f1e1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1e1a-112">inventoryCount</span><span class="sxs-lookup"><span data-stu-id="f1e1a-112">inventoryCount</span></span>|<span data-ttu-id="f1e1a-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e1a-113">Int32</span></span>|<span data-ttu-id="f1e1a-114">具有库存 swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-114">Number of devices with Inventory swung-over.</span></span> <span data-ttu-id="f1e1a-115">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-115">This property is read-only.</span></span>|
|<span data-ttu-id="f1e1a-116">compliancePolicyCount</span><span class="sxs-lookup"><span data-stu-id="f1e1a-116">compliancePolicyCount</span></span>|<span data-ttu-id="f1e1a-117">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e1a-117">Int32</span></span>|<span data-ttu-id="f1e1a-118">具有 CompliancePolicy swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-118">Number of devices with CompliancePolicy swung-over.</span></span> <span data-ttu-id="f1e1a-119">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-119">This property is read-only.</span></span>|
|<span data-ttu-id="f1e1a-120">resourceAccessCount</span><span class="sxs-lookup"><span data-stu-id="f1e1a-120">resourceAccessCount</span></span>|<span data-ttu-id="f1e1a-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e1a-121">Int32</span></span>|<span data-ttu-id="f1e1a-122">具有 ResourceAccess swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-122">Number of devices with ResourceAccess swung-over.</span></span> <span data-ttu-id="f1e1a-123">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-123">This property is read-only.</span></span>|
|<span data-ttu-id="f1e1a-124">configurationSettingsCount</span><span class="sxs-lookup"><span data-stu-id="f1e1a-124">configurationSettingsCount</span></span>|<span data-ttu-id="f1e1a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e1a-125">Int32</span></span>|<span data-ttu-id="f1e1a-126">具有 ConfigurationSettings swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-126">Number of devices with ConfigurationSettings swung-over.</span></span> <span data-ttu-id="f1e1a-127">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-127">This property is read-only.</span></span>|
|<span data-ttu-id="f1e1a-128">windowsUpdateForBusinessCount</span><span class="sxs-lookup"><span data-stu-id="f1e1a-128">windowsUpdateForBusinessCount</span></span>|<span data-ttu-id="f1e1a-129">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e1a-129">Int32</span></span>|<span data-ttu-id="f1e1a-130">具有 WindowsUpdateForBusiness swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-130">Number of devices with WindowsUpdateForBusiness swung-over.</span></span> <span data-ttu-id="f1e1a-131">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-131">This property is read-only.</span></span>|
|<span data-ttu-id="f1e1a-132">endpointProtectionCount</span><span class="sxs-lookup"><span data-stu-id="f1e1a-132">endpointProtectionCount</span></span>|<span data-ttu-id="f1e1a-133">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e1a-133">Int32</span></span>|<span data-ttu-id="f1e1a-134">具有 EndpointProtection swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-134">Number of devices with EndpointProtection swung-over.</span></span> <span data-ttu-id="f1e1a-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-135">This property is read-only.</span></span>|
|<span data-ttu-id="f1e1a-136">modernAppsCount</span><span class="sxs-lookup"><span data-stu-id="f1e1a-136">modernAppsCount</span></span>|<span data-ttu-id="f1e1a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e1a-137">Int32</span></span>|<span data-ttu-id="f1e1a-138">具有 ModernApps swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-138">Number of devices with ModernApps swung-over.</span></span> <span data-ttu-id="f1e1a-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-139">This property is read-only.</span></span>|
|<span data-ttu-id="f1e1a-140">officeAppsCount</span><span class="sxs-lookup"><span data-stu-id="f1e1a-140">officeAppsCount</span></span>|<span data-ttu-id="f1e1a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e1a-141">Int32</span></span>|<span data-ttu-id="f1e1a-142">具有 Officeoffice swung 的设备数量。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-142">Number of devices with OfficeApps swung-over.</span></span> <span data-ttu-id="f1e1a-143">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-143">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1e1a-144">关系</span><span class="sxs-lookup"><span data-stu-id="f1e1a-144">Relationships</span></span>
<span data-ttu-id="f1e1a-145">无</span><span class="sxs-lookup"><span data-stu-id="f1e1a-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1e1a-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1e1a-146">JSON Representation</span></span>
<span data-ttu-id="f1e1a-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1e1a-147">Here is a JSON representation of the resource.</span></span>
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
  "officeAppsCount": 1024
}
```



