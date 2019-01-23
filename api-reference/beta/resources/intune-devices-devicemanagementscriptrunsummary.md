---
title: deviceManagementScriptRunSummary 资源类型
description: 包含的设备管理脚本运行摘要属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f49e08c0f6351133b953e566ba8e89afe945e990
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423851"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="58963-103">deviceManagementScriptRunSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="58963-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="58963-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="58963-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="58963-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="58963-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58963-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58963-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58963-107">包含的设备管理脚本运行摘要属性。</span><span class="sxs-lookup"><span data-stu-id="58963-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="58963-108">方法</span><span class="sxs-lookup"><span data-stu-id="58963-108">Methods</span></span>
|<span data-ttu-id="58963-109">方法</span><span class="sxs-lookup"><span data-stu-id="58963-109">Method</span></span>|<span data-ttu-id="58963-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="58963-110">Return Type</span></span>|<span data-ttu-id="58963-111">说明</span><span class="sxs-lookup"><span data-stu-id="58963-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="58963-112">获取 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="58963-112">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="58963-113">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="58963-113">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="58963-114">读取属性和[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="58963-114">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="58963-115">更新 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="58963-115">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="58963-116">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="58963-116">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="58963-117">更新[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="58963-117">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="58963-118">属性</span><span class="sxs-lookup"><span data-stu-id="58963-118">Properties</span></span>
|<span data-ttu-id="58963-119">属性</span><span class="sxs-lookup"><span data-stu-id="58963-119">Property</span></span>|<span data-ttu-id="58963-120">类型</span><span class="sxs-lookup"><span data-stu-id="58963-120">Type</span></span>|<span data-ttu-id="58963-121">说明</span><span class="sxs-lookup"><span data-stu-id="58963-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58963-122">id</span><span class="sxs-lookup"><span data-stu-id="58963-122">id</span></span>|<span data-ttu-id="58963-123">String</span><span class="sxs-lookup"><span data-stu-id="58963-123">String</span></span>|<span data-ttu-id="58963-124">运行摘要实体的设备管理脚本的键。</span><span class="sxs-lookup"><span data-stu-id="58963-124">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="58963-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="58963-125">successDeviceCount</span></span>|<span data-ttu-id="58963-126">Int32</span><span class="sxs-lookup"><span data-stu-id="58963-126">Int32</span></span>|<span data-ttu-id="58963-127">成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="58963-127">Success device count.</span></span>|
|<span data-ttu-id="58963-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="58963-128">errorDeviceCount</span></span>|<span data-ttu-id="58963-129">Int32</span><span class="sxs-lookup"><span data-stu-id="58963-129">Int32</span></span>|<span data-ttu-id="58963-130">错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="58963-130">Error device count.</span></span>|
|<span data-ttu-id="58963-131">successUserCount</span><span class="sxs-lookup"><span data-stu-id="58963-131">successUserCount</span></span>|<span data-ttu-id="58963-132">Int32</span><span class="sxs-lookup"><span data-stu-id="58963-132">Int32</span></span>|<span data-ttu-id="58963-133">成功用户计数。</span><span class="sxs-lookup"><span data-stu-id="58963-133">Success user count.</span></span>|
|<span data-ttu-id="58963-134">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="58963-134">errorUserCount</span></span>|<span data-ttu-id="58963-135">Int32</span><span class="sxs-lookup"><span data-stu-id="58963-135">Int32</span></span>|<span data-ttu-id="58963-136">错误用户计数。</span><span class="sxs-lookup"><span data-stu-id="58963-136">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58963-137">关系</span><span class="sxs-lookup"><span data-stu-id="58963-137">Relationships</span></span>
<span data-ttu-id="58963-138">无</span><span class="sxs-lookup"><span data-stu-id="58963-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58963-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58963-139">JSON Representation</span></span>
<span data-ttu-id="58963-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58963-140">Here is a JSON representation of the resource.</span></span>
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




