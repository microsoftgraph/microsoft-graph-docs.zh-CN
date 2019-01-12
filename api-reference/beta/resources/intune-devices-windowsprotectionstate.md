---
title: windowsProtectionState 资源类型
description: 设备的保护状态实体。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f15044f597fb04e98571de7aec8796e9a9ddf74
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954524"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="5dfdd-103">windowsProtectionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="5dfdd-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="5dfdd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5dfdd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5dfdd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5dfdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5dfdd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5dfdd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5dfdd-107">设备的保护状态实体。</span><span class="sxs-lookup"><span data-stu-id="5dfdd-107">Device protection status entity.</span></span>
## <a name="methods"></a><span data-ttu-id="5dfdd-108">方法</span><span class="sxs-lookup"><span data-stu-id="5dfdd-108">Methods</span></span>
|<span data-ttu-id="5dfdd-109">方法</span><span class="sxs-lookup"><span data-stu-id="5dfdd-109">Method</span></span>|<span data-ttu-id="5dfdd-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5dfdd-110">Return Type</span></span>|<span data-ttu-id="5dfdd-111">说明</span><span class="sxs-lookup"><span data-stu-id="5dfdd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5dfdd-112">获取 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5dfdd-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="5dfdd-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5dfdd-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="5dfdd-114">读取属性和[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="5dfdd-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="5dfdd-115">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5dfdd-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="5dfdd-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5dfdd-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="5dfdd-117">更新[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5dfdd-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5dfdd-118">属性</span><span class="sxs-lookup"><span data-stu-id="5dfdd-118">Properties</span></span>
|<span data-ttu-id="5dfdd-119">属性</span><span class="sxs-lookup"><span data-stu-id="5dfdd-119">Property</span></span>|<span data-ttu-id="5dfdd-120">类型</span><span class="sxs-lookup"><span data-stu-id="5dfdd-120">Type</span></span>|<span data-ttu-id="5dfdd-121">说明</span><span class="sxs-lookup"><span data-stu-id="5dfdd-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dfdd-122">id</span><span class="sxs-lookup"><span data-stu-id="5dfdd-122">id</span></span>|<span data-ttu-id="5dfdd-123">字符串</span><span class="sxs-lookup"><span data-stu-id="5dfdd-123">String</span></span>|<span data-ttu-id="5dfdd-124">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5dfdd-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="5dfdd-125">这是设备的设备 id</span><span class="sxs-lookup"><span data-stu-id="5dfdd-125">This is device id of the device</span></span>|
|<span data-ttu-id="5dfdd-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5dfdd-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="5dfdd-127">布尔</span><span class="sxs-lookup"><span data-stu-id="5dfdd-127">Boolean</span></span>|<span data-ttu-id="5dfdd-128">反恶意软件被启用还是没有</span><span class="sxs-lookup"><span data-stu-id="5dfdd-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="5dfdd-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="5dfdd-129">deviceState</span></span>|[<span data-ttu-id="5dfdd-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="5dfdd-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="5dfdd-131">计算机的状态 （如清理挂起完全扫描或挂起的重新启动等）。</span><span class="sxs-lookup"><span data-stu-id="5dfdd-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="5dfdd-132">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="5dfdd-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="5dfdd-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5dfdd-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="5dfdd-134">布尔</span><span class="sxs-lookup"><span data-stu-id="5dfdd-134">Boolean</span></span>|<span data-ttu-id="5dfdd-135">是否启用实时保护？</span><span class="sxs-lookup"><span data-stu-id="5dfdd-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="5dfdd-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="5dfdd-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="5dfdd-137">布尔</span><span class="sxs-lookup"><span data-stu-id="5dfdd-137">Boolean</span></span>|<span data-ttu-id="5dfdd-138">启用或不网络检查系统？</span><span class="sxs-lookup"><span data-stu-id="5dfdd-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="5dfdd-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="5dfdd-139">quickScanOverdue</span></span>|<span data-ttu-id="5dfdd-140">布尔</span><span class="sxs-lookup"><span data-stu-id="5dfdd-140">Boolean</span></span>|<span data-ttu-id="5dfdd-141">快速扫描过期，或不？</span><span class="sxs-lookup"><span data-stu-id="5dfdd-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="5dfdd-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="5dfdd-142">fullScanOverdue</span></span>|<span data-ttu-id="5dfdd-143">布尔</span><span class="sxs-lookup"><span data-stu-id="5dfdd-143">Boolean</span></span>|<span data-ttu-id="5dfdd-144">或不完全扫描过期？</span><span class="sxs-lookup"><span data-stu-id="5dfdd-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="5dfdd-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="5dfdd-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="5dfdd-146">布尔</span><span class="sxs-lookup"><span data-stu-id="5dfdd-146">Boolean</span></span>|<span data-ttu-id="5dfdd-147">过期的签名或不？</span><span class="sxs-lookup"><span data-stu-id="5dfdd-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="5dfdd-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="5dfdd-148">rebootRequired</span></span>|<span data-ttu-id="5dfdd-149">布尔</span><span class="sxs-lookup"><span data-stu-id="5dfdd-149">Boolean</span></span>|<span data-ttu-id="5dfdd-150">需要或不重新启动？</span><span class="sxs-lookup"><span data-stu-id="5dfdd-150">Reboot required or not?</span></span>|
|<span data-ttu-id="5dfdd-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="5dfdd-151">fullScanRequired</span></span>|<span data-ttu-id="5dfdd-152">布尔</span><span class="sxs-lookup"><span data-stu-id="5dfdd-152">Boolean</span></span>|<span data-ttu-id="5dfdd-153">所需或不完全扫描？</span><span class="sxs-lookup"><span data-stu-id="5dfdd-153">Full scan required or not?</span></span>|
|<span data-ttu-id="5dfdd-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="5dfdd-154">engineVersion</span></span>|<span data-ttu-id="5dfdd-155">字符串</span><span class="sxs-lookup"><span data-stu-id="5dfdd-155">String</span></span>|<span data-ttu-id="5dfdd-156">当前终结点保护引擎的版本</span><span class="sxs-lookup"><span data-stu-id="5dfdd-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="5dfdd-157">特征码版本</span><span class="sxs-lookup"><span data-stu-id="5dfdd-157">signatureVersion</span></span>|<span data-ttu-id="5dfdd-158">字符串</span><span class="sxs-lookup"><span data-stu-id="5dfdd-158">String</span></span>|<span data-ttu-id="5dfdd-159">当前的恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="5dfdd-159">Current malware definitions version</span></span>|
|<span data-ttu-id="5dfdd-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="5dfdd-160">antiMalwareVersion</span></span>|<span data-ttu-id="5dfdd-161">字符串</span><span class="sxs-lookup"><span data-stu-id="5dfdd-161">String</span></span>|<span data-ttu-id="5dfdd-162">当前防恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="5dfdd-162">Current anti malware version</span></span>|
|<span data-ttu-id="5dfdd-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="5dfdd-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="5dfdd-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dfdd-164">DateTimeOffset</span></span>|<span data-ttu-id="5dfdd-165">最后一个快速扫描 datetime</span><span class="sxs-lookup"><span data-stu-id="5dfdd-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="5dfdd-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="5dfdd-166">lastFullScanDateTime</span></span>|<span data-ttu-id="5dfdd-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dfdd-167">DateTimeOffset</span></span>|<span data-ttu-id="5dfdd-168">最后一个快速扫描 datetime</span><span class="sxs-lookup"><span data-stu-id="5dfdd-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="5dfdd-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="5dfdd-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="5dfdd-170">字符串</span><span class="sxs-lookup"><span data-stu-id="5dfdd-170">String</span></span>|<span data-ttu-id="5dfdd-171">最后一个快速扫描病毒特征版本</span><span class="sxs-lookup"><span data-stu-id="5dfdd-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="5dfdd-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="5dfdd-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="5dfdd-173">字符串</span><span class="sxs-lookup"><span data-stu-id="5dfdd-173">String</span></span>|<span data-ttu-id="5dfdd-174">最后一个完全扫描病毒特征版本</span><span class="sxs-lookup"><span data-stu-id="5dfdd-174">Last full scan signature version</span></span>|
|<span data-ttu-id="5dfdd-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5dfdd-175">lastReportedDateTime</span></span>|<span data-ttu-id="5dfdd-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dfdd-176">DateTimeOffset</span></span>|<span data-ttu-id="5dfdd-177">最后一个设备运行状况状态报告的时间</span><span class="sxs-lookup"><span data-stu-id="5dfdd-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="5dfdd-178">Relationships</span><span class="sxs-lookup"><span data-stu-id="5dfdd-178">Relationships</span></span>
|<span data-ttu-id="5dfdd-179">关系</span><span class="sxs-lookup"><span data-stu-id="5dfdd-179">Relationship</span></span>|<span data-ttu-id="5dfdd-180">类型</span><span class="sxs-lookup"><span data-stu-id="5dfdd-180">Type</span></span>|<span data-ttu-id="5dfdd-181">Description</span><span class="sxs-lookup"><span data-stu-id="5dfdd-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dfdd-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="5dfdd-182">detectedMalwareState</span></span>|<span data-ttu-id="5dfdd-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="5dfdd-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="5dfdd-184">设备恶意软件的列表</span><span class="sxs-lookup"><span data-stu-id="5dfdd-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5dfdd-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5dfdd-185">JSON Representation</span></span>
<span data-ttu-id="5dfdd-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5dfdd-186">Here is a JSON representation of the resource.</span></span>
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





