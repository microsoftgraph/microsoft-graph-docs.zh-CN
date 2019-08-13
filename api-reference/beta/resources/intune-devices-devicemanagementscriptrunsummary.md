---
title: deviceManagementScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e9d2b0b92287a045607c02e271155e2e74a2fa90
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370023"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="0ae45-103">deviceManagementScriptRunSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ae45-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="0ae45-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0ae45-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ae45-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ae45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ae45-106">包含设备管理脚本的运行摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="0ae45-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="0ae45-107">方法</span><span class="sxs-lookup"><span data-stu-id="0ae45-107">Methods</span></span>
|<span data-ttu-id="0ae45-108">方法</span><span class="sxs-lookup"><span data-stu-id="0ae45-108">Method</span></span>|<span data-ttu-id="0ae45-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0ae45-109">Return Type</span></span>|<span data-ttu-id="0ae45-110">说明</span><span class="sxs-lookup"><span data-stu-id="0ae45-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0ae45-111">获取 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="0ae45-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="0ae45-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="0ae45-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="0ae45-113">读取[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0ae45-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="0ae45-114">更新 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="0ae45-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="0ae45-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="0ae45-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="0ae45-116">更新[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0ae45-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0ae45-117">属性</span><span class="sxs-lookup"><span data-stu-id="0ae45-117">Properties</span></span>
|<span data-ttu-id="0ae45-118">属性</span><span class="sxs-lookup"><span data-stu-id="0ae45-118">Property</span></span>|<span data-ttu-id="0ae45-119">类型</span><span class="sxs-lookup"><span data-stu-id="0ae45-119">Type</span></span>|<span data-ttu-id="0ae45-120">说明</span><span class="sxs-lookup"><span data-stu-id="0ae45-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ae45-121">id</span><span class="sxs-lookup"><span data-stu-id="0ae45-121">id</span></span>|<span data-ttu-id="0ae45-122">String</span><span class="sxs-lookup"><span data-stu-id="0ae45-122">String</span></span>|<span data-ttu-id="0ae45-123">设备管理脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="0ae45-123">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="0ae45-124">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0ae45-124">successDeviceCount</span></span>|<span data-ttu-id="0ae45-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0ae45-125">Int32</span></span>|<span data-ttu-id="0ae45-126">成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="0ae45-126">Success device count.</span></span>|
|<span data-ttu-id="0ae45-127">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0ae45-127">errorDeviceCount</span></span>|<span data-ttu-id="0ae45-128">Int32</span><span class="sxs-lookup"><span data-stu-id="0ae45-128">Int32</span></span>|<span data-ttu-id="0ae45-129">错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="0ae45-129">Error device count.</span></span>|
|<span data-ttu-id="0ae45-130">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0ae45-130">compliantDeviceCount</span></span>|<span data-ttu-id="0ae45-131">Int32</span><span class="sxs-lookup"><span data-stu-id="0ae45-131">Int32</span></span>|<span data-ttu-id="0ae45-132">合规设备计数。</span><span class="sxs-lookup"><span data-stu-id="0ae45-132">Compliant device count.</span></span>|
|<span data-ttu-id="0ae45-133">notCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0ae45-133">notCompliantDeviceCount</span></span>|<span data-ttu-id="0ae45-134">Int32</span><span class="sxs-lookup"><span data-stu-id="0ae45-134">Int32</span></span>|<span data-ttu-id="0ae45-135">不符合的设备计数。</span><span class="sxs-lookup"><span data-stu-id="0ae45-135">Not Compliant device count.</span></span>|
|<span data-ttu-id="0ae45-136">pendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0ae45-136">pendingDeviceCount</span></span>|<span data-ttu-id="0ae45-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0ae45-137">Int32</span></span>|<span data-ttu-id="0ae45-138">挂起的设备计数。</span><span class="sxs-lookup"><span data-stu-id="0ae45-138">Pending device count.</span></span>|
|<span data-ttu-id="0ae45-139">successUserCount</span><span class="sxs-lookup"><span data-stu-id="0ae45-139">successUserCount</span></span>|<span data-ttu-id="0ae45-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0ae45-140">Int32</span></span>|<span data-ttu-id="0ae45-141">成功的用户计数。</span><span class="sxs-lookup"><span data-stu-id="0ae45-141">Success user count.</span></span>|
|<span data-ttu-id="0ae45-142">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="0ae45-142">errorUserCount</span></span>|<span data-ttu-id="0ae45-143">Int32</span><span class="sxs-lookup"><span data-stu-id="0ae45-143">Int32</span></span>|<span data-ttu-id="0ae45-144">错误用户计数。</span><span class="sxs-lookup"><span data-stu-id="0ae45-144">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ae45-145">关系</span><span class="sxs-lookup"><span data-stu-id="0ae45-145">Relationships</span></span>
<span data-ttu-id="0ae45-146">无</span><span class="sxs-lookup"><span data-stu-id="0ae45-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ae45-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ae45-147">JSON Representation</span></span>
<span data-ttu-id="0ae45-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ae45-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "notCompliantDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```



