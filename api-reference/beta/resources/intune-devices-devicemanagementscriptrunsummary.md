---
title: deviceManagementScriptRunSummary 资源类型
description: 包含的设备管理脚本运行摘要属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9676fc7f6792c3bd9771ab7ed1ccbeaa67826d3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962035"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="9ed62-103">deviceManagementScriptRunSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ed62-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="9ed62-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9ed62-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ed62-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ed62-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ed62-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9ed62-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ed62-107">包含的设备管理脚本运行摘要属性。</span><span class="sxs-lookup"><span data-stu-id="9ed62-107">Contains properties for the run summary of a device management script.</span></span>
## <a name="methods"></a><span data-ttu-id="9ed62-108">方法</span><span class="sxs-lookup"><span data-stu-id="9ed62-108">Methods</span></span>
|<span data-ttu-id="9ed62-109">方法</span><span class="sxs-lookup"><span data-stu-id="9ed62-109">Method</span></span>|<span data-ttu-id="9ed62-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9ed62-110">Return Type</span></span>|<span data-ttu-id="9ed62-111">说明</span><span class="sxs-lookup"><span data-stu-id="9ed62-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ed62-112">获取 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9ed62-112">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="9ed62-113">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9ed62-113">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="9ed62-114">读取属性和[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="9ed62-114">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="9ed62-115">更新 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9ed62-115">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="9ed62-116">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9ed62-116">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="9ed62-117">更新[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9ed62-117">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ed62-118">属性</span><span class="sxs-lookup"><span data-stu-id="9ed62-118">Properties</span></span>
|<span data-ttu-id="9ed62-119">属性</span><span class="sxs-lookup"><span data-stu-id="9ed62-119">Property</span></span>|<span data-ttu-id="9ed62-120">类型</span><span class="sxs-lookup"><span data-stu-id="9ed62-120">Type</span></span>|<span data-ttu-id="9ed62-121">说明</span><span class="sxs-lookup"><span data-stu-id="9ed62-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ed62-122">id</span><span class="sxs-lookup"><span data-stu-id="9ed62-122">id</span></span>|<span data-ttu-id="9ed62-123">字符串</span><span class="sxs-lookup"><span data-stu-id="9ed62-123">String</span></span>|<span data-ttu-id="9ed62-124">运行摘要实体的设备管理脚本的键。</span><span class="sxs-lookup"><span data-stu-id="9ed62-124">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="9ed62-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9ed62-125">successDeviceCount</span></span>|<span data-ttu-id="9ed62-126">Int32</span><span class="sxs-lookup"><span data-stu-id="9ed62-126">Int32</span></span>|<span data-ttu-id="9ed62-127">成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="9ed62-127">Success device count.</span></span>|
|<span data-ttu-id="9ed62-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9ed62-128">errorDeviceCount</span></span>|<span data-ttu-id="9ed62-129">Int32</span><span class="sxs-lookup"><span data-stu-id="9ed62-129">Int32</span></span>|<span data-ttu-id="9ed62-130">错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="9ed62-130">Error device count.</span></span>|
|<span data-ttu-id="9ed62-131">successUserCount</span><span class="sxs-lookup"><span data-stu-id="9ed62-131">successUserCount</span></span>|<span data-ttu-id="9ed62-132">Int32</span><span class="sxs-lookup"><span data-stu-id="9ed62-132">Int32</span></span>|<span data-ttu-id="9ed62-133">成功用户计数。</span><span class="sxs-lookup"><span data-stu-id="9ed62-133">Success user count.</span></span>|
|<span data-ttu-id="9ed62-134">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="9ed62-134">errorUserCount</span></span>|<span data-ttu-id="9ed62-135">Int32</span><span class="sxs-lookup"><span data-stu-id="9ed62-135">Int32</span></span>|<span data-ttu-id="9ed62-136">错误用户计数。</span><span class="sxs-lookup"><span data-stu-id="9ed62-136">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ed62-137">Relationships</span><span class="sxs-lookup"><span data-stu-id="9ed62-137">Relationships</span></span>
<span data-ttu-id="9ed62-138">无</span><span class="sxs-lookup"><span data-stu-id="9ed62-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9ed62-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ed62-139">JSON Representation</span></span>
<span data-ttu-id="9ed62-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ed62-140">Here is a JSON representation of the resource.</span></span>
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





