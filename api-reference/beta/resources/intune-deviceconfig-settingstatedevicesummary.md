---
title: settingStateDeviceSummary 资源类型
description: 设置状态的设备合规性策略和配置摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed705b12c35c4414913ca0bd3686191f00941449
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049413"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="8b59d-103">settingStateDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b59d-103">settingStateDeviceSummary resource type</span></span>

<span data-ttu-id="8b59d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b59d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b59d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8b59d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b59d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8b59d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b59d-107">设置状态的设备合规性策略和配置摘要</span><span class="sxs-lookup"><span data-stu-id="8b59d-107">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="8b59d-108">方法</span><span class="sxs-lookup"><span data-stu-id="8b59d-108">Methods</span></span>
|<span data-ttu-id="8b59d-109">方法</span><span class="sxs-lookup"><span data-stu-id="8b59d-109">Method</span></span>|<span data-ttu-id="8b59d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8b59d-110">Return Type</span></span>|<span data-ttu-id="8b59d-111">说明</span><span class="sxs-lookup"><span data-stu-id="8b59d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8b59d-112">列出 settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="8b59d-112">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="8b59d-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8b59d-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="8b59d-114">列出 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8b59d-114">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="8b59d-115">获取 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="8b59d-115">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="8b59d-116">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="8b59d-116">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="8b59d-117">读取 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8b59d-117">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="8b59d-118">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="8b59d-118">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="8b59d-119">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="8b59d-119">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="8b59d-120">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8b59d-120">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="8b59d-121">删除 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="8b59d-121">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="8b59d-122">无</span><span class="sxs-lookup"><span data-stu-id="8b59d-122">None</span></span>|<span data-ttu-id="8b59d-123">删除 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="8b59d-123">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="8b59d-124">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="8b59d-124">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="8b59d-125">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="8b59d-125">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="8b59d-126">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8b59d-126">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8b59d-127">属性</span><span class="sxs-lookup"><span data-stu-id="8b59d-127">Properties</span></span>
|<span data-ttu-id="8b59d-128">属性</span><span class="sxs-lookup"><span data-stu-id="8b59d-128">Property</span></span>|<span data-ttu-id="8b59d-129">类型</span><span class="sxs-lookup"><span data-stu-id="8b59d-129">Type</span></span>|<span data-ttu-id="8b59d-130">说明</span><span class="sxs-lookup"><span data-stu-id="8b59d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b59d-131">id</span><span class="sxs-lookup"><span data-stu-id="8b59d-131">id</span></span>|<span data-ttu-id="8b59d-132">String</span><span class="sxs-lookup"><span data-stu-id="8b59d-132">String</span></span>|<span data-ttu-id="8b59d-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8b59d-133">Key of the entity.</span></span>|
|<span data-ttu-id="8b59d-134">settingName</span><span class="sxs-lookup"><span data-stu-id="8b59d-134">settingName</span></span>|<span data-ttu-id="8b59d-135">String</span><span class="sxs-lookup"><span data-stu-id="8b59d-135">String</span></span>|<span data-ttu-id="8b59d-136">设置的名称</span><span class="sxs-lookup"><span data-stu-id="8b59d-136">Name of the setting</span></span>|
|<span data-ttu-id="8b59d-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="8b59d-137">instancePath</span></span>|<span data-ttu-id="8b59d-138">String</span><span class="sxs-lookup"><span data-stu-id="8b59d-138">String</span></span>|<span data-ttu-id="8b59d-139">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="8b59d-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="8b59d-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8b59d-140">unknownDeviceCount</span></span>|<span data-ttu-id="8b59d-141">Int32</span><span class="sxs-lookup"><span data-stu-id="8b59d-141">Int32</span></span>|<span data-ttu-id="8b59d-142">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="8b59d-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="8b59d-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8b59d-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="8b59d-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8b59d-144">Int32</span></span>|<span data-ttu-id="8b59d-145">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="8b59d-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="8b59d-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8b59d-146">compliantDeviceCount</span></span>|<span data-ttu-id="8b59d-147">Int32</span><span class="sxs-lookup"><span data-stu-id="8b59d-147">Int32</span></span>|<span data-ttu-id="8b59d-148">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="8b59d-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="8b59d-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8b59d-149">remediatedDeviceCount</span></span>|<span data-ttu-id="8b59d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8b59d-150">Int32</span></span>|<span data-ttu-id="8b59d-151">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="8b59d-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="8b59d-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8b59d-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="8b59d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8b59d-153">Int32</span></span>|<span data-ttu-id="8b59d-154">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="8b59d-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="8b59d-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8b59d-155">errorDeviceCount</span></span>|<span data-ttu-id="8b59d-156">Int32</span><span class="sxs-lookup"><span data-stu-id="8b59d-156">Int32</span></span>|<span data-ttu-id="8b59d-157">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="8b59d-157">Device error count for the setting</span></span>|
|<span data-ttu-id="8b59d-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8b59d-158">conflictDeviceCount</span></span>|<span data-ttu-id="8b59d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="8b59d-159">Int32</span></span>|<span data-ttu-id="8b59d-160">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="8b59d-160">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b59d-161">关系</span><span class="sxs-lookup"><span data-stu-id="8b59d-161">Relationships</span></span>
<span data-ttu-id="8b59d-162">无</span><span class="sxs-lookup"><span data-stu-id="8b59d-162">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b59d-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b59d-163">JSON Representation</span></span>
<span data-ttu-id="8b59d-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b59d-164">Here is a JSON representation of the resource.</span></span>
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






