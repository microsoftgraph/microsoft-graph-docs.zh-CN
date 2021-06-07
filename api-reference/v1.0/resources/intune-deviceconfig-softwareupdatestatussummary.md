---
title: softwareUpdateStatusSummary 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3f70e091bc39b8591d59c2904a1e9ad743fcffa1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758797"
---
# <a name="softwareupdatestatussummary-resource-type"></a><span data-ttu-id="a2476-103">softwareUpdateStatusSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2476-103">softwareUpdateStatusSummary resource type</span></span>

<span data-ttu-id="a2476-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2476-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2476-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2476-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2476-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a2476-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="a2476-107">方法</span><span class="sxs-lookup"><span data-stu-id="a2476-107">Methods</span></span>
|<span data-ttu-id="a2476-108">方法</span><span class="sxs-lookup"><span data-stu-id="a2476-108">Method</span></span>|<span data-ttu-id="a2476-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a2476-109">Return Type</span></span>|<span data-ttu-id="a2476-110">说明</span><span class="sxs-lookup"><span data-stu-id="a2476-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a2476-111">获取 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="a2476-111">Get softwareUpdateStatusSummary</span></span>](../api/intune-deviceconfig-softwareupdatestatussummary-get.md)|[<span data-ttu-id="a2476-112">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="a2476-112">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="a2476-113">读取 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a2476-113">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>|
|[<span data-ttu-id="a2476-114">更新 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="a2476-114">Update softwareUpdateStatusSummary</span></span>](../api/intune-deviceconfig-softwareupdatestatussummary-update.md)|[<span data-ttu-id="a2476-115">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="a2476-115">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="a2476-116">更新 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a2476-116">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a2476-117">属性</span><span class="sxs-lookup"><span data-stu-id="a2476-117">Properties</span></span>
|<span data-ttu-id="a2476-118">属性</span><span class="sxs-lookup"><span data-stu-id="a2476-118">Property</span></span>|<span data-ttu-id="a2476-119">类型</span><span class="sxs-lookup"><span data-stu-id="a2476-119">Type</span></span>|<span data-ttu-id="a2476-120">说明</span><span class="sxs-lookup"><span data-stu-id="a2476-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2476-121">id</span><span class="sxs-lookup"><span data-stu-id="a2476-121">id</span></span>|<span data-ttu-id="a2476-122">String</span><span class="sxs-lookup"><span data-stu-id="a2476-122">String</span></span>|<span data-ttu-id="a2476-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a2476-123">Key of the entity.</span></span>|
|<span data-ttu-id="a2476-124">displayName</span><span class="sxs-lookup"><span data-stu-id="a2476-124">displayName</span></span>|<span data-ttu-id="a2476-125">String</span><span class="sxs-lookup"><span data-stu-id="a2476-125">String</span></span>|<span data-ttu-id="a2476-126">策略的名称。</span><span class="sxs-lookup"><span data-stu-id="a2476-126">The name of the policy.</span></span>|
|<span data-ttu-id="a2476-127">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a2476-127">compliantDeviceCount</span></span>|<span data-ttu-id="a2476-128">Int32</span><span class="sxs-lookup"><span data-stu-id="a2476-128">Int32</span></span>|<span data-ttu-id="a2476-129">兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="a2476-129">Number of compliant devices.</span></span>|
|<span data-ttu-id="a2476-130">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a2476-130">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a2476-131">Int32</span><span class="sxs-lookup"><span data-stu-id="a2476-131">Int32</span></span>|<span data-ttu-id="a2476-132">不兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="a2476-132">Number of non compliant devices.</span></span>|
|<span data-ttu-id="a2476-133">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a2476-133">remediatedDeviceCount</span></span>|<span data-ttu-id="a2476-134">Int32</span><span class="sxs-lookup"><span data-stu-id="a2476-134">Int32</span></span>|<span data-ttu-id="a2476-135">已修复设备的数量。</span><span class="sxs-lookup"><span data-stu-id="a2476-135">Number of remediated devices.</span></span>|
|<span data-ttu-id="a2476-136">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a2476-136">errorDeviceCount</span></span>|<span data-ttu-id="a2476-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a2476-137">Int32</span></span>|<span data-ttu-id="a2476-138">出现错误的设备数量。</span><span class="sxs-lookup"><span data-stu-id="a2476-138">Number of devices had error.</span></span>|
|<span data-ttu-id="a2476-139">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a2476-139">unknownDeviceCount</span></span>|<span data-ttu-id="a2476-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a2476-140">Int32</span></span>|<span data-ttu-id="a2476-141">未知设备的数量。</span><span class="sxs-lookup"><span data-stu-id="a2476-141">Number of unknown devices.</span></span>|
|<span data-ttu-id="a2476-142">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a2476-142">conflictDeviceCount</span></span>|<span data-ttu-id="a2476-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a2476-143">Int32</span></span>|<span data-ttu-id="a2476-144">冲突设备的数量。</span><span class="sxs-lookup"><span data-stu-id="a2476-144">Number of conflict devices.</span></span>|
|<span data-ttu-id="a2476-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a2476-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="a2476-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a2476-146">Int32</span></span>|<span data-ttu-id="a2476-147">不适用设备的数量。</span><span class="sxs-lookup"><span data-stu-id="a2476-147">Number of not applicable devices.</span></span>|
|<span data-ttu-id="a2476-148">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="a2476-148">compliantUserCount</span></span>|<span data-ttu-id="a2476-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a2476-149">Int32</span></span>|<span data-ttu-id="a2476-150">兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="a2476-150">Number of compliant users.</span></span>|
|<span data-ttu-id="a2476-151">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="a2476-151">nonCompliantUserCount</span></span>|<span data-ttu-id="a2476-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a2476-152">Int32</span></span>|<span data-ttu-id="a2476-153">不兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="a2476-153">Number of non compliant users.</span></span>|
|<span data-ttu-id="a2476-154">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="a2476-154">remediatedUserCount</span></span>|<span data-ttu-id="a2476-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a2476-155">Int32</span></span>|<span data-ttu-id="a2476-156">已修复用户的数量。</span><span class="sxs-lookup"><span data-stu-id="a2476-156">Number of remediated users.</span></span>|
|<span data-ttu-id="a2476-157">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="a2476-157">errorUserCount</span></span>|<span data-ttu-id="a2476-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a2476-158">Int32</span></span>|<span data-ttu-id="a2476-159">出现错误的用户数量。</span><span class="sxs-lookup"><span data-stu-id="a2476-159">Number of users had error.</span></span>|
|<span data-ttu-id="a2476-160">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="a2476-160">unknownUserCount</span></span>|<span data-ttu-id="a2476-161">Int32</span><span class="sxs-lookup"><span data-stu-id="a2476-161">Int32</span></span>|<span data-ttu-id="a2476-162">未知用户的数量。</span><span class="sxs-lookup"><span data-stu-id="a2476-162">Number of unknown users.</span></span>|
|<span data-ttu-id="a2476-163">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="a2476-163">conflictUserCount</span></span>|<span data-ttu-id="a2476-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a2476-164">Int32</span></span>|<span data-ttu-id="a2476-165">冲突用户的数量。</span><span class="sxs-lookup"><span data-stu-id="a2476-165">Number of conflict users.</span></span>|
|<span data-ttu-id="a2476-166">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="a2476-166">notApplicableUserCount</span></span>|<span data-ttu-id="a2476-167">Int32</span><span class="sxs-lookup"><span data-stu-id="a2476-167">Int32</span></span>|<span data-ttu-id="a2476-168">不适用用户的数量。</span><span class="sxs-lookup"><span data-stu-id="a2476-168">Number of not applicable users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2476-169">关系</span><span class="sxs-lookup"><span data-stu-id="a2476-169">Relationships</span></span>
<span data-ttu-id="a2476-170">无</span><span class="sxs-lookup"><span data-stu-id="a2476-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2476-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2476-171">JSON Representation</span></span>
<span data-ttu-id="a2476-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2476-172">Here is a JSON representation of the resource.</span></span>
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




