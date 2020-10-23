---
title: deviceComplianceScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9f1968b9573cf65429e9a01dbd25920e114ff4df
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734152"
---
# <a name="devicecompliancescriptrunsummary-resource-type"></a><span data-ttu-id="aa3d6-103">deviceComplianceScriptRunSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa3d6-103">deviceComplianceScriptRunSummary resource type</span></span>

<span data-ttu-id="aa3d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa3d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa3d6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aa3d6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa3d6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aa3d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa3d6-107">包含设备管理脚本的运行摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="aa3d6-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="aa3d6-108">Methods</span><span class="sxs-lookup"><span data-stu-id="aa3d6-108">Methods</span></span>
|<span data-ttu-id="aa3d6-109">方法</span><span class="sxs-lookup"><span data-stu-id="aa3d6-109">Method</span></span>|<span data-ttu-id="aa3d6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="aa3d6-110">Return Type</span></span>|<span data-ttu-id="aa3d6-111">说明</span><span class="sxs-lookup"><span data-stu-id="aa3d6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aa3d6-112">获取 deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="aa3d6-112">Get deviceComplianceScriptRunSummary</span></span>](../api/intune-devices-devicecompliancescriptrunsummary-get.md)|[<span data-ttu-id="aa3d6-113">deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="aa3d6-113">deviceComplianceScriptRunSummary</span></span>](../resources/intune-devices-devicecompliancescriptrunsummary.md)|<span data-ttu-id="aa3d6-114">读取 [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aa3d6-114">Read properties and relationships of the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="aa3d6-115">更新 deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="aa3d6-115">Update deviceComplianceScriptRunSummary</span></span>](../api/intune-devices-devicecompliancescriptrunsummary-update.md)|[<span data-ttu-id="aa3d6-116">deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="aa3d6-116">deviceComplianceScriptRunSummary</span></span>](../resources/intune-devices-devicecompliancescriptrunsummary.md)|<span data-ttu-id="aa3d6-117">更新 [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aa3d6-117">Update the properties of a [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa3d6-118">属性</span><span class="sxs-lookup"><span data-stu-id="aa3d6-118">Properties</span></span>
|<span data-ttu-id="aa3d6-119">属性</span><span class="sxs-lookup"><span data-stu-id="aa3d6-119">Property</span></span>|<span data-ttu-id="aa3d6-120">类型</span><span class="sxs-lookup"><span data-stu-id="aa3d6-120">Type</span></span>|<span data-ttu-id="aa3d6-121">说明</span><span class="sxs-lookup"><span data-stu-id="aa3d6-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa3d6-122">id</span><span class="sxs-lookup"><span data-stu-id="aa3d6-122">id</span></span>|<span data-ttu-id="aa3d6-123">String</span><span class="sxs-lookup"><span data-stu-id="aa3d6-123">String</span></span>|<span data-ttu-id="aa3d6-124">设备符合性脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="aa3d6-124">Key of the device compliance script run summary entity.</span></span> <span data-ttu-id="aa3d6-125">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="aa3d6-125">This property is read-only.</span></span>|
|<span data-ttu-id="aa3d6-126">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aa3d6-126">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="aa3d6-127">Int32</span><span class="sxs-lookup"><span data-stu-id="aa3d6-127">Int32</span></span>|<span data-ttu-id="aa3d6-128">检测脚本找不到问题且设备正常运行的设备数量。</span><span class="sxs-lookup"><span data-stu-id="aa3d6-128">Number of devices for which the detection script did not find an issue and the device is healthy.</span></span> <span data-ttu-id="aa3d6-129">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="aa3d6-129">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="aa3d6-130">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aa3d6-130">issueDetectedDeviceCount</span></span>|<span data-ttu-id="aa3d6-131">Int32</span><span class="sxs-lookup"><span data-stu-id="aa3d6-131">Int32</span></span>|<span data-ttu-id="aa3d6-132">检测脚本发现问题的设备数。</span><span class="sxs-lookup"><span data-stu-id="aa3d6-132">Number of devices for which the detection script found an issue.</span></span> <span data-ttu-id="aa3d6-133">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="aa3d6-133">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="aa3d6-134">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aa3d6-134">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="aa3d6-135">Int32</span><span class="sxs-lookup"><span data-stu-id="aa3d6-135">Int32</span></span>|<span data-ttu-id="aa3d6-136">检测脚本执行时遇到错误且未完成的设备数量。</span><span class="sxs-lookup"><span data-stu-id="aa3d6-136">Number of devices on which the detection script execution encountered an error and did not complete.</span></span> <span data-ttu-id="aa3d6-137">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="aa3d6-137">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="aa3d6-138">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aa3d6-138">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="aa3d6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="aa3d6-139">Int32</span></span>|<span data-ttu-id="aa3d6-140">尚未运行的设备符合性脚本的最新版本的设备数量。</span><span class="sxs-lookup"><span data-stu-id="aa3d6-140">Number of devices which have not yet run the latest version of the device compliance script.</span></span> <span data-ttu-id="aa3d6-141">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="aa3d6-141">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="aa3d6-142">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="aa3d6-142">lastScriptRunDateTime</span></span>|<span data-ttu-id="aa3d6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa3d6-143">DateTimeOffset</span></span>|<span data-ttu-id="aa3d6-144">在所有设备上的脚本的上次运行时间</span><span class="sxs-lookup"><span data-stu-id="aa3d6-144">Last run time for the script across all devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa3d6-145">关系</span><span class="sxs-lookup"><span data-stu-id="aa3d6-145">Relationships</span></span>
<span data-ttu-id="aa3d6-146">无</span><span class="sxs-lookup"><span data-stu-id="aa3d6-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa3d6-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa3d6-147">JSON Representation</span></span>
<span data-ttu-id="aa3d6-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa3d6-148">Here is a JSON representation of the resource.</span></span>
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





