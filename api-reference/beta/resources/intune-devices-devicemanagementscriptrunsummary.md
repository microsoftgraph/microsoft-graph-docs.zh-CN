---
title: deviceManagementScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 199b9efcdc3ea862502ea22d845480d990c99caf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995306"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="3f65b-103">deviceManagementScriptRunSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f65b-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="3f65b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f65b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f65b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f65b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f65b-106">包含设备管理脚本的运行摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="3f65b-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="3f65b-107">方法</span><span class="sxs-lookup"><span data-stu-id="3f65b-107">Methods</span></span>
|<span data-ttu-id="3f65b-108">方法</span><span class="sxs-lookup"><span data-stu-id="3f65b-108">Method</span></span>|<span data-ttu-id="3f65b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f65b-109">Return Type</span></span>|<span data-ttu-id="3f65b-110">说明</span><span class="sxs-lookup"><span data-stu-id="3f65b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3f65b-111">获取 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="3f65b-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="3f65b-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="3f65b-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="3f65b-113">读取[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f65b-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="3f65b-114">更新 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="3f65b-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="3f65b-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="3f65b-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="3f65b-116">更新[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3f65b-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f65b-117">属性</span><span class="sxs-lookup"><span data-stu-id="3f65b-117">Properties</span></span>
|<span data-ttu-id="3f65b-118">属性</span><span class="sxs-lookup"><span data-stu-id="3f65b-118">Property</span></span>|<span data-ttu-id="3f65b-119">类型</span><span class="sxs-lookup"><span data-stu-id="3f65b-119">Type</span></span>|<span data-ttu-id="3f65b-120">说明</span><span class="sxs-lookup"><span data-stu-id="3f65b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f65b-121">id</span><span class="sxs-lookup"><span data-stu-id="3f65b-121">id</span></span>|<span data-ttu-id="3f65b-122">String</span><span class="sxs-lookup"><span data-stu-id="3f65b-122">String</span></span>|<span data-ttu-id="3f65b-123">设备管理脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="3f65b-123">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="3f65b-124">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3f65b-124">successDeviceCount</span></span>|<span data-ttu-id="3f65b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="3f65b-125">Int32</span></span>|<span data-ttu-id="3f65b-126">成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="3f65b-126">Success device count.</span></span>|
|<span data-ttu-id="3f65b-127">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3f65b-127">errorDeviceCount</span></span>|<span data-ttu-id="3f65b-128">Int32</span><span class="sxs-lookup"><span data-stu-id="3f65b-128">Int32</span></span>|<span data-ttu-id="3f65b-129">错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="3f65b-129">Error device count.</span></span>|
|<span data-ttu-id="3f65b-130">successUserCount</span><span class="sxs-lookup"><span data-stu-id="3f65b-130">successUserCount</span></span>|<span data-ttu-id="3f65b-131">Int32</span><span class="sxs-lookup"><span data-stu-id="3f65b-131">Int32</span></span>|<span data-ttu-id="3f65b-132">成功的用户计数。</span><span class="sxs-lookup"><span data-stu-id="3f65b-132">Success user count.</span></span>|
|<span data-ttu-id="3f65b-133">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="3f65b-133">errorUserCount</span></span>|<span data-ttu-id="3f65b-134">Int32</span><span class="sxs-lookup"><span data-stu-id="3f65b-134">Int32</span></span>|<span data-ttu-id="3f65b-135">错误用户计数。</span><span class="sxs-lookup"><span data-stu-id="3f65b-135">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f65b-136">关系</span><span class="sxs-lookup"><span data-stu-id="3f65b-136">Relationships</span></span>
<span data-ttu-id="3f65b-137">无</span><span class="sxs-lookup"><span data-stu-id="3f65b-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f65b-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f65b-138">JSON Representation</span></span>
<span data-ttu-id="3f65b-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f65b-139">Here is a JSON representation of the resource.</span></span>
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





