---
title: deviceManagementScriptGroupAssignment 资源类型
description: 包含用于分配给组的设备管理脚本的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ab4cdc6565841623c16bb46b0e0e36c01c68a9de
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410572"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a><span data-ttu-id="f7b71-103">deviceManagementScriptGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7b71-103">deviceManagementScriptGroupAssignment resource type</span></span>

> <span data-ttu-id="f7b71-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f7b71-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f7b71-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f7b71-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7b71-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7b71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7b71-107">包含用于分配给组的设备管理脚本的属性。</span><span class="sxs-lookup"><span data-stu-id="f7b71-107">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="f7b71-108">方法</span><span class="sxs-lookup"><span data-stu-id="f7b71-108">Methods</span></span>
|<span data-ttu-id="f7b71-109">方法</span><span class="sxs-lookup"><span data-stu-id="f7b71-109">Method</span></span>|<span data-ttu-id="f7b71-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f7b71-110">Return Type</span></span>|<span data-ttu-id="f7b71-111">说明</span><span class="sxs-lookup"><span data-stu-id="f7b71-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f7b71-112">列表 deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="f7b71-112">List deviceManagementScriptGroupAssignments</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|<span data-ttu-id="f7b71-113">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="f7b71-113">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="f7b71-114">列出属性和[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="f7b71-114">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="f7b71-115">获取 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f7b71-115">Get deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[<span data-ttu-id="f7b71-116">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f7b71-116">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="f7b71-117">读取属性和[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="f7b71-117">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="f7b71-118">创建 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f7b71-118">Create deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[<span data-ttu-id="f7b71-119">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f7b71-119">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="f7b71-120">创建新的[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f7b71-120">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="f7b71-121">删除 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f7b71-121">Delete deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|<span data-ttu-id="f7b71-122">无</span><span class="sxs-lookup"><span data-stu-id="f7b71-122">None</span></span>|<span data-ttu-id="f7b71-123">删除[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="f7b71-123">Deletes a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>|
|[<span data-ttu-id="f7b71-124">更新 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f7b71-124">Update deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[<span data-ttu-id="f7b71-125">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f7b71-125">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="f7b71-126">更新[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f7b71-126">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7b71-127">属性</span><span class="sxs-lookup"><span data-stu-id="f7b71-127">Properties</span></span>
|<span data-ttu-id="f7b71-128">属性</span><span class="sxs-lookup"><span data-stu-id="f7b71-128">Property</span></span>|<span data-ttu-id="f7b71-129">类型</span><span class="sxs-lookup"><span data-stu-id="f7b71-129">Type</span></span>|<span data-ttu-id="f7b71-130">说明</span><span class="sxs-lookup"><span data-stu-id="f7b71-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7b71-131">id</span><span class="sxs-lookup"><span data-stu-id="f7b71-131">id</span></span>|<span data-ttu-id="f7b71-132">String</span><span class="sxs-lookup"><span data-stu-id="f7b71-132">String</span></span>|<span data-ttu-id="f7b71-133">设备管理脚本组工作分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="f7b71-133">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="f7b71-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="f7b71-134">targetGroupId</span></span>|<span data-ttu-id="f7b71-135">String</span><span class="sxs-lookup"><span data-stu-id="f7b71-135">String</span></span>|<span data-ttu-id="f7b71-136">Azure Active Directory 组的 Id 目标脚本。</span><span class="sxs-lookup"><span data-stu-id="f7b71-136">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7b71-137">关系</span><span class="sxs-lookup"><span data-stu-id="f7b71-137">Relationships</span></span>
<span data-ttu-id="f7b71-138">无</span><span class="sxs-lookup"><span data-stu-id="f7b71-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7b71-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7b71-139">JSON Representation</span></span>
<span data-ttu-id="f7b71-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7b71-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```




