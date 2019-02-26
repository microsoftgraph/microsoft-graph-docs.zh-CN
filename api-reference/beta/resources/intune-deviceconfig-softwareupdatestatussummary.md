---
title: softwareUpdateStatusSummary 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17314b5e37af0677c5e78dba9349695346b43d6a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161080"
---
# <a name="softwareupdatestatussummary-resource-type"></a><span data-ttu-id="314ba-103">softwareUpdateStatusSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="314ba-103">softwareUpdateStatusSummary resource type</span></span>

> <span data-ttu-id="314ba-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="314ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="314ba-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="314ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="314ba-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="314ba-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="314ba-107">方法</span><span class="sxs-lookup"><span data-stu-id="314ba-107">Methods</span></span>
|<span data-ttu-id="314ba-108">方法</span><span class="sxs-lookup"><span data-stu-id="314ba-108">Method</span></span>|<span data-ttu-id="314ba-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="314ba-109">Return Type</span></span>|<span data-ttu-id="314ba-110">说明</span><span class="sxs-lookup"><span data-stu-id="314ba-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="314ba-111">获取 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="314ba-111">Get softwareUpdateStatusSummary</span></span>](../api/intune-deviceconfig-softwareupdatestatussummary-get.md)|[<span data-ttu-id="314ba-112">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="314ba-112">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="314ba-113">读取 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="314ba-113">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>|
|[<span data-ttu-id="314ba-114">更新 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="314ba-114">Update softwareUpdateStatusSummary</span></span>](../api/intune-deviceconfig-softwareupdatestatussummary-update.md)|[<span data-ttu-id="314ba-115">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="314ba-115">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="314ba-116">更新 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="314ba-116">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="314ba-117">属性</span><span class="sxs-lookup"><span data-stu-id="314ba-117">Properties</span></span>
|<span data-ttu-id="314ba-118">属性</span><span class="sxs-lookup"><span data-stu-id="314ba-118">Property</span></span>|<span data-ttu-id="314ba-119">类型</span><span class="sxs-lookup"><span data-stu-id="314ba-119">Type</span></span>|<span data-ttu-id="314ba-120">说明</span><span class="sxs-lookup"><span data-stu-id="314ba-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="314ba-121">id</span><span class="sxs-lookup"><span data-stu-id="314ba-121">id</span></span>|<span data-ttu-id="314ba-122">String</span><span class="sxs-lookup"><span data-stu-id="314ba-122">String</span></span>|<span data-ttu-id="314ba-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="314ba-123">Key of the entity.</span></span>|
|<span data-ttu-id="314ba-124">displayName</span><span class="sxs-lookup"><span data-stu-id="314ba-124">displayName</span></span>|<span data-ttu-id="314ba-125">String</span><span class="sxs-lookup"><span data-stu-id="314ba-125">String</span></span>|<span data-ttu-id="314ba-126">策略的名称。</span><span class="sxs-lookup"><span data-stu-id="314ba-126">The name of the policy.</span></span>|
|<span data-ttu-id="314ba-127">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="314ba-127">compliantDeviceCount</span></span>|<span data-ttu-id="314ba-128">Int32</span><span class="sxs-lookup"><span data-stu-id="314ba-128">Int32</span></span>|<span data-ttu-id="314ba-129">兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="314ba-129">Number of compliant devices.</span></span>|
|<span data-ttu-id="314ba-130">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="314ba-130">nonCompliantDeviceCount</span></span>|<span data-ttu-id="314ba-131">Int32</span><span class="sxs-lookup"><span data-stu-id="314ba-131">Int32</span></span>|<span data-ttu-id="314ba-132">不兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="314ba-132">Number of non compliant devices.</span></span>|
|<span data-ttu-id="314ba-133">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="314ba-133">remediatedDeviceCount</span></span>|<span data-ttu-id="314ba-134">Int32</span><span class="sxs-lookup"><span data-stu-id="314ba-134">Int32</span></span>|<span data-ttu-id="314ba-135">已修复设备的数量。</span><span class="sxs-lookup"><span data-stu-id="314ba-135">Number of remediated devices.</span></span>|
|<span data-ttu-id="314ba-136">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="314ba-136">errorDeviceCount</span></span>|<span data-ttu-id="314ba-137">Int32</span><span class="sxs-lookup"><span data-stu-id="314ba-137">Int32</span></span>|<span data-ttu-id="314ba-138">出现错误的设备数量。</span><span class="sxs-lookup"><span data-stu-id="314ba-138">Number of devices had error.</span></span>|
|<span data-ttu-id="314ba-139">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="314ba-139">unknownDeviceCount</span></span>|<span data-ttu-id="314ba-140">Int32</span><span class="sxs-lookup"><span data-stu-id="314ba-140">Int32</span></span>|<span data-ttu-id="314ba-141">未知设备的数量。</span><span class="sxs-lookup"><span data-stu-id="314ba-141">Number of unknown devices.</span></span>|
|<span data-ttu-id="314ba-142">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="314ba-142">conflictDeviceCount</span></span>|<span data-ttu-id="314ba-143">Int32</span><span class="sxs-lookup"><span data-stu-id="314ba-143">Int32</span></span>|<span data-ttu-id="314ba-144">冲突设备的数量。</span><span class="sxs-lookup"><span data-stu-id="314ba-144">Number of conflict devices.</span></span>|
|<span data-ttu-id="314ba-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="314ba-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="314ba-146">Int32</span><span class="sxs-lookup"><span data-stu-id="314ba-146">Int32</span></span>|<span data-ttu-id="314ba-147">不适用设备的数量。</span><span class="sxs-lookup"><span data-stu-id="314ba-147">Number of not applicable devices.</span></span>|
|<span data-ttu-id="314ba-148">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="314ba-148">compliantUserCount</span></span>|<span data-ttu-id="314ba-149">Int32</span><span class="sxs-lookup"><span data-stu-id="314ba-149">Int32</span></span>|<span data-ttu-id="314ba-150">兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="314ba-150">Number of compliant users.</span></span>|
|<span data-ttu-id="314ba-151">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="314ba-151">nonCompliantUserCount</span></span>|<span data-ttu-id="314ba-152">Int32</span><span class="sxs-lookup"><span data-stu-id="314ba-152">Int32</span></span>|<span data-ttu-id="314ba-153">不兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="314ba-153">Number of non compliant users.</span></span>|
|<span data-ttu-id="314ba-154">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="314ba-154">remediatedUserCount</span></span>|<span data-ttu-id="314ba-155">Int32</span><span class="sxs-lookup"><span data-stu-id="314ba-155">Int32</span></span>|<span data-ttu-id="314ba-156">已修复用户的数量。</span><span class="sxs-lookup"><span data-stu-id="314ba-156">Number of remediated users.</span></span>|
|<span data-ttu-id="314ba-157">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="314ba-157">errorUserCount</span></span>|<span data-ttu-id="314ba-158">Int32</span><span class="sxs-lookup"><span data-stu-id="314ba-158">Int32</span></span>|<span data-ttu-id="314ba-159">出现错误的用户数量。</span><span class="sxs-lookup"><span data-stu-id="314ba-159">Number of users had error.</span></span>|
|<span data-ttu-id="314ba-160">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="314ba-160">unknownUserCount</span></span>|<span data-ttu-id="314ba-161">Int32</span><span class="sxs-lookup"><span data-stu-id="314ba-161">Int32</span></span>|<span data-ttu-id="314ba-162">未知用户的数量。</span><span class="sxs-lookup"><span data-stu-id="314ba-162">Number of unknown users.</span></span>|
|<span data-ttu-id="314ba-163">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="314ba-163">conflictUserCount</span></span>|<span data-ttu-id="314ba-164">Int32</span><span class="sxs-lookup"><span data-stu-id="314ba-164">Int32</span></span>|<span data-ttu-id="314ba-165">冲突用户的数量。</span><span class="sxs-lookup"><span data-stu-id="314ba-165">Number of conflict users.</span></span>|
|<span data-ttu-id="314ba-166">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="314ba-166">notApplicableUserCount</span></span>|<span data-ttu-id="314ba-167">Int32</span><span class="sxs-lookup"><span data-stu-id="314ba-167">Int32</span></span>|<span data-ttu-id="314ba-168">不适用用户的数量。</span><span class="sxs-lookup"><span data-stu-id="314ba-168">Number of not applicable users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="314ba-169">关系</span><span class="sxs-lookup"><span data-stu-id="314ba-169">Relationships</span></span>
<span data-ttu-id="314ba-170">无</span><span class="sxs-lookup"><span data-stu-id="314ba-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="314ba-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="314ba-171">JSON Representation</span></span>
<span data-ttu-id="314ba-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="314ba-172">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "errorUserCount": 1024,
  "unknownUserCount": 1024,
  "conflictUserCount": 1024,
  "notApplicableUserCount": 1024
}
```




