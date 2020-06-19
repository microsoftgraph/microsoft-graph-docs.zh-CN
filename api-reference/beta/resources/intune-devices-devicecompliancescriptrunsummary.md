---
title: deviceComplianceScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c436261961be8938e8905bc9f19be1690c7f79c4
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789337"
---
# <a name="devicecompliancescriptrunsummary-resource-type"></a><span data-ttu-id="16137-103">deviceComplianceScriptRunSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="16137-103">deviceComplianceScriptRunSummary resource type</span></span>

<span data-ttu-id="16137-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16137-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16137-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="16137-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16137-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="16137-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16137-107">包含设备管理脚本的运行摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="16137-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="16137-108">Methods</span><span class="sxs-lookup"><span data-stu-id="16137-108">Methods</span></span>
|<span data-ttu-id="16137-109">方法</span><span class="sxs-lookup"><span data-stu-id="16137-109">Method</span></span>|<span data-ttu-id="16137-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="16137-110">Return Type</span></span>|<span data-ttu-id="16137-111">说明</span><span class="sxs-lookup"><span data-stu-id="16137-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="16137-112">获取 deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="16137-112">Get deviceComplianceScriptRunSummary</span></span>](../api/intune-devices-devicecompliancescriptrunsummary-get.md)|[<span data-ttu-id="16137-113">deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="16137-113">deviceComplianceScriptRunSummary</span></span>](../resources/intune-devices-devicecompliancescriptrunsummary.md)|<span data-ttu-id="16137-114">读取[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="16137-114">Read properties and relationships of the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="16137-115">更新 deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="16137-115">Update deviceComplianceScriptRunSummary</span></span>](../api/intune-devices-devicecompliancescriptrunsummary-update.md)|[<span data-ttu-id="16137-116">deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="16137-116">deviceComplianceScriptRunSummary</span></span>](../resources/intune-devices-devicecompliancescriptrunsummary.md)|<span data-ttu-id="16137-117">更新[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="16137-117">Update the properties of a [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="16137-118">属性</span><span class="sxs-lookup"><span data-stu-id="16137-118">Properties</span></span>
|<span data-ttu-id="16137-119">属性</span><span class="sxs-lookup"><span data-stu-id="16137-119">Property</span></span>|<span data-ttu-id="16137-120">类型</span><span class="sxs-lookup"><span data-stu-id="16137-120">Type</span></span>|<span data-ttu-id="16137-121">说明</span><span class="sxs-lookup"><span data-stu-id="16137-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16137-122">id</span><span class="sxs-lookup"><span data-stu-id="16137-122">id</span></span>|<span data-ttu-id="16137-123">String</span><span class="sxs-lookup"><span data-stu-id="16137-123">String</span></span>|<span data-ttu-id="16137-124">设备符合性脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="16137-124">Key of the device compliance script run summary entity.</span></span> <span data-ttu-id="16137-125">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="16137-125">This property is read-only.</span></span>|
|<span data-ttu-id="16137-126">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16137-126">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="16137-127">Int32</span><span class="sxs-lookup"><span data-stu-id="16137-127">Int32</span></span>|<span data-ttu-id="16137-128">检测脚本找不到问题且设备正常运行的设备数量。</span><span class="sxs-lookup"><span data-stu-id="16137-128">Number of devices for which the detection script did not find an issue and the device is healthy.</span></span> <span data-ttu-id="16137-129">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="16137-129">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="16137-130">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16137-130">issueDetectedDeviceCount</span></span>|<span data-ttu-id="16137-131">Int32</span><span class="sxs-lookup"><span data-stu-id="16137-131">Int32</span></span>|<span data-ttu-id="16137-132">检测脚本发现问题的设备数。</span><span class="sxs-lookup"><span data-stu-id="16137-132">Number of devices for which the detection script found an issue.</span></span> <span data-ttu-id="16137-133">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="16137-133">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="16137-134">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16137-134">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="16137-135">Int32</span><span class="sxs-lookup"><span data-stu-id="16137-135">Int32</span></span>|<span data-ttu-id="16137-136">检测脚本执行时遇到错误且未完成的设备数量。</span><span class="sxs-lookup"><span data-stu-id="16137-136">Number of devices on which the detection script execution encountered an error and did not complete.</span></span> <span data-ttu-id="16137-137">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="16137-137">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="16137-138">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16137-138">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="16137-139">Int32</span><span class="sxs-lookup"><span data-stu-id="16137-139">Int32</span></span>|<span data-ttu-id="16137-140">尚未运行的设备符合性脚本的最新版本的设备数量。</span><span class="sxs-lookup"><span data-stu-id="16137-140">Number of devices which have not yet run the latest version of the device compliance script.</span></span> <span data-ttu-id="16137-141">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="16137-141">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="16137-142">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="16137-142">lastScriptRunDateTime</span></span>|<span data-ttu-id="16137-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16137-143">DateTimeOffset</span></span>|<span data-ttu-id="16137-144">在所有设备上的脚本的上次运行时间</span><span class="sxs-lookup"><span data-stu-id="16137-144">Last run time for the script across all devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="16137-145">关系</span><span class="sxs-lookup"><span data-stu-id="16137-145">Relationships</span></span>
<span data-ttu-id="16137-146">无</span><span class="sxs-lookup"><span data-stu-id="16137-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16137-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16137-147">JSON Representation</span></span>
<span data-ttu-id="16137-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16137-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)"
}
```



