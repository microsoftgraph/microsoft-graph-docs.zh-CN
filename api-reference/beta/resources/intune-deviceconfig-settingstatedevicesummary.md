---
title: settingStateDeviceSummary 资源类型
description: 设置状态的设备合规性策略和配置摘要
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fab849fa44c33996d31ddac15b44c23f8450988d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414835"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="b43fd-103">settingStateDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="b43fd-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="b43fd-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b43fd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b43fd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b43fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b43fd-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b43fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b43fd-107">设置状态的设备合规性策略和配置摘要</span><span class="sxs-lookup"><span data-stu-id="b43fd-107">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="b43fd-108">方法</span><span class="sxs-lookup"><span data-stu-id="b43fd-108">Methods</span></span>
|<span data-ttu-id="b43fd-109">方法</span><span class="sxs-lookup"><span data-stu-id="b43fd-109">Method</span></span>|<span data-ttu-id="b43fd-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b43fd-110">Return Type</span></span>|<span data-ttu-id="b43fd-111">说明</span><span class="sxs-lookup"><span data-stu-id="b43fd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b43fd-112">列出 settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="b43fd-112">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="b43fd-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b43fd-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="b43fd-114">列出 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b43fd-114">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="b43fd-115">获取 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="b43fd-115">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="b43fd-116">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="b43fd-116">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="b43fd-117">读取 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b43fd-117">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="b43fd-118">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="b43fd-118">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="b43fd-119">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="b43fd-119">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="b43fd-120">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b43fd-120">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="b43fd-121">删除 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="b43fd-121">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="b43fd-122">无</span><span class="sxs-lookup"><span data-stu-id="b43fd-122">None</span></span>|<span data-ttu-id="b43fd-123">删除 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="b43fd-123">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="b43fd-124">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="b43fd-124">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="b43fd-125">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="b43fd-125">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="b43fd-126">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b43fd-126">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b43fd-127">属性</span><span class="sxs-lookup"><span data-stu-id="b43fd-127">Properties</span></span>
|<span data-ttu-id="b43fd-128">属性</span><span class="sxs-lookup"><span data-stu-id="b43fd-128">Property</span></span>|<span data-ttu-id="b43fd-129">类型</span><span class="sxs-lookup"><span data-stu-id="b43fd-129">Type</span></span>|<span data-ttu-id="b43fd-130">说明</span><span class="sxs-lookup"><span data-stu-id="b43fd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b43fd-131">id</span><span class="sxs-lookup"><span data-stu-id="b43fd-131">id</span></span>|<span data-ttu-id="b43fd-132">String</span><span class="sxs-lookup"><span data-stu-id="b43fd-132">String</span></span>|<span data-ttu-id="b43fd-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b43fd-133">Key of the entity.</span></span>|
|<span data-ttu-id="b43fd-134">settingName</span><span class="sxs-lookup"><span data-stu-id="b43fd-134">settingName</span></span>|<span data-ttu-id="b43fd-135">String</span><span class="sxs-lookup"><span data-stu-id="b43fd-135">String</span></span>|<span data-ttu-id="b43fd-136">设置的名称</span><span class="sxs-lookup"><span data-stu-id="b43fd-136">Name of the setting</span></span>|
|<span data-ttu-id="b43fd-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="b43fd-137">instancePath</span></span>|<span data-ttu-id="b43fd-138">String</span><span class="sxs-lookup"><span data-stu-id="b43fd-138">String</span></span>|<span data-ttu-id="b43fd-139">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="b43fd-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="b43fd-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b43fd-140">unknownDeviceCount</span></span>|<span data-ttu-id="b43fd-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b43fd-141">Int32</span></span>|<span data-ttu-id="b43fd-142">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="b43fd-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="b43fd-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b43fd-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="b43fd-144">Int32</span><span class="sxs-lookup"><span data-stu-id="b43fd-144">Int32</span></span>|<span data-ttu-id="b43fd-145">设置的设备不适用计数</span><span class="sxs-lookup"><span data-stu-id="b43fd-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="b43fd-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b43fd-146">compliantDeviceCount</span></span>|<span data-ttu-id="b43fd-147">Int32</span><span class="sxs-lookup"><span data-stu-id="b43fd-147">Int32</span></span>|<span data-ttu-id="b43fd-148">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="b43fd-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="b43fd-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b43fd-149">remediatedDeviceCount</span></span>|<span data-ttu-id="b43fd-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b43fd-150">Int32</span></span>|<span data-ttu-id="b43fd-151">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="b43fd-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="b43fd-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b43fd-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="b43fd-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b43fd-153">Int32</span></span>|<span data-ttu-id="b43fd-154">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="b43fd-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="b43fd-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b43fd-155">errorDeviceCount</span></span>|<span data-ttu-id="b43fd-156">Int32</span><span class="sxs-lookup"><span data-stu-id="b43fd-156">Int32</span></span>|<span data-ttu-id="b43fd-157">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="b43fd-157">Device error count for the setting</span></span>|
|<span data-ttu-id="b43fd-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b43fd-158">conflictDeviceCount</span></span>|<span data-ttu-id="b43fd-159">Int32</span><span class="sxs-lookup"><span data-stu-id="b43fd-159">Int32</span></span>|<span data-ttu-id="b43fd-160">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="b43fd-160">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="b43fd-161">关系</span><span class="sxs-lookup"><span data-stu-id="b43fd-161">Relationships</span></span>
<span data-ttu-id="b43fd-162">无</span><span class="sxs-lookup"><span data-stu-id="b43fd-162">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b43fd-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b43fd-163">JSON Representation</span></span>
<span data-ttu-id="b43fd-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b43fd-164">Here is a JSON representation of the resource.</span></span>
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




