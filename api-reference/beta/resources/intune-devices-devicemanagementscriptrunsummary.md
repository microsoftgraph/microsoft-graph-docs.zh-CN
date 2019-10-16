---
title: deviceManagementScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1780dbfd6d53cf25fdd18b3c78f0c84c39b5455d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538789"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="e4bab-103">deviceManagementScriptRunSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4bab-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="e4bab-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e4bab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4bab-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4bab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4bab-106">包含设备管理脚本的运行摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="e4bab-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="e4bab-107">方法</span><span class="sxs-lookup"><span data-stu-id="e4bab-107">Methods</span></span>
|<span data-ttu-id="e4bab-108">方法</span><span class="sxs-lookup"><span data-stu-id="e4bab-108">Method</span></span>|<span data-ttu-id="e4bab-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e4bab-109">Return Type</span></span>|<span data-ttu-id="e4bab-110">说明</span><span class="sxs-lookup"><span data-stu-id="e4bab-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e4bab-111">获取 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e4bab-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="e4bab-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e4bab-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="e4bab-113">读取[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e4bab-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="e4bab-114">更新 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e4bab-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="e4bab-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e4bab-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="e4bab-116">更新[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e4bab-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e4bab-117">属性</span><span class="sxs-lookup"><span data-stu-id="e4bab-117">Properties</span></span>
|<span data-ttu-id="e4bab-118">属性</span><span class="sxs-lookup"><span data-stu-id="e4bab-118">Property</span></span>|<span data-ttu-id="e4bab-119">类型</span><span class="sxs-lookup"><span data-stu-id="e4bab-119">Type</span></span>|<span data-ttu-id="e4bab-120">说明</span><span class="sxs-lookup"><span data-stu-id="e4bab-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4bab-121">id</span><span class="sxs-lookup"><span data-stu-id="e4bab-121">id</span></span>|<span data-ttu-id="e4bab-122">字符串</span><span class="sxs-lookup"><span data-stu-id="e4bab-122">String</span></span>|<span data-ttu-id="e4bab-123">设备管理脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="e4bab-123">Key of the device management script run summary entity.</span></span> <span data-ttu-id="e4bab-124">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e4bab-124">This property is read-only.</span></span>|
|<span data-ttu-id="e4bab-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e4bab-125">successDeviceCount</span></span>|<span data-ttu-id="e4bab-126">Int32</span><span class="sxs-lookup"><span data-stu-id="e4bab-126">Int32</span></span>|<span data-ttu-id="e4bab-127">成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="e4bab-127">Success device count.</span></span>|
|<span data-ttu-id="e4bab-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e4bab-128">errorDeviceCount</span></span>|<span data-ttu-id="e4bab-129">Int32</span><span class="sxs-lookup"><span data-stu-id="e4bab-129">Int32</span></span>|<span data-ttu-id="e4bab-130">错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="e4bab-130">Error device count.</span></span>|
|<span data-ttu-id="e4bab-131">successUserCount</span><span class="sxs-lookup"><span data-stu-id="e4bab-131">successUserCount</span></span>|<span data-ttu-id="e4bab-132">Int32</span><span class="sxs-lookup"><span data-stu-id="e4bab-132">Int32</span></span>|<span data-ttu-id="e4bab-133">成功的用户计数。</span><span class="sxs-lookup"><span data-stu-id="e4bab-133">Success user count.</span></span>|
|<span data-ttu-id="e4bab-134">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="e4bab-134">errorUserCount</span></span>|<span data-ttu-id="e4bab-135">Int32</span><span class="sxs-lookup"><span data-stu-id="e4bab-135">Int32</span></span>|<span data-ttu-id="e4bab-136">错误用户计数。</span><span class="sxs-lookup"><span data-stu-id="e4bab-136">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4bab-137">关系</span><span class="sxs-lookup"><span data-stu-id="e4bab-137">Relationships</span></span>
<span data-ttu-id="e4bab-138">无</span><span class="sxs-lookup"><span data-stu-id="e4bab-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4bab-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4bab-139">JSON Representation</span></span>
<span data-ttu-id="e4bab-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4bab-140">Here is a JSON representation of the resource.</span></span>
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
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```



