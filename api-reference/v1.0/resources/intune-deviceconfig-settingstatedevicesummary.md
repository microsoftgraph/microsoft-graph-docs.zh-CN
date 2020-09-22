---
title: settingStateDeviceSummary 资源类型
description: 设置状态的设备合规性策略和配置摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b53713abbd1fc4389e454950c6617ba2d9d6fc40
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079268"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="56b79-103">settingStateDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="56b79-103">settingStateDeviceSummary resource type</span></span>

<span data-ttu-id="56b79-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56b79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56b79-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56b79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56b79-106">设置状态的设备合规性策略和配置摘要</span><span class="sxs-lookup"><span data-stu-id="56b79-106">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="56b79-107">方法</span><span class="sxs-lookup"><span data-stu-id="56b79-107">Methods</span></span>
|<span data-ttu-id="56b79-108">方法</span><span class="sxs-lookup"><span data-stu-id="56b79-108">Method</span></span>|<span data-ttu-id="56b79-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="56b79-109">Return Type</span></span>|<span data-ttu-id="56b79-110">说明</span><span class="sxs-lookup"><span data-stu-id="56b79-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="56b79-111">列出 settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="56b79-111">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="56b79-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56b79-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="56b79-113">列出 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56b79-113">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="56b79-114">获取 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="56b79-114">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="56b79-115">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="56b79-115">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="56b79-116">读取 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56b79-116">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="56b79-117">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="56b79-117">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="56b79-118">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="56b79-118">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="56b79-119">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56b79-119">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="56b79-120">删除 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="56b79-120">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="56b79-121">无</span><span class="sxs-lookup"><span data-stu-id="56b79-121">None</span></span>|<span data-ttu-id="56b79-122">删除 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="56b79-122">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="56b79-123">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="56b79-123">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="56b79-124">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="56b79-124">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="56b79-125">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="56b79-125">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="56b79-126">属性</span><span class="sxs-lookup"><span data-stu-id="56b79-126">Properties</span></span>
|<span data-ttu-id="56b79-127">属性</span><span class="sxs-lookup"><span data-stu-id="56b79-127">Property</span></span>|<span data-ttu-id="56b79-128">类型</span><span class="sxs-lookup"><span data-stu-id="56b79-128">Type</span></span>|<span data-ttu-id="56b79-129">说明</span><span class="sxs-lookup"><span data-stu-id="56b79-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56b79-130">id</span><span class="sxs-lookup"><span data-stu-id="56b79-130">id</span></span>|<span data-ttu-id="56b79-131">String</span><span class="sxs-lookup"><span data-stu-id="56b79-131">String</span></span>|<span data-ttu-id="56b79-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="56b79-132">Key of the entity.</span></span>|
|<span data-ttu-id="56b79-133">settingName</span><span class="sxs-lookup"><span data-stu-id="56b79-133">settingName</span></span>|<span data-ttu-id="56b79-134">String</span><span class="sxs-lookup"><span data-stu-id="56b79-134">String</span></span>|<span data-ttu-id="56b79-135">设置的名称</span><span class="sxs-lookup"><span data-stu-id="56b79-135">Name of the setting</span></span>|
|<span data-ttu-id="56b79-136">instancePath</span><span class="sxs-lookup"><span data-stu-id="56b79-136">instancePath</span></span>|<span data-ttu-id="56b79-137">String</span><span class="sxs-lookup"><span data-stu-id="56b79-137">String</span></span>|<span data-ttu-id="56b79-138">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="56b79-138">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="56b79-139">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56b79-139">unknownDeviceCount</span></span>|<span data-ttu-id="56b79-140">Int32</span><span class="sxs-lookup"><span data-stu-id="56b79-140">Int32</span></span>|<span data-ttu-id="56b79-141">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="56b79-141">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="56b79-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56b79-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="56b79-143">Int32</span><span class="sxs-lookup"><span data-stu-id="56b79-143">Int32</span></span>|<span data-ttu-id="56b79-144">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="56b79-144">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="56b79-145">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56b79-145">compliantDeviceCount</span></span>|<span data-ttu-id="56b79-146">Int32</span><span class="sxs-lookup"><span data-stu-id="56b79-146">Int32</span></span>|<span data-ttu-id="56b79-147">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="56b79-147">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="56b79-148">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56b79-148">remediatedDeviceCount</span></span>|<span data-ttu-id="56b79-149">Int32</span><span class="sxs-lookup"><span data-stu-id="56b79-149">Int32</span></span>|<span data-ttu-id="56b79-150">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="56b79-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="56b79-151">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56b79-151">nonCompliantDeviceCount</span></span>|<span data-ttu-id="56b79-152">Int32</span><span class="sxs-lookup"><span data-stu-id="56b79-152">Int32</span></span>|<span data-ttu-id="56b79-153">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="56b79-153">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="56b79-154">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56b79-154">errorDeviceCount</span></span>|<span data-ttu-id="56b79-155">Int32</span><span class="sxs-lookup"><span data-stu-id="56b79-155">Int32</span></span>|<span data-ttu-id="56b79-156">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="56b79-156">Device error count for the setting</span></span>|
|<span data-ttu-id="56b79-157">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56b79-157">conflictDeviceCount</span></span>|<span data-ttu-id="56b79-158">Int32</span><span class="sxs-lookup"><span data-stu-id="56b79-158">Int32</span></span>|<span data-ttu-id="56b79-159">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="56b79-159">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="56b79-160">关系</span><span class="sxs-lookup"><span data-stu-id="56b79-160">Relationships</span></span>
<span data-ttu-id="56b79-161">无</span><span class="sxs-lookup"><span data-stu-id="56b79-161">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56b79-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56b79-162">JSON Representation</span></span>
<span data-ttu-id="56b79-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56b79-163">Here is a JSON representation of the resource.</span></span>
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









