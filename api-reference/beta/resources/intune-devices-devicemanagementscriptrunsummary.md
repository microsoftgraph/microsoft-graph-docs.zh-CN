---
title: deviceManagementScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6807114ebaf7ba3a778520c7b2a383f5a13c31f1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794195"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="11191-103">deviceManagementScriptRunSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="11191-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="11191-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11191-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11191-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11191-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11191-106">包含设备管理脚本的运行摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="11191-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="11191-107">方法</span><span class="sxs-lookup"><span data-stu-id="11191-107">Methods</span></span>
|<span data-ttu-id="11191-108">方法</span><span class="sxs-lookup"><span data-stu-id="11191-108">Method</span></span>|<span data-ttu-id="11191-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="11191-109">Return Type</span></span>|<span data-ttu-id="11191-110">说明</span><span class="sxs-lookup"><span data-stu-id="11191-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="11191-111">获取 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="11191-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="11191-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="11191-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="11191-113">读取[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="11191-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="11191-114">更新 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="11191-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="11191-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="11191-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="11191-116">更新[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="11191-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="11191-117">属性</span><span class="sxs-lookup"><span data-stu-id="11191-117">Properties</span></span>
|<span data-ttu-id="11191-118">属性</span><span class="sxs-lookup"><span data-stu-id="11191-118">Property</span></span>|<span data-ttu-id="11191-119">类型</span><span class="sxs-lookup"><span data-stu-id="11191-119">Type</span></span>|<span data-ttu-id="11191-120">说明</span><span class="sxs-lookup"><span data-stu-id="11191-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11191-121">id</span><span class="sxs-lookup"><span data-stu-id="11191-121">id</span></span>|<span data-ttu-id="11191-122">String</span><span class="sxs-lookup"><span data-stu-id="11191-122">String</span></span>|<span data-ttu-id="11191-123">设备管理脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="11191-123">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="11191-124">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="11191-124">successDeviceCount</span></span>|<span data-ttu-id="11191-125">Int32</span><span class="sxs-lookup"><span data-stu-id="11191-125">Int32</span></span>|<span data-ttu-id="11191-126">成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="11191-126">Success device count.</span></span>|
|<span data-ttu-id="11191-127">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="11191-127">errorDeviceCount</span></span>|<span data-ttu-id="11191-128">Int32</span><span class="sxs-lookup"><span data-stu-id="11191-128">Int32</span></span>|<span data-ttu-id="11191-129">错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="11191-129">Error device count.</span></span>|
|<span data-ttu-id="11191-130">successUserCount</span><span class="sxs-lookup"><span data-stu-id="11191-130">successUserCount</span></span>|<span data-ttu-id="11191-131">Int32</span><span class="sxs-lookup"><span data-stu-id="11191-131">Int32</span></span>|<span data-ttu-id="11191-132">成功的用户计数。</span><span class="sxs-lookup"><span data-stu-id="11191-132">Success user count.</span></span>|
|<span data-ttu-id="11191-133">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="11191-133">errorUserCount</span></span>|<span data-ttu-id="11191-134">Int32</span><span class="sxs-lookup"><span data-stu-id="11191-134">Int32</span></span>|<span data-ttu-id="11191-135">错误用户计数。</span><span class="sxs-lookup"><span data-stu-id="11191-135">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11191-136">关系</span><span class="sxs-lookup"><span data-stu-id="11191-136">Relationships</span></span>
<span data-ttu-id="11191-137">无</span><span class="sxs-lookup"><span data-stu-id="11191-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11191-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11191-138">JSON Representation</span></span>
<span data-ttu-id="11191-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11191-139">Here is a JSON representation of the resource.</span></span>
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





