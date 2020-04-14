---
title: settingStateDeviceSummary 资源类型
description: 设置状态的设备合规性策略和配置摘要
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0352b3e27da90d1dffee34be7ecfbe634f3796c0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444816"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="94804-103">settingStateDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="94804-103">settingStateDeviceSummary resource type</span></span>

<span data-ttu-id="94804-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94804-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94804-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="94804-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94804-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94804-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94804-107">设置状态的设备合规性策略和配置摘要</span><span class="sxs-lookup"><span data-stu-id="94804-107">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="94804-108">方法</span><span class="sxs-lookup"><span data-stu-id="94804-108">Methods</span></span>
|<span data-ttu-id="94804-109">方法</span><span class="sxs-lookup"><span data-stu-id="94804-109">Method</span></span>|<span data-ttu-id="94804-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="94804-110">Return Type</span></span>|<span data-ttu-id="94804-111">说明</span><span class="sxs-lookup"><span data-stu-id="94804-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="94804-112">列出 settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="94804-112">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="94804-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94804-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="94804-114">列出 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94804-114">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="94804-115">获取 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="94804-115">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="94804-116">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="94804-116">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="94804-117">读取 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94804-117">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="94804-118">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="94804-118">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="94804-119">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="94804-119">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="94804-120">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94804-120">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="94804-121">删除 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="94804-121">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="94804-122">无</span><span class="sxs-lookup"><span data-stu-id="94804-122">None</span></span>|<span data-ttu-id="94804-123">删除 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="94804-123">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="94804-124">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="94804-124">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="94804-125">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="94804-125">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="94804-126">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94804-126">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="94804-127">属性</span><span class="sxs-lookup"><span data-stu-id="94804-127">Properties</span></span>
|<span data-ttu-id="94804-128">属性</span><span class="sxs-lookup"><span data-stu-id="94804-128">Property</span></span>|<span data-ttu-id="94804-129">类型</span><span class="sxs-lookup"><span data-stu-id="94804-129">Type</span></span>|<span data-ttu-id="94804-130">说明</span><span class="sxs-lookup"><span data-stu-id="94804-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94804-131">id</span><span class="sxs-lookup"><span data-stu-id="94804-131">id</span></span>|<span data-ttu-id="94804-132">String</span><span class="sxs-lookup"><span data-stu-id="94804-132">String</span></span>|<span data-ttu-id="94804-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="94804-133">Key of the entity.</span></span>|
|<span data-ttu-id="94804-134">settingName</span><span class="sxs-lookup"><span data-stu-id="94804-134">settingName</span></span>|<span data-ttu-id="94804-135">String</span><span class="sxs-lookup"><span data-stu-id="94804-135">String</span></span>|<span data-ttu-id="94804-136">设置的名称</span><span class="sxs-lookup"><span data-stu-id="94804-136">Name of the setting</span></span>|
|<span data-ttu-id="94804-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="94804-137">instancePath</span></span>|<span data-ttu-id="94804-138">String</span><span class="sxs-lookup"><span data-stu-id="94804-138">String</span></span>|<span data-ttu-id="94804-139">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="94804-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="94804-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94804-140">unknownDeviceCount</span></span>|<span data-ttu-id="94804-141">Int32</span><span class="sxs-lookup"><span data-stu-id="94804-141">Int32</span></span>|<span data-ttu-id="94804-142">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="94804-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="94804-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94804-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="94804-144">Int32</span><span class="sxs-lookup"><span data-stu-id="94804-144">Int32</span></span>|<span data-ttu-id="94804-145">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="94804-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="94804-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94804-146">compliantDeviceCount</span></span>|<span data-ttu-id="94804-147">Int32</span><span class="sxs-lookup"><span data-stu-id="94804-147">Int32</span></span>|<span data-ttu-id="94804-148">设置的设备符合计数</span><span class="sxs-lookup"><span data-stu-id="94804-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="94804-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94804-149">remediatedDeviceCount</span></span>|<span data-ttu-id="94804-150">Int32</span><span class="sxs-lookup"><span data-stu-id="94804-150">Int32</span></span>|<span data-ttu-id="94804-151">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="94804-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="94804-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94804-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="94804-153">Int32</span><span class="sxs-lookup"><span data-stu-id="94804-153">Int32</span></span>|<span data-ttu-id="94804-154">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="94804-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="94804-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94804-155">errorDeviceCount</span></span>|<span data-ttu-id="94804-156">Int32</span><span class="sxs-lookup"><span data-stu-id="94804-156">Int32</span></span>|<span data-ttu-id="94804-157">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="94804-157">Device error count for the setting</span></span>|
|<span data-ttu-id="94804-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94804-158">conflictDeviceCount</span></span>|<span data-ttu-id="94804-159">Int32</span><span class="sxs-lookup"><span data-stu-id="94804-159">Int32</span></span>|<span data-ttu-id="94804-160">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="94804-160">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="94804-161">关系</span><span class="sxs-lookup"><span data-stu-id="94804-161">Relationships</span></span>
<span data-ttu-id="94804-162">无</span><span class="sxs-lookup"><span data-stu-id="94804-162">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94804-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94804-163">JSON Representation</span></span>
<span data-ttu-id="94804-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94804-164">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.settingStateDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "instancePath": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



