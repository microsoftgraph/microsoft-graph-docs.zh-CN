---
title: settingStateDeviceSummary 资源类型
description: 设置状态的设备合规性策略和配置摘要
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ed7427e05e8d48f090f991b45e3a46cbc2985b01
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031113"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="81e5e-103">settingStateDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="81e5e-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="81e5e-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81e5e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81e5e-105">设置状态的设备合规性策略和配置摘要</span><span class="sxs-lookup"><span data-stu-id="81e5e-105">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="81e5e-106">方法</span><span class="sxs-lookup"><span data-stu-id="81e5e-106">Methods</span></span>
|<span data-ttu-id="81e5e-107">方法</span><span class="sxs-lookup"><span data-stu-id="81e5e-107">Method</span></span>|<span data-ttu-id="81e5e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="81e5e-108">Return Type</span></span>|<span data-ttu-id="81e5e-109">说明</span><span class="sxs-lookup"><span data-stu-id="81e5e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81e5e-110">列出 settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="81e5e-110">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="81e5e-111">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81e5e-111">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="81e5e-112">列出 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81e5e-112">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="81e5e-113">获取 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="81e5e-113">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="81e5e-114">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="81e5e-114">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="81e5e-115">读取 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81e5e-115">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="81e5e-116">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="81e5e-116">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="81e5e-117">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="81e5e-117">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="81e5e-118">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="81e5e-118">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="81e5e-119">删除 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="81e5e-119">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="81e5e-120">无</span><span class="sxs-lookup"><span data-stu-id="81e5e-120">None</span></span>|<span data-ttu-id="81e5e-121">删除 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="81e5e-121">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="81e5e-122">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="81e5e-122">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="81e5e-123">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="81e5e-123">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="81e5e-124">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="81e5e-124">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81e5e-125">属性</span><span class="sxs-lookup"><span data-stu-id="81e5e-125">Properties</span></span>
|<span data-ttu-id="81e5e-126">属性</span><span class="sxs-lookup"><span data-stu-id="81e5e-126">Property</span></span>|<span data-ttu-id="81e5e-127">类型</span><span class="sxs-lookup"><span data-stu-id="81e5e-127">Type</span></span>|<span data-ttu-id="81e5e-128">说明</span><span class="sxs-lookup"><span data-stu-id="81e5e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81e5e-129">id</span><span class="sxs-lookup"><span data-stu-id="81e5e-129">id</span></span>|<span data-ttu-id="81e5e-130">String</span><span class="sxs-lookup"><span data-stu-id="81e5e-130">String</span></span>|<span data-ttu-id="81e5e-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="81e5e-131">Key of the entity.</span></span>|
|<span data-ttu-id="81e5e-132">settingName</span><span class="sxs-lookup"><span data-stu-id="81e5e-132">settingName</span></span>|<span data-ttu-id="81e5e-133">String</span><span class="sxs-lookup"><span data-stu-id="81e5e-133">String</span></span>|<span data-ttu-id="81e5e-134">设置的名称</span><span class="sxs-lookup"><span data-stu-id="81e5e-134">Name of the setting</span></span>|
|<span data-ttu-id="81e5e-135">instancePath</span><span class="sxs-lookup"><span data-stu-id="81e5e-135">instancePath</span></span>|<span data-ttu-id="81e5e-136">String</span><span class="sxs-lookup"><span data-stu-id="81e5e-136">String</span></span>|<span data-ttu-id="81e5e-137">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="81e5e-137">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="81e5e-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="81e5e-138">unknownDeviceCount</span></span>|<span data-ttu-id="81e5e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="81e5e-139">Int32</span></span>|<span data-ttu-id="81e5e-140">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="81e5e-140">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="81e5e-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="81e5e-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="81e5e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="81e5e-142">Int32</span></span>|<span data-ttu-id="81e5e-143">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="81e5e-143">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="81e5e-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="81e5e-144">compliantDeviceCount</span></span>|<span data-ttu-id="81e5e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="81e5e-145">Int32</span></span>|<span data-ttu-id="81e5e-146">设置的设备符合计数</span><span class="sxs-lookup"><span data-stu-id="81e5e-146">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="81e5e-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="81e5e-147">remediatedDeviceCount</span></span>|<span data-ttu-id="81e5e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="81e5e-148">Int32</span></span>|<span data-ttu-id="81e5e-149">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="81e5e-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="81e5e-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="81e5e-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="81e5e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="81e5e-151">Int32</span></span>|<span data-ttu-id="81e5e-152">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="81e5e-152">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="81e5e-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="81e5e-153">errorDeviceCount</span></span>|<span data-ttu-id="81e5e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="81e5e-154">Int32</span></span>|<span data-ttu-id="81e5e-155">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="81e5e-155">Device error count for the setting</span></span>|
|<span data-ttu-id="81e5e-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="81e5e-156">conflictDeviceCount</span></span>|<span data-ttu-id="81e5e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="81e5e-157">Int32</span></span>|<span data-ttu-id="81e5e-158">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="81e5e-158">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="81e5e-159">关系</span><span class="sxs-lookup"><span data-stu-id="81e5e-159">Relationships</span></span>
<span data-ttu-id="81e5e-160">无</span><span class="sxs-lookup"><span data-stu-id="81e5e-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81e5e-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81e5e-161">JSON Representation</span></span>
<span data-ttu-id="81e5e-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81e5e-162">Here is a JSON representation of the resource.</span></span>
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



