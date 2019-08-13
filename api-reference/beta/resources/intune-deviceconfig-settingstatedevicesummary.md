---
title: settingStateDeviceSummary 资源类型
description: 设置状态的设备合规性策略和配置摘要
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 03916d1e41fb89c1ae8a218ca0caa47ccf4afb37
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368007"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="69999-103">settingStateDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="69999-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="69999-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69999-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69999-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69999-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69999-106">设置状态的设备合规性策略和配置摘要</span><span class="sxs-lookup"><span data-stu-id="69999-106">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="69999-107">方法</span><span class="sxs-lookup"><span data-stu-id="69999-107">Methods</span></span>
|<span data-ttu-id="69999-108">方法</span><span class="sxs-lookup"><span data-stu-id="69999-108">Method</span></span>|<span data-ttu-id="69999-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="69999-109">Return Type</span></span>|<span data-ttu-id="69999-110">说明</span><span class="sxs-lookup"><span data-stu-id="69999-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="69999-111">列出 settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="69999-111">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="69999-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="69999-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="69999-113">列出 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="69999-113">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="69999-114">获取 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="69999-114">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="69999-115">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="69999-115">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="69999-116">读取 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="69999-116">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="69999-117">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="69999-117">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="69999-118">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="69999-118">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="69999-119">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="69999-119">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="69999-120">删除 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="69999-120">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="69999-121">无</span><span class="sxs-lookup"><span data-stu-id="69999-121">None</span></span>|<span data-ttu-id="69999-122">删除 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="69999-122">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="69999-123">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="69999-123">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="69999-124">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="69999-124">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="69999-125">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="69999-125">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="69999-126">属性</span><span class="sxs-lookup"><span data-stu-id="69999-126">Properties</span></span>
|<span data-ttu-id="69999-127">属性</span><span class="sxs-lookup"><span data-stu-id="69999-127">Property</span></span>|<span data-ttu-id="69999-128">类型</span><span class="sxs-lookup"><span data-stu-id="69999-128">Type</span></span>|<span data-ttu-id="69999-129">说明</span><span class="sxs-lookup"><span data-stu-id="69999-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69999-130">id</span><span class="sxs-lookup"><span data-stu-id="69999-130">id</span></span>|<span data-ttu-id="69999-131">String</span><span class="sxs-lookup"><span data-stu-id="69999-131">String</span></span>|<span data-ttu-id="69999-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="69999-132">Key of the entity.</span></span>|
|<span data-ttu-id="69999-133">settingName</span><span class="sxs-lookup"><span data-stu-id="69999-133">settingName</span></span>|<span data-ttu-id="69999-134">String</span><span class="sxs-lookup"><span data-stu-id="69999-134">String</span></span>|<span data-ttu-id="69999-135">设置的名称</span><span class="sxs-lookup"><span data-stu-id="69999-135">Name of the setting</span></span>|
|<span data-ttu-id="69999-136">instancePath</span><span class="sxs-lookup"><span data-stu-id="69999-136">instancePath</span></span>|<span data-ttu-id="69999-137">String</span><span class="sxs-lookup"><span data-stu-id="69999-137">String</span></span>|<span data-ttu-id="69999-138">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="69999-138">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="69999-139">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69999-139">unknownDeviceCount</span></span>|<span data-ttu-id="69999-140">Int32</span><span class="sxs-lookup"><span data-stu-id="69999-140">Int32</span></span>|<span data-ttu-id="69999-141">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="69999-141">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="69999-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69999-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="69999-143">Int32</span><span class="sxs-lookup"><span data-stu-id="69999-143">Int32</span></span>|<span data-ttu-id="69999-144">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="69999-144">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="69999-145">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69999-145">compliantDeviceCount</span></span>|<span data-ttu-id="69999-146">Int32</span><span class="sxs-lookup"><span data-stu-id="69999-146">Int32</span></span>|<span data-ttu-id="69999-147">设置的设备符合计数</span><span class="sxs-lookup"><span data-stu-id="69999-147">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="69999-148">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69999-148">remediatedDeviceCount</span></span>|<span data-ttu-id="69999-149">Int32</span><span class="sxs-lookup"><span data-stu-id="69999-149">Int32</span></span>|<span data-ttu-id="69999-150">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="69999-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="69999-151">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69999-151">nonCompliantDeviceCount</span></span>|<span data-ttu-id="69999-152">Int32</span><span class="sxs-lookup"><span data-stu-id="69999-152">Int32</span></span>|<span data-ttu-id="69999-153">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="69999-153">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="69999-154">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69999-154">errorDeviceCount</span></span>|<span data-ttu-id="69999-155">Int32</span><span class="sxs-lookup"><span data-stu-id="69999-155">Int32</span></span>|<span data-ttu-id="69999-156">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="69999-156">Device error count for the setting</span></span>|
|<span data-ttu-id="69999-157">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69999-157">conflictDeviceCount</span></span>|<span data-ttu-id="69999-158">Int32</span><span class="sxs-lookup"><span data-stu-id="69999-158">Int32</span></span>|<span data-ttu-id="69999-159">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="69999-159">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="69999-160">关系</span><span class="sxs-lookup"><span data-stu-id="69999-160">Relationships</span></span>
<span data-ttu-id="69999-161">无</span><span class="sxs-lookup"><span data-stu-id="69999-161">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69999-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69999-162">JSON Representation</span></span>
<span data-ttu-id="69999-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69999-163">Here is a JSON representation of the resource.</span></span>
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



