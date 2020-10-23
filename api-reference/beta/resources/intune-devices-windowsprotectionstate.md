---
title: windowsProtectionState 资源类型
description: 设备保护状态实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 63ac9a9e5f6dd153238ea2666cf0bffd88ebf9da
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731034"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="f1460-103">windowsProtectionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1460-103">windowsProtectionState resource type</span></span>

<span data-ttu-id="f1460-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1460-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1460-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1460-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1460-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1460-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1460-107">设备保护状态实体。</span><span class="sxs-lookup"><span data-stu-id="f1460-107">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="f1460-108">Methods</span><span class="sxs-lookup"><span data-stu-id="f1460-108">Methods</span></span>
|<span data-ttu-id="f1460-109">方法</span><span class="sxs-lookup"><span data-stu-id="f1460-109">Method</span></span>|<span data-ttu-id="f1460-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f1460-110">Return Type</span></span>|<span data-ttu-id="f1460-111">说明</span><span class="sxs-lookup"><span data-stu-id="f1460-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f1460-112">获取 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f1460-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="f1460-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f1460-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="f1460-114">读取 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f1460-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="f1460-115">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f1460-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="f1460-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f1460-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="f1460-117">更新 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f1460-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f1460-118">属性</span><span class="sxs-lookup"><span data-stu-id="f1460-118">Properties</span></span>
|<span data-ttu-id="f1460-119">属性</span><span class="sxs-lookup"><span data-stu-id="f1460-119">Property</span></span>|<span data-ttu-id="f1460-120">类型</span><span class="sxs-lookup"><span data-stu-id="f1460-120">Type</span></span>|<span data-ttu-id="f1460-121">说明</span><span class="sxs-lookup"><span data-stu-id="f1460-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1460-122">id</span><span class="sxs-lookup"><span data-stu-id="f1460-122">id</span></span>|<span data-ttu-id="f1460-123">String</span><span class="sxs-lookup"><span data-stu-id="f1460-123">String</span></span>|<span data-ttu-id="f1460-124">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f1460-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="f1460-125">这是设备的设备 id</span><span class="sxs-lookup"><span data-stu-id="f1460-125">This is device id of the device</span></span>|
|<span data-ttu-id="f1460-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f1460-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="f1460-127">布尔</span><span class="sxs-lookup"><span data-stu-id="f1460-127">Boolean</span></span>|<span data-ttu-id="f1460-128">已启用反恶意软件</span><span class="sxs-lookup"><span data-stu-id="f1460-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="f1460-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="f1460-129">deviceState</span></span>|[<span data-ttu-id="f1460-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="f1460-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="f1460-131">计算机的状态 (如干净或挂起的完全扫描或挂起的重新启动等) 。</span><span class="sxs-lookup"><span data-stu-id="f1460-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="f1460-132">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="f1460-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="f1460-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f1460-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="f1460-134">布尔</span><span class="sxs-lookup"><span data-stu-id="f1460-134">Boolean</span></span>|<span data-ttu-id="f1460-135">是否启用了实时保护？</span><span class="sxs-lookup"><span data-stu-id="f1460-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="f1460-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="f1460-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="f1460-137">布尔</span><span class="sxs-lookup"><span data-stu-id="f1460-137">Boolean</span></span>|<span data-ttu-id="f1460-138">网络检查系统是否已启用？</span><span class="sxs-lookup"><span data-stu-id="f1460-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="f1460-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="f1460-139">quickScanOverdue</span></span>|<span data-ttu-id="f1460-140">布尔</span><span class="sxs-lookup"><span data-stu-id="f1460-140">Boolean</span></span>|<span data-ttu-id="f1460-141">快速扫描是否过期？</span><span class="sxs-lookup"><span data-stu-id="f1460-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="f1460-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="f1460-142">fullScanOverdue</span></span>|<span data-ttu-id="f1460-143">布尔</span><span class="sxs-lookup"><span data-stu-id="f1460-143">Boolean</span></span>|<span data-ttu-id="f1460-144">完全扫描逾期？</span><span class="sxs-lookup"><span data-stu-id="f1460-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="f1460-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="f1460-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="f1460-146">布尔</span><span class="sxs-lookup"><span data-stu-id="f1460-146">Boolean</span></span>|<span data-ttu-id="f1460-147">签名是否已过期？</span><span class="sxs-lookup"><span data-stu-id="f1460-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="f1460-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="f1460-148">rebootRequired</span></span>|<span data-ttu-id="f1460-149">布尔</span><span class="sxs-lookup"><span data-stu-id="f1460-149">Boolean</span></span>|<span data-ttu-id="f1460-150">是否需要重新启动？</span><span class="sxs-lookup"><span data-stu-id="f1460-150">Reboot required or not?</span></span>|
|<span data-ttu-id="f1460-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="f1460-151">fullScanRequired</span></span>|<span data-ttu-id="f1460-152">布尔</span><span class="sxs-lookup"><span data-stu-id="f1460-152">Boolean</span></span>|<span data-ttu-id="f1460-153">需要完全扫描吗？</span><span class="sxs-lookup"><span data-stu-id="f1460-153">Full scan required or not?</span></span>|
|<span data-ttu-id="f1460-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="f1460-154">engineVersion</span></span>|<span data-ttu-id="f1460-155">String</span><span class="sxs-lookup"><span data-stu-id="f1460-155">String</span></span>|<span data-ttu-id="f1460-156">当前 endpoint protection 引擎的版本</span><span class="sxs-lookup"><span data-stu-id="f1460-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="f1460-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="f1460-157">signatureVersion</span></span>|<span data-ttu-id="f1460-158">String</span><span class="sxs-lookup"><span data-stu-id="f1460-158">String</span></span>|<span data-ttu-id="f1460-159">当前恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="f1460-159">Current malware definitions version</span></span>|
|<span data-ttu-id="f1460-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="f1460-160">antiMalwareVersion</span></span>|<span data-ttu-id="f1460-161">String</span><span class="sxs-lookup"><span data-stu-id="f1460-161">String</span></span>|<span data-ttu-id="f1460-162">当前反恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="f1460-162">Current anti malware version</span></span>|
|<span data-ttu-id="f1460-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="f1460-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="f1460-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1460-164">DateTimeOffset</span></span>|<span data-ttu-id="f1460-165">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="f1460-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="f1460-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="f1460-166">lastFullScanDateTime</span></span>|<span data-ttu-id="f1460-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1460-167">DateTimeOffset</span></span>|<span data-ttu-id="f1460-168">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="f1460-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="f1460-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="f1460-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="f1460-170">String</span><span class="sxs-lookup"><span data-stu-id="f1460-170">String</span></span>|<span data-ttu-id="f1460-171">上次快速扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="f1460-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="f1460-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="f1460-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="f1460-173">String</span><span class="sxs-lookup"><span data-stu-id="f1460-173">String</span></span>|<span data-ttu-id="f1460-174">上次完全扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="f1460-174">Last full scan signature version</span></span>|
|<span data-ttu-id="f1460-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1460-175">lastReportedDateTime</span></span>|<span data-ttu-id="f1460-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1460-176">DateTimeOffset</span></span>|<span data-ttu-id="f1460-177">上次设备运行状况状态报告时间</span><span class="sxs-lookup"><span data-stu-id="f1460-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1460-178">关系</span><span class="sxs-lookup"><span data-stu-id="f1460-178">Relationships</span></span>
|<span data-ttu-id="f1460-179">关系</span><span class="sxs-lookup"><span data-stu-id="f1460-179">Relationship</span></span>|<span data-ttu-id="f1460-180">类型</span><span class="sxs-lookup"><span data-stu-id="f1460-180">Type</span></span>|<span data-ttu-id="f1460-181">说明</span><span class="sxs-lookup"><span data-stu-id="f1460-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1460-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="f1460-182">detectedMalwareState</span></span>|<span data-ttu-id="f1460-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1460-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="f1460-184">设备恶意软件列表</span><span class="sxs-lookup"><span data-stu-id="f1460-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1460-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1460-185">JSON Representation</span></span>
<span data-ttu-id="f1460-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1460-186">Here is a JSON representation of the resource.</span></span>
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





