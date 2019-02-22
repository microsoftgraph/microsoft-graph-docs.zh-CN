---
title: windowsProtectionState 资源类型
description: 设备保护状态实体。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eebf798a41e5cbab27fab849cdead8a288a782e2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148312"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="e8cd8-103">windowsProtectionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8cd8-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="e8cd8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e8cd8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8cd8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8cd8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8cd8-106">设备保护状态实体。</span><span class="sxs-lookup"><span data-stu-id="e8cd8-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="e8cd8-107">方法</span><span class="sxs-lookup"><span data-stu-id="e8cd8-107">Methods</span></span>
|<span data-ttu-id="e8cd8-108">方法</span><span class="sxs-lookup"><span data-stu-id="e8cd8-108">Method</span></span>|<span data-ttu-id="e8cd8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e8cd8-109">Return Type</span></span>|<span data-ttu-id="e8cd8-110">说明</span><span class="sxs-lookup"><span data-stu-id="e8cd8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e8cd8-111">获取 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="e8cd8-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="e8cd8-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="e8cd8-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="e8cd8-113">读取[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e8cd8-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="e8cd8-114">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="e8cd8-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="e8cd8-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="e8cd8-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="e8cd8-116">更新[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e8cd8-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e8cd8-117">属性</span><span class="sxs-lookup"><span data-stu-id="e8cd8-117">Properties</span></span>
|<span data-ttu-id="e8cd8-118">属性</span><span class="sxs-lookup"><span data-stu-id="e8cd8-118">Property</span></span>|<span data-ttu-id="e8cd8-119">类型</span><span class="sxs-lookup"><span data-stu-id="e8cd8-119">Type</span></span>|<span data-ttu-id="e8cd8-120">说明</span><span class="sxs-lookup"><span data-stu-id="e8cd8-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8cd8-121">id</span><span class="sxs-lookup"><span data-stu-id="e8cd8-121">id</span></span>|<span data-ttu-id="e8cd8-122">字符串</span><span class="sxs-lookup"><span data-stu-id="e8cd8-122">String</span></span>|<span data-ttu-id="e8cd8-123">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e8cd8-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="e8cd8-124">这是设备的设备 id</span><span class="sxs-lookup"><span data-stu-id="e8cd8-124">This is device id of the device</span></span>|
|<span data-ttu-id="e8cd8-125">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e8cd8-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="e8cd8-126">布尔</span><span class="sxs-lookup"><span data-stu-id="e8cd8-126">Boolean</span></span>|<span data-ttu-id="e8cd8-127">已启用反恶意软件</span><span class="sxs-lookup"><span data-stu-id="e8cd8-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="e8cd8-128">deviceState</span><span class="sxs-lookup"><span data-stu-id="e8cd8-128">deviceState</span></span>|[<span data-ttu-id="e8cd8-129">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="e8cd8-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="e8cd8-130">计算机的状态 (如清理或挂起完全扫描或等待重新启动等)。</span><span class="sxs-lookup"><span data-stu-id="e8cd8-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="e8cd8-131">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="e8cd8-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="e8cd8-132">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e8cd8-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="e8cd8-133">布尔</span><span class="sxs-lookup"><span data-stu-id="e8cd8-133">Boolean</span></span>|<span data-ttu-id="e8cd8-134">是否启用了实时保护？</span><span class="sxs-lookup"><span data-stu-id="e8cd8-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="e8cd8-135">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="e8cd8-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="e8cd8-136">布尔</span><span class="sxs-lookup"><span data-stu-id="e8cd8-136">Boolean</span></span>|<span data-ttu-id="e8cd8-137">网络检查系统是否已启用？</span><span class="sxs-lookup"><span data-stu-id="e8cd8-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="e8cd8-138">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="e8cd8-138">quickScanOverdue</span></span>|<span data-ttu-id="e8cd8-139">布尔</span><span class="sxs-lookup"><span data-stu-id="e8cd8-139">Boolean</span></span>|<span data-ttu-id="e8cd8-140">快速扫描是否过期？</span><span class="sxs-lookup"><span data-stu-id="e8cd8-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="e8cd8-141">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="e8cd8-141">fullScanOverdue</span></span>|<span data-ttu-id="e8cd8-142">布尔</span><span class="sxs-lookup"><span data-stu-id="e8cd8-142">Boolean</span></span>|<span data-ttu-id="e8cd8-143">完全扫描逾期？</span><span class="sxs-lookup"><span data-stu-id="e8cd8-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="e8cd8-144">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="e8cd8-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="e8cd8-145">布尔</span><span class="sxs-lookup"><span data-stu-id="e8cd8-145">Boolean</span></span>|<span data-ttu-id="e8cd8-146">签名是否已过期？</span><span class="sxs-lookup"><span data-stu-id="e8cd8-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="e8cd8-147">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="e8cd8-147">rebootRequired</span></span>|<span data-ttu-id="e8cd8-148">布尔</span><span class="sxs-lookup"><span data-stu-id="e8cd8-148">Boolean</span></span>|<span data-ttu-id="e8cd8-149">是否需要重新启动？</span><span class="sxs-lookup"><span data-stu-id="e8cd8-149">Reboot required or not?</span></span>|
|<span data-ttu-id="e8cd8-150">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="e8cd8-150">fullScanRequired</span></span>|<span data-ttu-id="e8cd8-151">布尔</span><span class="sxs-lookup"><span data-stu-id="e8cd8-151">Boolean</span></span>|<span data-ttu-id="e8cd8-152">需要完全扫描吗？</span><span class="sxs-lookup"><span data-stu-id="e8cd8-152">Full scan required or not?</span></span>|
|<span data-ttu-id="e8cd8-153">engineVersion</span><span class="sxs-lookup"><span data-stu-id="e8cd8-153">engineVersion</span></span>|<span data-ttu-id="e8cd8-154">字符串</span><span class="sxs-lookup"><span data-stu-id="e8cd8-154">String</span></span>|<span data-ttu-id="e8cd8-155">当前 endpoint protection 引擎的版本</span><span class="sxs-lookup"><span data-stu-id="e8cd8-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="e8cd8-156">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="e8cd8-156">signatureVersion</span></span>|<span data-ttu-id="e8cd8-157">字符串</span><span class="sxs-lookup"><span data-stu-id="e8cd8-157">String</span></span>|<span data-ttu-id="e8cd8-158">当前恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="e8cd8-158">Current malware definitions version</span></span>|
|<span data-ttu-id="e8cd8-159">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="e8cd8-159">antiMalwareVersion</span></span>|<span data-ttu-id="e8cd8-160">字符串</span><span class="sxs-lookup"><span data-stu-id="e8cd8-160">String</span></span>|<span data-ttu-id="e8cd8-161">当前反恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="e8cd8-161">Current anti malware version</span></span>|
|<span data-ttu-id="e8cd8-162">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="e8cd8-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="e8cd8-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8cd8-163">DateTimeOffset</span></span>|<span data-ttu-id="e8cd8-164">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="e8cd8-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="e8cd8-165">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="e8cd8-165">lastFullScanDateTime</span></span>|<span data-ttu-id="e8cd8-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8cd8-166">DateTimeOffset</span></span>|<span data-ttu-id="e8cd8-167">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="e8cd8-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="e8cd8-168">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="e8cd8-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="e8cd8-169">字符串</span><span class="sxs-lookup"><span data-stu-id="e8cd8-169">String</span></span>|<span data-ttu-id="e8cd8-170">上次快速扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="e8cd8-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="e8cd8-171">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="e8cd8-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="e8cd8-172">字符串</span><span class="sxs-lookup"><span data-stu-id="e8cd8-172">String</span></span>|<span data-ttu-id="e8cd8-173">上次完全扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="e8cd8-173">Last full scan signature version</span></span>|
|<span data-ttu-id="e8cd8-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8cd8-174">lastReportedDateTime</span></span>|<span data-ttu-id="e8cd8-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8cd8-175">DateTimeOffset</span></span>|<span data-ttu-id="e8cd8-176">上次设备运行状况状态报告时间</span><span class="sxs-lookup"><span data-stu-id="e8cd8-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8cd8-177">关系</span><span class="sxs-lookup"><span data-stu-id="e8cd8-177">Relationships</span></span>
|<span data-ttu-id="e8cd8-178">关系</span><span class="sxs-lookup"><span data-stu-id="e8cd8-178">Relationship</span></span>|<span data-ttu-id="e8cd8-179">类型</span><span class="sxs-lookup"><span data-stu-id="e8cd8-179">Type</span></span>|<span data-ttu-id="e8cd8-180">说明</span><span class="sxs-lookup"><span data-stu-id="e8cd8-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8cd8-181">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="e8cd8-181">detectedMalwareState</span></span>|<span data-ttu-id="e8cd8-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="e8cd8-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="e8cd8-183">设备恶意软件列表</span><span class="sxs-lookup"><span data-stu-id="e8cd8-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8cd8-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8cd8-184">JSON Representation</span></span>
<span data-ttu-id="e8cd8-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8cd8-185">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```




