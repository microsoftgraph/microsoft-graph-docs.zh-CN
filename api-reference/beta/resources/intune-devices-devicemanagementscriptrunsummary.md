---
title: deviceManagementScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ce974f3d5e024a9559f454e8837fd04183e4de9d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784893"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="97608-103">deviceManagementScriptRunSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="97608-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="97608-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="97608-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97608-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97608-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97608-106">包含设备管理脚本的运行摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="97608-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="97608-107">方法</span><span class="sxs-lookup"><span data-stu-id="97608-107">Methods</span></span>
|<span data-ttu-id="97608-108">方法</span><span class="sxs-lookup"><span data-stu-id="97608-108">Method</span></span>|<span data-ttu-id="97608-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="97608-109">Return Type</span></span>|<span data-ttu-id="97608-110">说明</span><span class="sxs-lookup"><span data-stu-id="97608-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="97608-111">获取 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="97608-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="97608-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="97608-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="97608-113">读取[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="97608-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="97608-114">更新 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="97608-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="97608-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="97608-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="97608-116">更新[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="97608-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="97608-117">属性</span><span class="sxs-lookup"><span data-stu-id="97608-117">Properties</span></span>
|<span data-ttu-id="97608-118">属性</span><span class="sxs-lookup"><span data-stu-id="97608-118">Property</span></span>|<span data-ttu-id="97608-119">类型</span><span class="sxs-lookup"><span data-stu-id="97608-119">Type</span></span>|<span data-ttu-id="97608-120">说明</span><span class="sxs-lookup"><span data-stu-id="97608-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97608-121">id</span><span class="sxs-lookup"><span data-stu-id="97608-121">id</span></span>|<span data-ttu-id="97608-122">String</span><span class="sxs-lookup"><span data-stu-id="97608-122">String</span></span>|<span data-ttu-id="97608-123">设备管理脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="97608-123">Key of the device management script run summary entity.</span></span> <span data-ttu-id="97608-124">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="97608-124">This property is read-only.</span></span>|
|<span data-ttu-id="97608-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="97608-125">successDeviceCount</span></span>|<span data-ttu-id="97608-126">Int32</span><span class="sxs-lookup"><span data-stu-id="97608-126">Int32</span></span>|<span data-ttu-id="97608-127">成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="97608-127">Success device count.</span></span>|
|<span data-ttu-id="97608-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="97608-128">errorDeviceCount</span></span>|<span data-ttu-id="97608-129">Int32</span><span class="sxs-lookup"><span data-stu-id="97608-129">Int32</span></span>|<span data-ttu-id="97608-130">错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="97608-130">Error device count.</span></span>|
|<span data-ttu-id="97608-131">successUserCount</span><span class="sxs-lookup"><span data-stu-id="97608-131">successUserCount</span></span>|<span data-ttu-id="97608-132">Int32</span><span class="sxs-lookup"><span data-stu-id="97608-132">Int32</span></span>|<span data-ttu-id="97608-133">成功的用户计数。</span><span class="sxs-lookup"><span data-stu-id="97608-133">Success user count.</span></span>|
|<span data-ttu-id="97608-134">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="97608-134">errorUserCount</span></span>|<span data-ttu-id="97608-135">Int32</span><span class="sxs-lookup"><span data-stu-id="97608-135">Int32</span></span>|<span data-ttu-id="97608-136">错误用户计数。</span><span class="sxs-lookup"><span data-stu-id="97608-136">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97608-137">关系</span><span class="sxs-lookup"><span data-stu-id="97608-137">Relationships</span></span>
<span data-ttu-id="97608-138">无</span><span class="sxs-lookup"><span data-stu-id="97608-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97608-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97608-139">JSON Representation</span></span>
<span data-ttu-id="97608-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97608-140">Here is a JSON representation of the resource.</span></span>
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



