---
title: deviceManagementScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e39890bfd728e94dbb48e6420931dbdd00cf9c01
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43374514"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="8fc6f-103">deviceManagementScriptRunSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="8fc6f-103">deviceManagementScriptRunSummary resource type</span></span>

<span data-ttu-id="8fc6f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fc6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8fc6f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8fc6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fc6f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8fc6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fc6f-107">包含设备管理脚本的运行摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="8fc6f-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="8fc6f-108">方法</span><span class="sxs-lookup"><span data-stu-id="8fc6f-108">Methods</span></span>
|<span data-ttu-id="8fc6f-109">方法</span><span class="sxs-lookup"><span data-stu-id="8fc6f-109">Method</span></span>|<span data-ttu-id="8fc6f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8fc6f-110">Return Type</span></span>|<span data-ttu-id="8fc6f-111">说明</span><span class="sxs-lookup"><span data-stu-id="8fc6f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8fc6f-112">获取 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="8fc6f-112">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="8fc6f-113">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="8fc6f-113">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="8fc6f-114">读取[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8fc6f-114">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="8fc6f-115">更新 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="8fc6f-115">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="8fc6f-116">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="8fc6f-116">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="8fc6f-117">更新[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8fc6f-117">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8fc6f-118">属性</span><span class="sxs-lookup"><span data-stu-id="8fc6f-118">Properties</span></span>
|<span data-ttu-id="8fc6f-119">属性</span><span class="sxs-lookup"><span data-stu-id="8fc6f-119">Property</span></span>|<span data-ttu-id="8fc6f-120">类型</span><span class="sxs-lookup"><span data-stu-id="8fc6f-120">Type</span></span>|<span data-ttu-id="8fc6f-121">说明</span><span class="sxs-lookup"><span data-stu-id="8fc6f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fc6f-122">id</span><span class="sxs-lookup"><span data-stu-id="8fc6f-122">id</span></span>|<span data-ttu-id="8fc6f-123">字符串</span><span class="sxs-lookup"><span data-stu-id="8fc6f-123">String</span></span>|<span data-ttu-id="8fc6f-124">设备管理脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="8fc6f-124">Key of the device management script run summary entity.</span></span> <span data-ttu-id="8fc6f-125">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8fc6f-125">This property is read-only.</span></span>|
|<span data-ttu-id="8fc6f-126">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fc6f-126">successDeviceCount</span></span>|<span data-ttu-id="8fc6f-127">Int32</span><span class="sxs-lookup"><span data-stu-id="8fc6f-127">Int32</span></span>|<span data-ttu-id="8fc6f-128">成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="8fc6f-128">Success device count.</span></span>|
|<span data-ttu-id="8fc6f-129">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fc6f-129">errorDeviceCount</span></span>|<span data-ttu-id="8fc6f-130">Int32</span><span class="sxs-lookup"><span data-stu-id="8fc6f-130">Int32</span></span>|<span data-ttu-id="8fc6f-131">错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="8fc6f-131">Error device count.</span></span>|
|<span data-ttu-id="8fc6f-132">successUserCount</span><span class="sxs-lookup"><span data-stu-id="8fc6f-132">successUserCount</span></span>|<span data-ttu-id="8fc6f-133">Int32</span><span class="sxs-lookup"><span data-stu-id="8fc6f-133">Int32</span></span>|<span data-ttu-id="8fc6f-134">成功的用户计数。</span><span class="sxs-lookup"><span data-stu-id="8fc6f-134">Success user count.</span></span>|
|<span data-ttu-id="8fc6f-135">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="8fc6f-135">errorUserCount</span></span>|<span data-ttu-id="8fc6f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="8fc6f-136">Int32</span></span>|<span data-ttu-id="8fc6f-137">错误用户计数。</span><span class="sxs-lookup"><span data-stu-id="8fc6f-137">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fc6f-138">关系</span><span class="sxs-lookup"><span data-stu-id="8fc6f-138">Relationships</span></span>
<span data-ttu-id="8fc6f-139">无</span><span class="sxs-lookup"><span data-stu-id="8fc6f-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8fc6f-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8fc6f-140">JSON Representation</span></span>
<span data-ttu-id="8fc6f-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fc6f-141">Here is a JSON representation of the resource.</span></span>
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



