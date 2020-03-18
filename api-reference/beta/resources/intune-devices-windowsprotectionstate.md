---
title: windowsProtectionState 资源类型
description: 设备保护状态实体。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d42efcc04a060d9585c8d02d17d72449ae0a9c8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783597"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="8f5df-103">windowsProtectionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f5df-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="8f5df-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8f5df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f5df-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8f5df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f5df-106">设备保护状态实体。</span><span class="sxs-lookup"><span data-stu-id="8f5df-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="8f5df-107">方法</span><span class="sxs-lookup"><span data-stu-id="8f5df-107">Methods</span></span>
|<span data-ttu-id="8f5df-108">方法</span><span class="sxs-lookup"><span data-stu-id="8f5df-108">Method</span></span>|<span data-ttu-id="8f5df-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8f5df-109">Return Type</span></span>|<span data-ttu-id="8f5df-110">说明</span><span class="sxs-lookup"><span data-stu-id="8f5df-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8f5df-111">获取 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="8f5df-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="8f5df-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="8f5df-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="8f5df-113">读取[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8f5df-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="8f5df-114">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="8f5df-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="8f5df-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="8f5df-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="8f5df-116">更新[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8f5df-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f5df-117">属性</span><span class="sxs-lookup"><span data-stu-id="8f5df-117">Properties</span></span>
|<span data-ttu-id="8f5df-118">属性</span><span class="sxs-lookup"><span data-stu-id="8f5df-118">Property</span></span>|<span data-ttu-id="8f5df-119">类型</span><span class="sxs-lookup"><span data-stu-id="8f5df-119">Type</span></span>|<span data-ttu-id="8f5df-120">说明</span><span class="sxs-lookup"><span data-stu-id="8f5df-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f5df-121">id</span><span class="sxs-lookup"><span data-stu-id="8f5df-121">id</span></span>|<span data-ttu-id="8f5df-122">String</span><span class="sxs-lookup"><span data-stu-id="8f5df-122">String</span></span>|<span data-ttu-id="8f5df-123">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8f5df-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="8f5df-124">这是设备的设备 id</span><span class="sxs-lookup"><span data-stu-id="8f5df-124">This is device id of the device</span></span>|
|<span data-ttu-id="8f5df-125">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="8f5df-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="8f5df-126">布尔值</span><span class="sxs-lookup"><span data-stu-id="8f5df-126">Boolean</span></span>|<span data-ttu-id="8f5df-127">已启用反恶意软件</span><span class="sxs-lookup"><span data-stu-id="8f5df-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="8f5df-128">deviceState</span><span class="sxs-lookup"><span data-stu-id="8f5df-128">deviceState</span></span>|[<span data-ttu-id="8f5df-129">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="8f5df-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="8f5df-130">计算机的状态（如清理或挂起完全扫描或等待重新启动等）。</span><span class="sxs-lookup"><span data-stu-id="8f5df-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="8f5df-131">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="8f5df-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="8f5df-132">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="8f5df-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="8f5df-133">布尔值</span><span class="sxs-lookup"><span data-stu-id="8f5df-133">Boolean</span></span>|<span data-ttu-id="8f5df-134">是否启用了实时保护？</span><span class="sxs-lookup"><span data-stu-id="8f5df-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="8f5df-135">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="8f5df-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="8f5df-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="8f5df-136">Boolean</span></span>|<span data-ttu-id="8f5df-137">网络检查系统是否已启用？</span><span class="sxs-lookup"><span data-stu-id="8f5df-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="8f5df-138">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="8f5df-138">quickScanOverdue</span></span>|<span data-ttu-id="8f5df-139">布尔值</span><span class="sxs-lookup"><span data-stu-id="8f5df-139">Boolean</span></span>|<span data-ttu-id="8f5df-140">快速扫描是否过期？</span><span class="sxs-lookup"><span data-stu-id="8f5df-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="8f5df-141">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="8f5df-141">fullScanOverdue</span></span>|<span data-ttu-id="8f5df-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="8f5df-142">Boolean</span></span>|<span data-ttu-id="8f5df-143">完全扫描逾期？</span><span class="sxs-lookup"><span data-stu-id="8f5df-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="8f5df-144">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="8f5df-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="8f5df-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="8f5df-145">Boolean</span></span>|<span data-ttu-id="8f5df-146">签名是否已过期？</span><span class="sxs-lookup"><span data-stu-id="8f5df-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="8f5df-147">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="8f5df-147">rebootRequired</span></span>|<span data-ttu-id="8f5df-148">布尔值</span><span class="sxs-lookup"><span data-stu-id="8f5df-148">Boolean</span></span>|<span data-ttu-id="8f5df-149">是否需要重新启动？</span><span class="sxs-lookup"><span data-stu-id="8f5df-149">Reboot required or not?</span></span>|
|<span data-ttu-id="8f5df-150">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="8f5df-150">fullScanRequired</span></span>|<span data-ttu-id="8f5df-151">布尔值</span><span class="sxs-lookup"><span data-stu-id="8f5df-151">Boolean</span></span>|<span data-ttu-id="8f5df-152">需要完全扫描吗？</span><span class="sxs-lookup"><span data-stu-id="8f5df-152">Full scan required or not?</span></span>|
|<span data-ttu-id="8f5df-153">engineVersion</span><span class="sxs-lookup"><span data-stu-id="8f5df-153">engineVersion</span></span>|<span data-ttu-id="8f5df-154">String</span><span class="sxs-lookup"><span data-stu-id="8f5df-154">String</span></span>|<span data-ttu-id="8f5df-155">当前 endpoint protection 引擎的版本</span><span class="sxs-lookup"><span data-stu-id="8f5df-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="8f5df-156">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="8f5df-156">signatureVersion</span></span>|<span data-ttu-id="8f5df-157">String</span><span class="sxs-lookup"><span data-stu-id="8f5df-157">String</span></span>|<span data-ttu-id="8f5df-158">当前恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="8f5df-158">Current malware definitions version</span></span>|
|<span data-ttu-id="8f5df-159">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="8f5df-159">antiMalwareVersion</span></span>|<span data-ttu-id="8f5df-160">String</span><span class="sxs-lookup"><span data-stu-id="8f5df-160">String</span></span>|<span data-ttu-id="8f5df-161">当前反恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="8f5df-161">Current anti malware version</span></span>|
|<span data-ttu-id="8f5df-162">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="8f5df-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="8f5df-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f5df-163">DateTimeOffset</span></span>|<span data-ttu-id="8f5df-164">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="8f5df-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="8f5df-165">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="8f5df-165">lastFullScanDateTime</span></span>|<span data-ttu-id="8f5df-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f5df-166">DateTimeOffset</span></span>|<span data-ttu-id="8f5df-167">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="8f5df-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="8f5df-168">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="8f5df-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="8f5df-169">String</span><span class="sxs-lookup"><span data-stu-id="8f5df-169">String</span></span>|<span data-ttu-id="8f5df-170">上次快速扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="8f5df-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="8f5df-171">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="8f5df-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="8f5df-172">String</span><span class="sxs-lookup"><span data-stu-id="8f5df-172">String</span></span>|<span data-ttu-id="8f5df-173">上次完全扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="8f5df-173">Last full scan signature version</span></span>|
|<span data-ttu-id="8f5df-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f5df-174">lastReportedDateTime</span></span>|<span data-ttu-id="8f5df-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f5df-175">DateTimeOffset</span></span>|<span data-ttu-id="8f5df-176">上次设备运行状况状态报告时间</span><span class="sxs-lookup"><span data-stu-id="8f5df-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f5df-177">关系</span><span class="sxs-lookup"><span data-stu-id="8f5df-177">Relationships</span></span>
|<span data-ttu-id="8f5df-178">关系</span><span class="sxs-lookup"><span data-stu-id="8f5df-178">Relationship</span></span>|<span data-ttu-id="8f5df-179">类型</span><span class="sxs-lookup"><span data-stu-id="8f5df-179">Type</span></span>|<span data-ttu-id="8f5df-180">说明</span><span class="sxs-lookup"><span data-stu-id="8f5df-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f5df-181">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="8f5df-181">detectedMalwareState</span></span>|<span data-ttu-id="8f5df-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="8f5df-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="8f5df-183">设备恶意软件列表</span><span class="sxs-lookup"><span data-stu-id="8f5df-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f5df-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f5df-184">JSON Representation</span></span>
<span data-ttu-id="8f5df-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f5df-185">Here is a JSON representation of the resource.</span></span>
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



