---
title: deviceCompliancePolicyDeviceStateSummary 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 006b1ca71f8441898ba758397334c7ae31ac5690
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318807"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="88ca4-103">deviceCompliancePolicyDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="88ca4-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="88ca4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="88ca4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88ca4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="88ca4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88ca4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="88ca4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88ca4-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="88ca4-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="88ca4-108">方法</span><span class="sxs-lookup"><span data-stu-id="88ca4-108">Methods</span></span>
|<span data-ttu-id="88ca4-109">方法</span><span class="sxs-lookup"><span data-stu-id="88ca4-109">Method</span></span>|<span data-ttu-id="88ca4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="88ca4-110">Return Type</span></span>|<span data-ttu-id="88ca4-111">说明</span><span class="sxs-lookup"><span data-stu-id="88ca4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88ca4-112">获取 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="88ca4-112">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="88ca4-113">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="88ca4-113">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="88ca4-114">读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88ca4-114">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="88ca4-115">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="88ca4-115">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="88ca4-116">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="88ca4-116">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="88ca4-117">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="88ca4-117">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="88ca4-118">属性</span><span class="sxs-lookup"><span data-stu-id="88ca4-118">Properties</span></span>
|<span data-ttu-id="88ca4-119">属性</span><span class="sxs-lookup"><span data-stu-id="88ca4-119">Property</span></span>|<span data-ttu-id="88ca4-120">类型</span><span class="sxs-lookup"><span data-stu-id="88ca4-120">Type</span></span>|<span data-ttu-id="88ca4-121">说明</span><span class="sxs-lookup"><span data-stu-id="88ca4-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88ca4-122">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="88ca4-122">inGracePeriodCount</span></span>|<span data-ttu-id="88ca4-123">Int32</span><span class="sxs-lookup"><span data-stu-id="88ca4-123">Int32</span></span>|<span data-ttu-id="88ca4-124">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="88ca4-124">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="88ca4-125">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="88ca4-125">configManagerCount</span></span>|<span data-ttu-id="88ca4-126">Int32</span><span class="sxs-lookup"><span data-stu-id="88ca4-126">Int32</span></span>|<span data-ttu-id="88ca4-127">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="88ca4-127">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="88ca4-128">id</span><span class="sxs-lookup"><span data-stu-id="88ca4-128">id</span></span>|<span data-ttu-id="88ca4-129">String</span><span class="sxs-lookup"><span data-stu-id="88ca4-129">String</span></span>|<span data-ttu-id="88ca4-130">实体的键。</span><span class="sxs-lookup"><span data-stu-id="88ca4-130">Key of the entity.</span></span>|
|<span data-ttu-id="88ca4-131">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="88ca4-131">unknownDeviceCount</span></span>|<span data-ttu-id="88ca4-132">Int32</span><span class="sxs-lookup"><span data-stu-id="88ca4-132">Int32</span></span>|<span data-ttu-id="88ca4-133">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="88ca4-133">Number of unknown devices</span></span>|
|<span data-ttu-id="88ca4-134">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="88ca4-134">notApplicableDeviceCount</span></span>|<span data-ttu-id="88ca4-135">Int32</span><span class="sxs-lookup"><span data-stu-id="88ca4-135">Int32</span></span>|<span data-ttu-id="88ca4-136">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="88ca4-136">Number of not applicable devices</span></span>|
|<span data-ttu-id="88ca4-137">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="88ca4-137">compliantDeviceCount</span></span>|<span data-ttu-id="88ca4-138">Int32</span><span class="sxs-lookup"><span data-stu-id="88ca4-138">Int32</span></span>|<span data-ttu-id="88ca4-139">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="88ca4-139">Number of compliant devices</span></span>|
|<span data-ttu-id="88ca4-140">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="88ca4-140">remediatedDeviceCount</span></span>|<span data-ttu-id="88ca4-141">Int32</span><span class="sxs-lookup"><span data-stu-id="88ca4-141">Int32</span></span>|<span data-ttu-id="88ca4-142">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="88ca4-142">Number of remediated devices</span></span>|
|<span data-ttu-id="88ca4-143">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="88ca4-143">nonCompliantDeviceCount</span></span>|<span data-ttu-id="88ca4-144">Int32</span><span class="sxs-lookup"><span data-stu-id="88ca4-144">Int32</span></span>|<span data-ttu-id="88ca4-145">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="88ca4-145">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="88ca4-146">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="88ca4-146">errorDeviceCount</span></span>|<span data-ttu-id="88ca4-147">Int32</span><span class="sxs-lookup"><span data-stu-id="88ca4-147">Int32</span></span>|<span data-ttu-id="88ca4-148">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="88ca4-148">Number of error devices</span></span>|
|<span data-ttu-id="88ca4-149">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="88ca4-149">conflictDeviceCount</span></span>|<span data-ttu-id="88ca4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="88ca4-150">Int32</span></span>|<span data-ttu-id="88ca4-151">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="88ca4-151">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="88ca4-152">关系</span><span class="sxs-lookup"><span data-stu-id="88ca4-152">Relationships</span></span>
<span data-ttu-id="88ca4-153">无</span><span class="sxs-lookup"><span data-stu-id="88ca4-153">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="88ca4-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88ca4-154">JSON Representation</span></span>
<span data-ttu-id="88ca4-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88ca4-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```





