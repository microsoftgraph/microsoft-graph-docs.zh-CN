---
title: settingStateDeviceSummary 资源类型
description: 设置状态的设备合规性策略和配置摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4abf6f56dd51410faab49222de64184aec7dd67f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709885"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="e0fc1-103">settingStateDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0fc1-103">settingStateDeviceSummary resource type</span></span>

<span data-ttu-id="e0fc1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0fc1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0fc1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e0fc1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0fc1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0fc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0fc1-107">设置状态的设备合规性策略和配置摘要</span><span class="sxs-lookup"><span data-stu-id="e0fc1-107">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="e0fc1-108">Methods</span><span class="sxs-lookup"><span data-stu-id="e0fc1-108">Methods</span></span>
|<span data-ttu-id="e0fc1-109">方法</span><span class="sxs-lookup"><span data-stu-id="e0fc1-109">Method</span></span>|<span data-ttu-id="e0fc1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e0fc1-110">Return Type</span></span>|<span data-ttu-id="e0fc1-111">说明</span><span class="sxs-lookup"><span data-stu-id="e0fc1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e0fc1-112">列出 settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="e0fc1-112">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="e0fc1-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0fc1-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="e0fc1-114">列出 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e0fc1-114">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="e0fc1-115">获取 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e0fc1-115">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="e0fc1-116">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e0fc1-116">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="e0fc1-117">读取 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e0fc1-117">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="e0fc1-118">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e0fc1-118">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="e0fc1-119">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e0fc1-119">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="e0fc1-120">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0fc1-120">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="e0fc1-121">删除 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e0fc1-121">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="e0fc1-122">无</span><span class="sxs-lookup"><span data-stu-id="e0fc1-122">None</span></span>|<span data-ttu-id="e0fc1-123">删除 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="e0fc1-123">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="e0fc1-124">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e0fc1-124">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="e0fc1-125">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e0fc1-125">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="e0fc1-126">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e0fc1-126">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e0fc1-127">属性</span><span class="sxs-lookup"><span data-stu-id="e0fc1-127">Properties</span></span>
|<span data-ttu-id="e0fc1-128">属性</span><span class="sxs-lookup"><span data-stu-id="e0fc1-128">Property</span></span>|<span data-ttu-id="e0fc1-129">类型</span><span class="sxs-lookup"><span data-stu-id="e0fc1-129">Type</span></span>|<span data-ttu-id="e0fc1-130">说明</span><span class="sxs-lookup"><span data-stu-id="e0fc1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0fc1-131">id</span><span class="sxs-lookup"><span data-stu-id="e0fc1-131">id</span></span>|<span data-ttu-id="e0fc1-132">String</span><span class="sxs-lookup"><span data-stu-id="e0fc1-132">String</span></span>|<span data-ttu-id="e0fc1-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e0fc1-133">Key of the entity.</span></span>|
|<span data-ttu-id="e0fc1-134">settingName</span><span class="sxs-lookup"><span data-stu-id="e0fc1-134">settingName</span></span>|<span data-ttu-id="e0fc1-135">String</span><span class="sxs-lookup"><span data-stu-id="e0fc1-135">String</span></span>|<span data-ttu-id="e0fc1-136">设置的名称</span><span class="sxs-lookup"><span data-stu-id="e0fc1-136">Name of the setting</span></span>|
|<span data-ttu-id="e0fc1-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="e0fc1-137">instancePath</span></span>|<span data-ttu-id="e0fc1-138">String</span><span class="sxs-lookup"><span data-stu-id="e0fc1-138">String</span></span>|<span data-ttu-id="e0fc1-139">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="e0fc1-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="e0fc1-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0fc1-140">unknownDeviceCount</span></span>|<span data-ttu-id="e0fc1-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e0fc1-141">Int32</span></span>|<span data-ttu-id="e0fc1-142">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="e0fc1-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="e0fc1-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0fc1-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="e0fc1-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e0fc1-144">Int32</span></span>|<span data-ttu-id="e0fc1-145">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="e0fc1-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="e0fc1-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0fc1-146">compliantDeviceCount</span></span>|<span data-ttu-id="e0fc1-147">Int32</span><span class="sxs-lookup"><span data-stu-id="e0fc1-147">Int32</span></span>|<span data-ttu-id="e0fc1-148">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="e0fc1-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="e0fc1-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0fc1-149">remediatedDeviceCount</span></span>|<span data-ttu-id="e0fc1-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e0fc1-150">Int32</span></span>|<span data-ttu-id="e0fc1-151">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="e0fc1-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="e0fc1-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0fc1-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e0fc1-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e0fc1-153">Int32</span></span>|<span data-ttu-id="e0fc1-154">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="e0fc1-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="e0fc1-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0fc1-155">errorDeviceCount</span></span>|<span data-ttu-id="e0fc1-156">Int32</span><span class="sxs-lookup"><span data-stu-id="e0fc1-156">Int32</span></span>|<span data-ttu-id="e0fc1-157">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="e0fc1-157">Device error count for the setting</span></span>|
|<span data-ttu-id="e0fc1-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0fc1-158">conflictDeviceCount</span></span>|<span data-ttu-id="e0fc1-159">Int32</span><span class="sxs-lookup"><span data-stu-id="e0fc1-159">Int32</span></span>|<span data-ttu-id="e0fc1-160">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="e0fc1-160">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0fc1-161">关系</span><span class="sxs-lookup"><span data-stu-id="e0fc1-161">Relationships</span></span>
<span data-ttu-id="e0fc1-162">无</span><span class="sxs-lookup"><span data-stu-id="e0fc1-162">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0fc1-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0fc1-163">JSON Representation</span></span>
<span data-ttu-id="e0fc1-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0fc1-164">Here is a JSON representation of the resource.</span></span>
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





