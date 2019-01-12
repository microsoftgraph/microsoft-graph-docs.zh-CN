---
title: settingStateDeviceSummary 资源类型
description: 设置状态的设备合规性策略和配置摘要
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2104998cfdd65659114b1850d3cfcf1392bf9642
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925873"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="5eeb3-103">settingStateDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="5eeb3-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="5eeb3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5eeb3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5eeb3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5eeb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5eeb3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5eeb3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5eeb3-107">设置状态的设备合规性策略和配置摘要</span><span class="sxs-lookup"><span data-stu-id="5eeb3-107">Device Compilance Policy and Configuration for a Setting State summary</span></span>
## <a name="methods"></a><span data-ttu-id="5eeb3-108">方法</span><span class="sxs-lookup"><span data-stu-id="5eeb3-108">Methods</span></span>
|<span data-ttu-id="5eeb3-109">方法</span><span class="sxs-lookup"><span data-stu-id="5eeb3-109">Method</span></span>|<span data-ttu-id="5eeb3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5eeb3-110">Return Type</span></span>|<span data-ttu-id="5eeb3-111">说明</span><span class="sxs-lookup"><span data-stu-id="5eeb3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5eeb3-112">列出 settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="5eeb3-112">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="5eeb3-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5eeb3-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="5eeb3-114">列出 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5eeb3-114">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="5eeb3-115">获取 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="5eeb3-115">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="5eeb3-116">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="5eeb3-116">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="5eeb3-117">读取 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5eeb3-117">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="5eeb3-118">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="5eeb3-118">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="5eeb3-119">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="5eeb3-119">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="5eeb3-120">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5eeb3-120">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="5eeb3-121">删除 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="5eeb3-121">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="5eeb3-122">无</span><span class="sxs-lookup"><span data-stu-id="5eeb3-122">None</span></span>|<span data-ttu-id="5eeb3-123">删除 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="5eeb3-123">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="5eeb3-124">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="5eeb3-124">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="5eeb3-125">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="5eeb3-125">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="5eeb3-126">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5eeb3-126">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5eeb3-127">属性</span><span class="sxs-lookup"><span data-stu-id="5eeb3-127">Properties</span></span>
|<span data-ttu-id="5eeb3-128">属性</span><span class="sxs-lookup"><span data-stu-id="5eeb3-128">Property</span></span>|<span data-ttu-id="5eeb3-129">类型</span><span class="sxs-lookup"><span data-stu-id="5eeb3-129">Type</span></span>|<span data-ttu-id="5eeb3-130">说明</span><span class="sxs-lookup"><span data-stu-id="5eeb3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5eeb3-131">id</span><span class="sxs-lookup"><span data-stu-id="5eeb3-131">id</span></span>|<span data-ttu-id="5eeb3-132">String</span><span class="sxs-lookup"><span data-stu-id="5eeb3-132">String</span></span>|<span data-ttu-id="5eeb3-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5eeb3-133">Key of the entity.</span></span>|
|<span data-ttu-id="5eeb3-134">settingName</span><span class="sxs-lookup"><span data-stu-id="5eeb3-134">settingName</span></span>|<span data-ttu-id="5eeb3-135">String</span><span class="sxs-lookup"><span data-stu-id="5eeb3-135">String</span></span>|<span data-ttu-id="5eeb3-136">设置的名称</span><span class="sxs-lookup"><span data-stu-id="5eeb3-136">Name of the setting</span></span>|
|<span data-ttu-id="5eeb3-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="5eeb3-137">instancePath</span></span>|<span data-ttu-id="5eeb3-138">String</span><span class="sxs-lookup"><span data-stu-id="5eeb3-138">String</span></span>|<span data-ttu-id="5eeb3-139">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="5eeb3-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="5eeb3-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eeb3-140">unknownDeviceCount</span></span>|<span data-ttu-id="5eeb3-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5eeb3-141">Int32</span></span>|<span data-ttu-id="5eeb3-142">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="5eeb3-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="5eeb3-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eeb3-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="5eeb3-144">Int32</span><span class="sxs-lookup"><span data-stu-id="5eeb3-144">Int32</span></span>|<span data-ttu-id="5eeb3-145">设置的设备不适用计数</span><span class="sxs-lookup"><span data-stu-id="5eeb3-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="5eeb3-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eeb3-146">compliantDeviceCount</span></span>|<span data-ttu-id="5eeb3-147">Int32</span><span class="sxs-lookup"><span data-stu-id="5eeb3-147">Int32</span></span>|<span data-ttu-id="5eeb3-148">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="5eeb3-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="5eeb3-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eeb3-149">remediatedDeviceCount</span></span>|<span data-ttu-id="5eeb3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5eeb3-150">Int32</span></span>|<span data-ttu-id="5eeb3-151">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="5eeb3-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="5eeb3-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eeb3-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="5eeb3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5eeb3-153">Int32</span></span>|<span data-ttu-id="5eeb3-154">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="5eeb3-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="5eeb3-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eeb3-155">errorDeviceCount</span></span>|<span data-ttu-id="5eeb3-156">Int32</span><span class="sxs-lookup"><span data-stu-id="5eeb3-156">Int32</span></span>|<span data-ttu-id="5eeb3-157">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="5eeb3-157">Device error count for the setting</span></span>|
|<span data-ttu-id="5eeb3-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eeb3-158">conflictDeviceCount</span></span>|<span data-ttu-id="5eeb3-159">Int32</span><span class="sxs-lookup"><span data-stu-id="5eeb3-159">Int32</span></span>|<span data-ttu-id="5eeb3-160">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="5eeb3-160">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="5eeb3-161">关系</span><span class="sxs-lookup"><span data-stu-id="5eeb3-161">Relationships</span></span>
<span data-ttu-id="5eeb3-162">无</span><span class="sxs-lookup"><span data-stu-id="5eeb3-162">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5eeb3-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5eeb3-163">JSON Representation</span></span>
<span data-ttu-id="5eeb3-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5eeb3-164">Here is a JSON representation of the resource.</span></span>
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





