---
title: settingStateDeviceSummary 资源类型
description: 设置状态的设备合规性策略和配置摘要
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f233b285fa9967dca03406c3ca7c649773e9832
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464934"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="59412-103">settingStateDeviceSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="59412-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="59412-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="59412-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59412-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="59412-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59412-106">设置状态的设备合规性策略和配置摘要</span><span class="sxs-lookup"><span data-stu-id="59412-106">Device Compilance Policy and Configuration for a Setting State summary</span></span>

## <a name="methods"></a><span data-ttu-id="59412-107">方法</span><span class="sxs-lookup"><span data-stu-id="59412-107">Methods</span></span>
|<span data-ttu-id="59412-108">方法</span><span class="sxs-lookup"><span data-stu-id="59412-108">Method</span></span>|<span data-ttu-id="59412-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="59412-109">Return Type</span></span>|<span data-ttu-id="59412-110">说明</span><span class="sxs-lookup"><span data-stu-id="59412-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="59412-111">列出 settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="59412-111">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="59412-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="59412-112">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="59412-113">列出 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="59412-113">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="59412-114">获取 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="59412-114">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="59412-115">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="59412-115">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="59412-116">读取 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="59412-116">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="59412-117">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="59412-117">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="59412-118">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="59412-118">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="59412-119">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59412-119">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="59412-120">删除 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="59412-120">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="59412-121">无</span><span class="sxs-lookup"><span data-stu-id="59412-121">None</span></span>|<span data-ttu-id="59412-122">删除 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="59412-122">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="59412-123">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="59412-123">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="59412-124">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="59412-124">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="59412-125">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="59412-125">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="59412-126">属性</span><span class="sxs-lookup"><span data-stu-id="59412-126">Properties</span></span>
|<span data-ttu-id="59412-127">属性</span><span class="sxs-lookup"><span data-stu-id="59412-127">Property</span></span>|<span data-ttu-id="59412-128">类型</span><span class="sxs-lookup"><span data-stu-id="59412-128">Type</span></span>|<span data-ttu-id="59412-129">说明</span><span class="sxs-lookup"><span data-stu-id="59412-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59412-130">id</span><span class="sxs-lookup"><span data-stu-id="59412-130">id</span></span>|<span data-ttu-id="59412-131">String</span><span class="sxs-lookup"><span data-stu-id="59412-131">String</span></span>|<span data-ttu-id="59412-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="59412-132">Key of the entity.</span></span>|
|<span data-ttu-id="59412-133">settingName</span><span class="sxs-lookup"><span data-stu-id="59412-133">settingName</span></span>|<span data-ttu-id="59412-134">字符串</span><span class="sxs-lookup"><span data-stu-id="59412-134">String</span></span>|<span data-ttu-id="59412-135">设置的名称</span><span class="sxs-lookup"><span data-stu-id="59412-135">Name of the setting</span></span>|
|<span data-ttu-id="59412-136">instancePath</span><span class="sxs-lookup"><span data-stu-id="59412-136">instancePath</span></span>|<span data-ttu-id="59412-137">String</span><span class="sxs-lookup"><span data-stu-id="59412-137">String</span></span>|<span data-ttu-id="59412-138">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="59412-138">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="59412-139">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59412-139">unknownDeviceCount</span></span>|<span data-ttu-id="59412-140">Int32</span><span class="sxs-lookup"><span data-stu-id="59412-140">Int32</span></span>|<span data-ttu-id="59412-141">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="59412-141">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="59412-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59412-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="59412-143">Int32</span><span class="sxs-lookup"><span data-stu-id="59412-143">Int32</span></span>|<span data-ttu-id="59412-144">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="59412-144">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="59412-145">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59412-145">compliantDeviceCount</span></span>|<span data-ttu-id="59412-146">Int32</span><span class="sxs-lookup"><span data-stu-id="59412-146">Int32</span></span>|<span data-ttu-id="59412-147">设置的设备符合计数</span><span class="sxs-lookup"><span data-stu-id="59412-147">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="59412-148">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59412-148">remediatedDeviceCount</span></span>|<span data-ttu-id="59412-149">Int32</span><span class="sxs-lookup"><span data-stu-id="59412-149">Int32</span></span>|<span data-ttu-id="59412-150">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="59412-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="59412-151">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59412-151">nonCompliantDeviceCount</span></span>|<span data-ttu-id="59412-152">Int32</span><span class="sxs-lookup"><span data-stu-id="59412-152">Int32</span></span>|<span data-ttu-id="59412-153">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="59412-153">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="59412-154">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59412-154">errorDeviceCount</span></span>|<span data-ttu-id="59412-155">Int32</span><span class="sxs-lookup"><span data-stu-id="59412-155">Int32</span></span>|<span data-ttu-id="59412-156">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="59412-156">Device error count for the setting</span></span>|
|<span data-ttu-id="59412-157">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59412-157">conflictDeviceCount</span></span>|<span data-ttu-id="59412-158">Int32</span><span class="sxs-lookup"><span data-stu-id="59412-158">Int32</span></span>|<span data-ttu-id="59412-159">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="59412-159">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="59412-160">关系</span><span class="sxs-lookup"><span data-stu-id="59412-160">Relationships</span></span>
<span data-ttu-id="59412-161">无</span><span class="sxs-lookup"><span data-stu-id="59412-161">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59412-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59412-162">JSON Representation</span></span>
<span data-ttu-id="59412-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59412-163">Here is a JSON representation of the resource.</span></span>
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





