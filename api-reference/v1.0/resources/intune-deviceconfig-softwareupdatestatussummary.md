---
title: softwareUpdateStatusSummary 资源类型
description: 尚未记录
ms.openlocfilehash: a090c9a88a72e03206c6eeb1f644ce31c88ef808
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007858"
---
# <a name="softwareupdatestatussummary-resource-type"></a><span data-ttu-id="5c330-103">softwareUpdateStatusSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c330-103">softwareUpdateStatusSummary resource type</span></span>

> <span data-ttu-id="5c330-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5c330-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c330-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5c330-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="5c330-106">方法</span><span class="sxs-lookup"><span data-stu-id="5c330-106">Methods</span></span>
|<span data-ttu-id="5c330-107">方法</span><span class="sxs-lookup"><span data-stu-id="5c330-107">Method</span></span>|<span data-ttu-id="5c330-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="5c330-108">Return Type</span></span>|<span data-ttu-id="5c330-109">说明</span><span class="sxs-lookup"><span data-stu-id="5c330-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5c330-110">获取 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="5c330-110">Get softwareUpdateStatusSummary</span></span>](../api/intune-deviceconfig-softwareupdatestatussummary-get.md)|[<span data-ttu-id="5c330-111">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="5c330-111">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="5c330-112">读取 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5c330-112">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>|
|[<span data-ttu-id="5c330-113">更新 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="5c330-113">Update softwareUpdateStatusSummary</span></span>](../api/intune-deviceconfig-softwareupdatestatussummary-update.md)|[<span data-ttu-id="5c330-114">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="5c330-114">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="5c330-115">更新 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5c330-115">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5c330-116">属性</span><span class="sxs-lookup"><span data-stu-id="5c330-116">Properties</span></span>
|<span data-ttu-id="5c330-117">属性</span><span class="sxs-lookup"><span data-stu-id="5c330-117">Property</span></span>|<span data-ttu-id="5c330-118">类型</span><span class="sxs-lookup"><span data-stu-id="5c330-118">Type</span></span>|<span data-ttu-id="5c330-119">说明</span><span class="sxs-lookup"><span data-stu-id="5c330-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c330-120">id</span><span class="sxs-lookup"><span data-stu-id="5c330-120">id</span></span>|<span data-ttu-id="5c330-121">String</span><span class="sxs-lookup"><span data-stu-id="5c330-121">String</span></span>|<span data-ttu-id="5c330-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5c330-122">Key of the entity.</span></span>|
|<span data-ttu-id="5c330-123">displayName</span><span class="sxs-lookup"><span data-stu-id="5c330-123">displayName</span></span>|<span data-ttu-id="5c330-124">String</span><span class="sxs-lookup"><span data-stu-id="5c330-124">String</span></span>|<span data-ttu-id="5c330-125">策略的名称。</span><span class="sxs-lookup"><span data-stu-id="5c330-125">The name of the policy.</span></span>|
|<span data-ttu-id="5c330-126">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c330-126">compliantDeviceCount</span></span>|<span data-ttu-id="5c330-127">Int32</span><span class="sxs-lookup"><span data-stu-id="5c330-127">Int32</span></span>|<span data-ttu-id="5c330-128">兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="5c330-128">Number of compliant devices.</span></span>|
|<span data-ttu-id="5c330-129">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c330-129">nonCompliantDeviceCount</span></span>|<span data-ttu-id="5c330-130">Int32</span><span class="sxs-lookup"><span data-stu-id="5c330-130">Int32</span></span>|<span data-ttu-id="5c330-131">不兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="5c330-131">Number of non compliant devices.</span></span>|
|<span data-ttu-id="5c330-132">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c330-132">remediatedDeviceCount</span></span>|<span data-ttu-id="5c330-133">Int32</span><span class="sxs-lookup"><span data-stu-id="5c330-133">Int32</span></span>|<span data-ttu-id="5c330-134">已修复设备的数量。</span><span class="sxs-lookup"><span data-stu-id="5c330-134">Number of remediated devices.</span></span>|
|<span data-ttu-id="5c330-135">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c330-135">errorDeviceCount</span></span>|<span data-ttu-id="5c330-136">Int32</span><span class="sxs-lookup"><span data-stu-id="5c330-136">Int32</span></span>|<span data-ttu-id="5c330-137">出现错误的设备数量。</span><span class="sxs-lookup"><span data-stu-id="5c330-137">Number of devices had error.</span></span>|
|<span data-ttu-id="5c330-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c330-138">unknownDeviceCount</span></span>|<span data-ttu-id="5c330-139">Int32</span><span class="sxs-lookup"><span data-stu-id="5c330-139">Int32</span></span>|<span data-ttu-id="5c330-140">未知设备的数量。</span><span class="sxs-lookup"><span data-stu-id="5c330-140">Number of unknown devices.</span></span>|
|<span data-ttu-id="5c330-141">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c330-141">conflictDeviceCount</span></span>|<span data-ttu-id="5c330-142">Int32</span><span class="sxs-lookup"><span data-stu-id="5c330-142">Int32</span></span>|<span data-ttu-id="5c330-143">冲突设备的数量。</span><span class="sxs-lookup"><span data-stu-id="5c330-143">Number of conflict devices.</span></span>|
|<span data-ttu-id="5c330-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c330-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="5c330-145">Int32</span><span class="sxs-lookup"><span data-stu-id="5c330-145">Int32</span></span>|<span data-ttu-id="5c330-146">不适用设备的数量。</span><span class="sxs-lookup"><span data-stu-id="5c330-146">Number of not applicable devices.</span></span>|
|<span data-ttu-id="5c330-147">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="5c330-147">compliantUserCount</span></span>|<span data-ttu-id="5c330-148">Int32</span><span class="sxs-lookup"><span data-stu-id="5c330-148">Int32</span></span>|<span data-ttu-id="5c330-149">兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="5c330-149">Number of compliant users.</span></span>|
|<span data-ttu-id="5c330-150">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="5c330-150">nonCompliantUserCount</span></span>|<span data-ttu-id="5c330-151">Int32</span><span class="sxs-lookup"><span data-stu-id="5c330-151">Int32</span></span>|<span data-ttu-id="5c330-152">不兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="5c330-152">Number of non compliant users.</span></span>|
|<span data-ttu-id="5c330-153">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="5c330-153">remediatedUserCount</span></span>|<span data-ttu-id="5c330-154">Int32</span><span class="sxs-lookup"><span data-stu-id="5c330-154">Int32</span></span>|<span data-ttu-id="5c330-155">已修复用户的数量。</span><span class="sxs-lookup"><span data-stu-id="5c330-155">Number of remediated users.</span></span>|
|<span data-ttu-id="5c330-156">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="5c330-156">errorUserCount</span></span>|<span data-ttu-id="5c330-157">Int32</span><span class="sxs-lookup"><span data-stu-id="5c330-157">Int32</span></span>|<span data-ttu-id="5c330-158">出现错误的用户数量。</span><span class="sxs-lookup"><span data-stu-id="5c330-158">Number of users had error.</span></span>|
|<span data-ttu-id="5c330-159">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="5c330-159">unknownUserCount</span></span>|<span data-ttu-id="5c330-160">Int32</span><span class="sxs-lookup"><span data-stu-id="5c330-160">Int32</span></span>|<span data-ttu-id="5c330-161">未知用户的数量。</span><span class="sxs-lookup"><span data-stu-id="5c330-161">Number of unknown users.</span></span>|
|<span data-ttu-id="5c330-162">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="5c330-162">conflictUserCount</span></span>|<span data-ttu-id="5c330-163">Int32</span><span class="sxs-lookup"><span data-stu-id="5c330-163">Int32</span></span>|<span data-ttu-id="5c330-164">冲突用户的数量。</span><span class="sxs-lookup"><span data-stu-id="5c330-164">Number of conflict users.</span></span>|
|<span data-ttu-id="5c330-165">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="5c330-165">notApplicableUserCount</span></span>|<span data-ttu-id="5c330-166">Int32</span><span class="sxs-lookup"><span data-stu-id="5c330-166">Int32</span></span>|<span data-ttu-id="5c330-167">不适用用户的数量。</span><span class="sxs-lookup"><span data-stu-id="5c330-167">Number of not applicable users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c330-168">关系</span><span class="sxs-lookup"><span data-stu-id="5c330-168">Relationships</span></span>
<span data-ttu-id="5c330-169">无</span><span class="sxs-lookup"><span data-stu-id="5c330-169">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5c330-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c330-170">JSON Representation</span></span>
<span data-ttu-id="5c330-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c330-171">Here is a JSON representation of the resource.</span></span>
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



