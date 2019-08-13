---
title: windowsProtectionState 资源类型
description: 设备保护状态实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2710d1085cca36f84331a1a89e1307e5475db427
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365186"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="f914c-103">windowsProtectionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="f914c-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="f914c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f914c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f914c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f914c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f914c-106">设备保护状态实体。</span><span class="sxs-lookup"><span data-stu-id="f914c-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="f914c-107">方法</span><span class="sxs-lookup"><span data-stu-id="f914c-107">Methods</span></span>
|<span data-ttu-id="f914c-108">方法</span><span class="sxs-lookup"><span data-stu-id="f914c-108">Method</span></span>|<span data-ttu-id="f914c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f914c-109">Return Type</span></span>|<span data-ttu-id="f914c-110">说明</span><span class="sxs-lookup"><span data-stu-id="f914c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f914c-111">获取 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f914c-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="f914c-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f914c-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="f914c-113">读取[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f914c-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="f914c-114">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f914c-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="f914c-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f914c-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="f914c-116">更新[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f914c-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f914c-117">属性</span><span class="sxs-lookup"><span data-stu-id="f914c-117">Properties</span></span>
|<span data-ttu-id="f914c-118">属性</span><span class="sxs-lookup"><span data-stu-id="f914c-118">Property</span></span>|<span data-ttu-id="f914c-119">类型</span><span class="sxs-lookup"><span data-stu-id="f914c-119">Type</span></span>|<span data-ttu-id="f914c-120">说明</span><span class="sxs-lookup"><span data-stu-id="f914c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f914c-121">id</span><span class="sxs-lookup"><span data-stu-id="f914c-121">id</span></span>|<span data-ttu-id="f914c-122">String</span><span class="sxs-lookup"><span data-stu-id="f914c-122">String</span></span>|<span data-ttu-id="f914c-123">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f914c-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="f914c-124">这是设备的设备 id</span><span class="sxs-lookup"><span data-stu-id="f914c-124">This is device id of the device</span></span>|
|<span data-ttu-id="f914c-125">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f914c-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="f914c-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="f914c-126">Boolean</span></span>|<span data-ttu-id="f914c-127">已启用反恶意软件</span><span class="sxs-lookup"><span data-stu-id="f914c-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="f914c-128">deviceState</span><span class="sxs-lookup"><span data-stu-id="f914c-128">deviceState</span></span>|[<span data-ttu-id="f914c-129">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="f914c-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="f914c-130">计算机的状态 (如清理或挂起完全扫描或等待重新启动等)。</span><span class="sxs-lookup"><span data-stu-id="f914c-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="f914c-131">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="f914c-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="f914c-132">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f914c-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="f914c-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="f914c-133">Boolean</span></span>|<span data-ttu-id="f914c-134">是否启用了实时保护？</span><span class="sxs-lookup"><span data-stu-id="f914c-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="f914c-135">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="f914c-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="f914c-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="f914c-136">Boolean</span></span>|<span data-ttu-id="f914c-137">网络检查系统是否已启用？</span><span class="sxs-lookup"><span data-stu-id="f914c-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="f914c-138">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="f914c-138">quickScanOverdue</span></span>|<span data-ttu-id="f914c-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="f914c-139">Boolean</span></span>|<span data-ttu-id="f914c-140">快速扫描是否过期？</span><span class="sxs-lookup"><span data-stu-id="f914c-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="f914c-141">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="f914c-141">fullScanOverdue</span></span>|<span data-ttu-id="f914c-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f914c-142">Boolean</span></span>|<span data-ttu-id="f914c-143">完全扫描逾期？</span><span class="sxs-lookup"><span data-stu-id="f914c-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="f914c-144">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="f914c-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="f914c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f914c-145">Boolean</span></span>|<span data-ttu-id="f914c-146">签名是否已过期？</span><span class="sxs-lookup"><span data-stu-id="f914c-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="f914c-147">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="f914c-147">rebootRequired</span></span>|<span data-ttu-id="f914c-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="f914c-148">Boolean</span></span>|<span data-ttu-id="f914c-149">是否需要重新启动？</span><span class="sxs-lookup"><span data-stu-id="f914c-149">Reboot required or not?</span></span>|
|<span data-ttu-id="f914c-150">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="f914c-150">fullScanRequired</span></span>|<span data-ttu-id="f914c-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="f914c-151">Boolean</span></span>|<span data-ttu-id="f914c-152">需要完全扫描吗？</span><span class="sxs-lookup"><span data-stu-id="f914c-152">Full scan required or not?</span></span>|
|<span data-ttu-id="f914c-153">engineVersion</span><span class="sxs-lookup"><span data-stu-id="f914c-153">engineVersion</span></span>|<span data-ttu-id="f914c-154">String</span><span class="sxs-lookup"><span data-stu-id="f914c-154">String</span></span>|<span data-ttu-id="f914c-155">当前 endpoint protection 引擎的版本</span><span class="sxs-lookup"><span data-stu-id="f914c-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="f914c-156">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="f914c-156">signatureVersion</span></span>|<span data-ttu-id="f914c-157">String</span><span class="sxs-lookup"><span data-stu-id="f914c-157">String</span></span>|<span data-ttu-id="f914c-158">当前恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="f914c-158">Current malware definitions version</span></span>|
|<span data-ttu-id="f914c-159">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="f914c-159">antiMalwareVersion</span></span>|<span data-ttu-id="f914c-160">String</span><span class="sxs-lookup"><span data-stu-id="f914c-160">String</span></span>|<span data-ttu-id="f914c-161">当前反恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="f914c-161">Current anti malware version</span></span>|
|<span data-ttu-id="f914c-162">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="f914c-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="f914c-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f914c-163">DateTimeOffset</span></span>|<span data-ttu-id="f914c-164">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="f914c-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="f914c-165">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="f914c-165">lastFullScanDateTime</span></span>|<span data-ttu-id="f914c-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f914c-166">DateTimeOffset</span></span>|<span data-ttu-id="f914c-167">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="f914c-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="f914c-168">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="f914c-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="f914c-169">String</span><span class="sxs-lookup"><span data-stu-id="f914c-169">String</span></span>|<span data-ttu-id="f914c-170">上次快速扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="f914c-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="f914c-171">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="f914c-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="f914c-172">String</span><span class="sxs-lookup"><span data-stu-id="f914c-172">String</span></span>|<span data-ttu-id="f914c-173">上次完全扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="f914c-173">Last full scan signature version</span></span>|
|<span data-ttu-id="f914c-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f914c-174">lastReportedDateTime</span></span>|<span data-ttu-id="f914c-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f914c-175">DateTimeOffset</span></span>|<span data-ttu-id="f914c-176">上次设备运行状况状态报告时间</span><span class="sxs-lookup"><span data-stu-id="f914c-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="f914c-177">关系</span><span class="sxs-lookup"><span data-stu-id="f914c-177">Relationships</span></span>
|<span data-ttu-id="f914c-178">关系</span><span class="sxs-lookup"><span data-stu-id="f914c-178">Relationship</span></span>|<span data-ttu-id="f914c-179">类型</span><span class="sxs-lookup"><span data-stu-id="f914c-179">Type</span></span>|<span data-ttu-id="f914c-180">说明</span><span class="sxs-lookup"><span data-stu-id="f914c-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f914c-181">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="f914c-181">detectedMalwareState</span></span>|<span data-ttu-id="f914c-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="f914c-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="f914c-183">设备恶意软件列表</span><span class="sxs-lookup"><span data-stu-id="f914c-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f914c-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f914c-184">JSON Representation</span></span>
<span data-ttu-id="f914c-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f914c-185">Here is a JSON representation of the resource.</span></span>
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



