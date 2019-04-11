---
title: deviceManagementScriptAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: def29ebd398b56514ad6c1e5897715b603429d4c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779144"
---
# <a name="devicemanagementscriptassignment-resource-type"></a><span data-ttu-id="f0a10-103">deviceManagementScriptAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0a10-103">deviceManagementScriptAssignment resource type</span></span>

> <span data-ttu-id="f0a10-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0a10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0a10-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0a10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0a10-106">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="f0a10-106">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="f0a10-107">方法</span><span class="sxs-lookup"><span data-stu-id="f0a10-107">Methods</span></span>
|<span data-ttu-id="f0a10-108">方法</span><span class="sxs-lookup"><span data-stu-id="f0a10-108">Method</span></span>|<span data-ttu-id="f0a10-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f0a10-109">Return Type</span></span>|<span data-ttu-id="f0a10-110">说明</span><span class="sxs-lookup"><span data-stu-id="f0a10-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f0a10-111">列出 deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="f0a10-111">List deviceManagementScriptAssignments</span></span>](../api/intune-devices-devicemanagementscriptassignment-list.md)|<span data-ttu-id="f0a10-112">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="f0a10-112">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="f0a10-113">列出[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f0a10-113">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="f0a10-114">获取 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="f0a10-114">Get deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-get.md)|[<span data-ttu-id="f0a10-115">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="f0a10-115">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="f0a10-116">读取[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f0a10-116">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="f0a10-117">创建 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="f0a10-117">Create deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-create.md)|[<span data-ttu-id="f0a10-118">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="f0a10-118">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="f0a10-119">创建新的[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f0a10-119">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="f0a10-120">删除 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="f0a10-120">Delete deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-delete.md)|<span data-ttu-id="f0a10-121">无</span><span class="sxs-lookup"><span data-stu-id="f0a10-121">None</span></span>|<span data-ttu-id="f0a10-122">删除[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="f0a10-122">Deletes a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>|
|[<span data-ttu-id="f0a10-123">更新 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="f0a10-123">Update deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-update.md)|[<span data-ttu-id="f0a10-124">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="f0a10-124">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="f0a10-125">更新[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f0a10-125">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f0a10-126">属性</span><span class="sxs-lookup"><span data-stu-id="f0a10-126">Properties</span></span>
|<span data-ttu-id="f0a10-127">属性</span><span class="sxs-lookup"><span data-stu-id="f0a10-127">Property</span></span>|<span data-ttu-id="f0a10-128">类型</span><span class="sxs-lookup"><span data-stu-id="f0a10-128">Type</span></span>|<span data-ttu-id="f0a10-129">说明</span><span class="sxs-lookup"><span data-stu-id="f0a10-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0a10-130">id</span><span class="sxs-lookup"><span data-stu-id="f0a10-130">id</span></span>|<span data-ttu-id="f0a10-131">String</span><span class="sxs-lookup"><span data-stu-id="f0a10-131">String</span></span>|<span data-ttu-id="f0a10-132">device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="f0a10-132">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="f0a10-133">target</span><span class="sxs-lookup"><span data-stu-id="f0a10-133">target</span></span>|[<span data-ttu-id="f0a10-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f0a10-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f0a10-135">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="f0a10-135">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0a10-136">关系</span><span class="sxs-lookup"><span data-stu-id="f0a10-136">Relationships</span></span>
<span data-ttu-id="f0a10-137">无</span><span class="sxs-lookup"><span data-stu-id="f0a10-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0a10-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0a10-138">JSON Representation</span></span>
<span data-ttu-id="f0a10-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0a10-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





