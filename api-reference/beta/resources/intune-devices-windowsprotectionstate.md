---
title: windowsProtectionState 资源类型
description: 设备保护状态实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd507daef4d9055dcabce1e90481e22a77ec8180
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983916"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="33114-103">windowsProtectionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="33114-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="33114-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="33114-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33114-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="33114-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33114-106">设备保护状态实体。</span><span class="sxs-lookup"><span data-stu-id="33114-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="33114-107">方法</span><span class="sxs-lookup"><span data-stu-id="33114-107">Methods</span></span>
|<span data-ttu-id="33114-108">方法</span><span class="sxs-lookup"><span data-stu-id="33114-108">Method</span></span>|<span data-ttu-id="33114-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="33114-109">Return Type</span></span>|<span data-ttu-id="33114-110">说明</span><span class="sxs-lookup"><span data-stu-id="33114-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="33114-111">获取 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="33114-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="33114-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="33114-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="33114-113">读取[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="33114-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="33114-114">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="33114-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="33114-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="33114-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="33114-116">更新[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="33114-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="33114-117">属性</span><span class="sxs-lookup"><span data-stu-id="33114-117">Properties</span></span>
|<span data-ttu-id="33114-118">属性</span><span class="sxs-lookup"><span data-stu-id="33114-118">Property</span></span>|<span data-ttu-id="33114-119">类型</span><span class="sxs-lookup"><span data-stu-id="33114-119">Type</span></span>|<span data-ttu-id="33114-120">说明</span><span class="sxs-lookup"><span data-stu-id="33114-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33114-121">id</span><span class="sxs-lookup"><span data-stu-id="33114-121">id</span></span>|<span data-ttu-id="33114-122">String</span><span class="sxs-lookup"><span data-stu-id="33114-122">String</span></span>|<span data-ttu-id="33114-123">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="33114-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="33114-124">这是设备的设备 id</span><span class="sxs-lookup"><span data-stu-id="33114-124">This is device id of the device</span></span>|
|<span data-ttu-id="33114-125">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="33114-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="33114-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="33114-126">Boolean</span></span>|<span data-ttu-id="33114-127">已启用反恶意软件</span><span class="sxs-lookup"><span data-stu-id="33114-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="33114-128">deviceState</span><span class="sxs-lookup"><span data-stu-id="33114-128">deviceState</span></span>|[<span data-ttu-id="33114-129">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="33114-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="33114-130">计算机的状态 (如清理或挂起完全扫描或等待重新启动等)。</span><span class="sxs-lookup"><span data-stu-id="33114-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="33114-131">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="33114-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="33114-132">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="33114-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="33114-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="33114-133">Boolean</span></span>|<span data-ttu-id="33114-134">是否启用了实时保护？</span><span class="sxs-lookup"><span data-stu-id="33114-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="33114-135">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="33114-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="33114-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="33114-136">Boolean</span></span>|<span data-ttu-id="33114-137">网络检查系统是否已启用？</span><span class="sxs-lookup"><span data-stu-id="33114-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="33114-138">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="33114-138">quickScanOverdue</span></span>|<span data-ttu-id="33114-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="33114-139">Boolean</span></span>|<span data-ttu-id="33114-140">快速扫描是否过期？</span><span class="sxs-lookup"><span data-stu-id="33114-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="33114-141">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="33114-141">fullScanOverdue</span></span>|<span data-ttu-id="33114-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="33114-142">Boolean</span></span>|<span data-ttu-id="33114-143">完全扫描逾期？</span><span class="sxs-lookup"><span data-stu-id="33114-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="33114-144">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="33114-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="33114-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="33114-145">Boolean</span></span>|<span data-ttu-id="33114-146">签名是否已过期？</span><span class="sxs-lookup"><span data-stu-id="33114-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="33114-147">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="33114-147">rebootRequired</span></span>|<span data-ttu-id="33114-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="33114-148">Boolean</span></span>|<span data-ttu-id="33114-149">是否需要重新启动？</span><span class="sxs-lookup"><span data-stu-id="33114-149">Reboot required or not?</span></span>|
|<span data-ttu-id="33114-150">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="33114-150">fullScanRequired</span></span>|<span data-ttu-id="33114-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="33114-151">Boolean</span></span>|<span data-ttu-id="33114-152">需要完全扫描吗？</span><span class="sxs-lookup"><span data-stu-id="33114-152">Full scan required or not?</span></span>|
|<span data-ttu-id="33114-153">engineVersion</span><span class="sxs-lookup"><span data-stu-id="33114-153">engineVersion</span></span>|<span data-ttu-id="33114-154">String</span><span class="sxs-lookup"><span data-stu-id="33114-154">String</span></span>|<span data-ttu-id="33114-155">当前 endpoint protection 引擎的版本</span><span class="sxs-lookup"><span data-stu-id="33114-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="33114-156">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="33114-156">signatureVersion</span></span>|<span data-ttu-id="33114-157">String</span><span class="sxs-lookup"><span data-stu-id="33114-157">String</span></span>|<span data-ttu-id="33114-158">当前恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="33114-158">Current malware definitions version</span></span>|
|<span data-ttu-id="33114-159">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="33114-159">antiMalwareVersion</span></span>|<span data-ttu-id="33114-160">String</span><span class="sxs-lookup"><span data-stu-id="33114-160">String</span></span>|<span data-ttu-id="33114-161">当前反恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="33114-161">Current anti malware version</span></span>|
|<span data-ttu-id="33114-162">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="33114-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="33114-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33114-163">DateTimeOffset</span></span>|<span data-ttu-id="33114-164">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="33114-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="33114-165">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="33114-165">lastFullScanDateTime</span></span>|<span data-ttu-id="33114-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33114-166">DateTimeOffset</span></span>|<span data-ttu-id="33114-167">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="33114-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="33114-168">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="33114-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="33114-169">String</span><span class="sxs-lookup"><span data-stu-id="33114-169">String</span></span>|<span data-ttu-id="33114-170">上次快速扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="33114-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="33114-171">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="33114-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="33114-172">String</span><span class="sxs-lookup"><span data-stu-id="33114-172">String</span></span>|<span data-ttu-id="33114-173">上次完全扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="33114-173">Last full scan signature version</span></span>|
|<span data-ttu-id="33114-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="33114-174">lastReportedDateTime</span></span>|<span data-ttu-id="33114-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33114-175">DateTimeOffset</span></span>|<span data-ttu-id="33114-176">上次设备运行状况状态报告时间</span><span class="sxs-lookup"><span data-stu-id="33114-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="33114-177">关系</span><span class="sxs-lookup"><span data-stu-id="33114-177">Relationships</span></span>
|<span data-ttu-id="33114-178">关系</span><span class="sxs-lookup"><span data-stu-id="33114-178">Relationship</span></span>|<span data-ttu-id="33114-179">类型</span><span class="sxs-lookup"><span data-stu-id="33114-179">Type</span></span>|<span data-ttu-id="33114-180">说明</span><span class="sxs-lookup"><span data-stu-id="33114-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33114-181">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="33114-181">detectedMalwareState</span></span>|<span data-ttu-id="33114-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="33114-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="33114-183">设备恶意软件列表</span><span class="sxs-lookup"><span data-stu-id="33114-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33114-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33114-184">JSON Representation</span></span>
<span data-ttu-id="33114-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33114-185">Here is a JSON representation of the resource.</span></span>
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





