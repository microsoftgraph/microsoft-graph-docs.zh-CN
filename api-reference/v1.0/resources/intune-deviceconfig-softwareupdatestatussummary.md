---
title: softwareUpdateStatusSummary 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc66eb63e4f48a2b60303a9f868cb74c2ee52fbd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263474"
---
# <a name="softwareupdatestatussummary-resource-type"></a><span data-ttu-id="4d03f-103">softwareUpdateStatusSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d03f-103">softwareUpdateStatusSummary resource type</span></span>

> <span data-ttu-id="4d03f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d03f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d03f-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4d03f-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="4d03f-106">方法</span><span class="sxs-lookup"><span data-stu-id="4d03f-106">Methods</span></span>
|<span data-ttu-id="4d03f-107">方法</span><span class="sxs-lookup"><span data-stu-id="4d03f-107">Method</span></span>|<span data-ttu-id="4d03f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4d03f-108">Return Type</span></span>|<span data-ttu-id="4d03f-109">说明</span><span class="sxs-lookup"><span data-stu-id="4d03f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4d03f-110">获取 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="4d03f-110">Get softwareUpdateStatusSummary</span></span>](../api/intune-deviceconfig-softwareupdatestatussummary-get.md)|[<span data-ttu-id="4d03f-111">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="4d03f-111">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="4d03f-112">读取 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4d03f-112">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>|
|[<span data-ttu-id="4d03f-113">更新 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="4d03f-113">Update softwareUpdateStatusSummary</span></span>](../api/intune-deviceconfig-softwareupdatestatussummary-update.md)|[<span data-ttu-id="4d03f-114">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="4d03f-114">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="4d03f-115">更新 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4d03f-115">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4d03f-116">属性</span><span class="sxs-lookup"><span data-stu-id="4d03f-116">Properties</span></span>
|<span data-ttu-id="4d03f-117">属性</span><span class="sxs-lookup"><span data-stu-id="4d03f-117">Property</span></span>|<span data-ttu-id="4d03f-118">类型</span><span class="sxs-lookup"><span data-stu-id="4d03f-118">Type</span></span>|<span data-ttu-id="4d03f-119">说明</span><span class="sxs-lookup"><span data-stu-id="4d03f-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d03f-120">id</span><span class="sxs-lookup"><span data-stu-id="4d03f-120">id</span></span>|<span data-ttu-id="4d03f-121">String</span><span class="sxs-lookup"><span data-stu-id="4d03f-121">String</span></span>|<span data-ttu-id="4d03f-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4d03f-122">Key of the entity.</span></span>|
|<span data-ttu-id="4d03f-123">displayName</span><span class="sxs-lookup"><span data-stu-id="4d03f-123">displayName</span></span>|<span data-ttu-id="4d03f-124">String</span><span class="sxs-lookup"><span data-stu-id="4d03f-124">String</span></span>|<span data-ttu-id="4d03f-125">策略的名称。</span><span class="sxs-lookup"><span data-stu-id="4d03f-125">The name of the policy.</span></span>|
|<span data-ttu-id="4d03f-126">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4d03f-126">compliantDeviceCount</span></span>|<span data-ttu-id="4d03f-127">Int32</span><span class="sxs-lookup"><span data-stu-id="4d03f-127">Int32</span></span>|<span data-ttu-id="4d03f-128">兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="4d03f-128">Number of compliant devices.</span></span>|
|<span data-ttu-id="4d03f-129">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4d03f-129">nonCompliantDeviceCount</span></span>|<span data-ttu-id="4d03f-130">Int32</span><span class="sxs-lookup"><span data-stu-id="4d03f-130">Int32</span></span>|<span data-ttu-id="4d03f-131">不兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="4d03f-131">Number of non compliant devices.</span></span>|
|<span data-ttu-id="4d03f-132">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4d03f-132">remediatedDeviceCount</span></span>|<span data-ttu-id="4d03f-133">Int32</span><span class="sxs-lookup"><span data-stu-id="4d03f-133">Int32</span></span>|<span data-ttu-id="4d03f-134">已修复设备的数量。</span><span class="sxs-lookup"><span data-stu-id="4d03f-134">Number of remediated devices.</span></span>|
|<span data-ttu-id="4d03f-135">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4d03f-135">errorDeviceCount</span></span>|<span data-ttu-id="4d03f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4d03f-136">Int32</span></span>|<span data-ttu-id="4d03f-137">出现错误的设备数量。</span><span class="sxs-lookup"><span data-stu-id="4d03f-137">Number of devices had error.</span></span>|
|<span data-ttu-id="4d03f-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4d03f-138">unknownDeviceCount</span></span>|<span data-ttu-id="4d03f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4d03f-139">Int32</span></span>|<span data-ttu-id="4d03f-140">未知设备的数量。</span><span class="sxs-lookup"><span data-stu-id="4d03f-140">Number of unknown devices.</span></span>|
|<span data-ttu-id="4d03f-141">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4d03f-141">conflictDeviceCount</span></span>|<span data-ttu-id="4d03f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4d03f-142">Int32</span></span>|<span data-ttu-id="4d03f-143">冲突设备的数量。</span><span class="sxs-lookup"><span data-stu-id="4d03f-143">Number of conflict devices.</span></span>|
|<span data-ttu-id="4d03f-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4d03f-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="4d03f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="4d03f-145">Int32</span></span>|<span data-ttu-id="4d03f-146">不适用设备的数量。</span><span class="sxs-lookup"><span data-stu-id="4d03f-146">Number of not applicable devices.</span></span>|
|<span data-ttu-id="4d03f-147">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="4d03f-147">compliantUserCount</span></span>|<span data-ttu-id="4d03f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4d03f-148">Int32</span></span>|<span data-ttu-id="4d03f-149">兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="4d03f-149">Number of compliant users.</span></span>|
|<span data-ttu-id="4d03f-150">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="4d03f-150">nonCompliantUserCount</span></span>|<span data-ttu-id="4d03f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="4d03f-151">Int32</span></span>|<span data-ttu-id="4d03f-152">不兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="4d03f-152">Number of non compliant users.</span></span>|
|<span data-ttu-id="4d03f-153">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="4d03f-153">remediatedUserCount</span></span>|<span data-ttu-id="4d03f-154">Int32</span><span class="sxs-lookup"><span data-stu-id="4d03f-154">Int32</span></span>|<span data-ttu-id="4d03f-155">已修复用户的数量。</span><span class="sxs-lookup"><span data-stu-id="4d03f-155">Number of remediated users.</span></span>|
|<span data-ttu-id="4d03f-156">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="4d03f-156">errorUserCount</span></span>|<span data-ttu-id="4d03f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4d03f-157">Int32</span></span>|<span data-ttu-id="4d03f-158">出现错误的用户数量。</span><span class="sxs-lookup"><span data-stu-id="4d03f-158">Number of users had error.</span></span>|
|<span data-ttu-id="4d03f-159">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="4d03f-159">unknownUserCount</span></span>|<span data-ttu-id="4d03f-160">Int32</span><span class="sxs-lookup"><span data-stu-id="4d03f-160">Int32</span></span>|<span data-ttu-id="4d03f-161">未知用户的数量。</span><span class="sxs-lookup"><span data-stu-id="4d03f-161">Number of unknown users.</span></span>|
|<span data-ttu-id="4d03f-162">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="4d03f-162">conflictUserCount</span></span>|<span data-ttu-id="4d03f-163">Int32</span><span class="sxs-lookup"><span data-stu-id="4d03f-163">Int32</span></span>|<span data-ttu-id="4d03f-164">冲突用户的数量。</span><span class="sxs-lookup"><span data-stu-id="4d03f-164">Number of conflict users.</span></span>|
|<span data-ttu-id="4d03f-165">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="4d03f-165">notApplicableUserCount</span></span>|<span data-ttu-id="4d03f-166">Int32</span><span class="sxs-lookup"><span data-stu-id="4d03f-166">Int32</span></span>|<span data-ttu-id="4d03f-167">不适用用户的数量。</span><span class="sxs-lookup"><span data-stu-id="4d03f-167">Number of not applicable users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d03f-168">关系</span><span class="sxs-lookup"><span data-stu-id="4d03f-168">Relationships</span></span>
<span data-ttu-id="4d03f-169">无</span><span class="sxs-lookup"><span data-stu-id="4d03f-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d03f-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d03f-170">JSON Representation</span></span>
<span data-ttu-id="4d03f-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d03f-171">Here is a JSON representation of the resource.</span></span>
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



