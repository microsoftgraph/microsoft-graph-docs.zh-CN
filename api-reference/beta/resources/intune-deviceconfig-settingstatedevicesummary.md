---
title: settingStateDeviceSummary 资源类型
description: 设置状态的设备合规性策略和配置摘要
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 26d0c2d39d79a81e419141087e508497c91f4e03
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944731"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="6b526-103">settingStateDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b526-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="6b526-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6b526-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b526-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b526-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b526-106">设置状态的设备合规性策略和配置摘要</span><span class="sxs-lookup"><span data-stu-id="6b526-106">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="6b526-107">方法</span><span class="sxs-lookup"><span data-stu-id="6b526-107">Methods</span></span>
|<span data-ttu-id="6b526-108">方法</span><span class="sxs-lookup"><span data-stu-id="6b526-108">Method</span></span>|<span data-ttu-id="6b526-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="6b526-109">Return Type</span></span>|<span data-ttu-id="6b526-110">说明</span><span class="sxs-lookup"><span data-stu-id="6b526-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6b526-111">列出 settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="6b526-111">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="6b526-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b526-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="6b526-113">列出 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6b526-113">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="6b526-114">获取 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b526-114">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="6b526-115">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b526-115">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="6b526-116">读取 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6b526-116">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="6b526-117">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b526-117">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="6b526-118">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b526-118">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="6b526-119">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b526-119">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="6b526-120">删除 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b526-120">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="6b526-121">无</span><span class="sxs-lookup"><span data-stu-id="6b526-121">None</span></span>|<span data-ttu-id="6b526-122">删除 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="6b526-122">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="6b526-123">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b526-123">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="6b526-124">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b526-124">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="6b526-125">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6b526-125">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6b526-126">属性</span><span class="sxs-lookup"><span data-stu-id="6b526-126">Properties</span></span>
|<span data-ttu-id="6b526-127">属性</span><span class="sxs-lookup"><span data-stu-id="6b526-127">Property</span></span>|<span data-ttu-id="6b526-128">类型</span><span class="sxs-lookup"><span data-stu-id="6b526-128">Type</span></span>|<span data-ttu-id="6b526-129">说明</span><span class="sxs-lookup"><span data-stu-id="6b526-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b526-130">id</span><span class="sxs-lookup"><span data-stu-id="6b526-130">id</span></span>|<span data-ttu-id="6b526-131">String</span><span class="sxs-lookup"><span data-stu-id="6b526-131">String</span></span>|<span data-ttu-id="6b526-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6b526-132">Key of the entity.</span></span>|
|<span data-ttu-id="6b526-133">settingName</span><span class="sxs-lookup"><span data-stu-id="6b526-133">settingName</span></span>|<span data-ttu-id="6b526-134">String</span><span class="sxs-lookup"><span data-stu-id="6b526-134">String</span></span>|<span data-ttu-id="6b526-135">设置的名称</span><span class="sxs-lookup"><span data-stu-id="6b526-135">Name of the setting</span></span>|
|<span data-ttu-id="6b526-136">instancePath</span><span class="sxs-lookup"><span data-stu-id="6b526-136">instancePath</span></span>|<span data-ttu-id="6b526-137">String</span><span class="sxs-lookup"><span data-stu-id="6b526-137">String</span></span>|<span data-ttu-id="6b526-138">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="6b526-138">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="6b526-139">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b526-139">unknownDeviceCount</span></span>|<span data-ttu-id="6b526-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6b526-140">Int32</span></span>|<span data-ttu-id="6b526-141">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="6b526-141">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="6b526-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b526-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="6b526-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6b526-143">Int32</span></span>|<span data-ttu-id="6b526-144">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="6b526-144">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="6b526-145">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b526-145">compliantDeviceCount</span></span>|<span data-ttu-id="6b526-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6b526-146">Int32</span></span>|<span data-ttu-id="6b526-147">设置的设备符合计数</span><span class="sxs-lookup"><span data-stu-id="6b526-147">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="6b526-148">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b526-148">remediatedDeviceCount</span></span>|<span data-ttu-id="6b526-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6b526-149">Int32</span></span>|<span data-ttu-id="6b526-150">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="6b526-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="6b526-151">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b526-151">nonCompliantDeviceCount</span></span>|<span data-ttu-id="6b526-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6b526-152">Int32</span></span>|<span data-ttu-id="6b526-153">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="6b526-153">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="6b526-154">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b526-154">errorDeviceCount</span></span>|<span data-ttu-id="6b526-155">Int32</span><span class="sxs-lookup"><span data-stu-id="6b526-155">Int32</span></span>|<span data-ttu-id="6b526-156">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="6b526-156">Device error count for the setting</span></span>|
|<span data-ttu-id="6b526-157">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b526-157">conflictDeviceCount</span></span>|<span data-ttu-id="6b526-158">Int32</span><span class="sxs-lookup"><span data-stu-id="6b526-158">Int32</span></span>|<span data-ttu-id="6b526-159">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="6b526-159">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b526-160">关系</span><span class="sxs-lookup"><span data-stu-id="6b526-160">Relationships</span></span>
<span data-ttu-id="6b526-161">无</span><span class="sxs-lookup"><span data-stu-id="6b526-161">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b526-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b526-162">JSON Representation</span></span>
<span data-ttu-id="6b526-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b526-163">Here is a JSON representation of the resource.</span></span>
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




