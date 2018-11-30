---
title: deviceManagementScriptAssignment 资源类型
description: 包含用于分配给组的设备管理脚本的属性。
ms.openlocfilehash: fb4be06fe36153cd9a015808823cf1e90d86a707
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048983"
---
# <a name="devicemanagementscriptassignment-resource-type"></a><span data-ttu-id="d2e18-103">deviceManagementScriptAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2e18-103">deviceManagementScriptAssignment resource type</span></span>

> <span data-ttu-id="d2e18-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d2e18-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2e18-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d2e18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2e18-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d2e18-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2e18-107">包含用于分配给组的设备管理脚本的属性。</span><span class="sxs-lookup"><span data-stu-id="d2e18-107">Contains properties used to assign a device management script to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="d2e18-108">方法</span><span class="sxs-lookup"><span data-stu-id="d2e18-108">Methods</span></span>
|<span data-ttu-id="d2e18-109">方法</span><span class="sxs-lookup"><span data-stu-id="d2e18-109">Method</span></span>|<span data-ttu-id="d2e18-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2e18-110">Return Type</span></span>|<span data-ttu-id="d2e18-111">说明</span><span class="sxs-lookup"><span data-stu-id="d2e18-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2e18-112">列表 deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="d2e18-112">List deviceManagementScriptAssignments</span></span>](../api/intune-devices-devicemanagementscriptassignment-list.md)|<span data-ttu-id="d2e18-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="d2e18-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="d2e18-114">列出属性和[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="d2e18-114">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="d2e18-115">获取 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d2e18-115">Get deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-get.md)|[<span data-ttu-id="d2e18-116">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d2e18-116">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="d2e18-117">读取属性和[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d2e18-117">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="d2e18-118">创建 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d2e18-118">Create deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-create.md)|[<span data-ttu-id="d2e18-119">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d2e18-119">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="d2e18-120">创建新的[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d2e18-120">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="d2e18-121">删除 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d2e18-121">Delete deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-delete.md)|<span data-ttu-id="d2e18-122">无</span><span class="sxs-lookup"><span data-stu-id="d2e18-122">None</span></span>|<span data-ttu-id="d2e18-123">删除[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="d2e18-123">Deletes a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>|
|[<span data-ttu-id="d2e18-124">更新 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d2e18-124">Update deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-update.md)|[<span data-ttu-id="d2e18-125">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d2e18-125">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="d2e18-126">更新[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d2e18-126">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2e18-127">属性</span><span class="sxs-lookup"><span data-stu-id="d2e18-127">Properties</span></span>
|<span data-ttu-id="d2e18-128">属性</span><span class="sxs-lookup"><span data-stu-id="d2e18-128">Property</span></span>|<span data-ttu-id="d2e18-129">类型</span><span class="sxs-lookup"><span data-stu-id="d2e18-129">Type</span></span>|<span data-ttu-id="d2e18-130">说明</span><span class="sxs-lookup"><span data-stu-id="d2e18-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2e18-131">id</span><span class="sxs-lookup"><span data-stu-id="d2e18-131">id</span></span>|<span data-ttu-id="d2e18-132">字符串</span><span class="sxs-lookup"><span data-stu-id="d2e18-132">String</span></span>|<span data-ttu-id="d2e18-133">设备管理脚本组工作分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="d2e18-133">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="d2e18-134">target</span><span class="sxs-lookup"><span data-stu-id="d2e18-134">target</span></span>|[<span data-ttu-id="d2e18-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d2e18-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d2e18-136">Azure Active Directory 组的 Id 目标脚本。</span><span class="sxs-lookup"><span data-stu-id="d2e18-136">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2e18-137">Relationships</span><span class="sxs-lookup"><span data-stu-id="d2e18-137">Relationships</span></span>
<span data-ttu-id="d2e18-138">无</span><span class="sxs-lookup"><span data-stu-id="d2e18-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2e18-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2e18-139">JSON Representation</span></span>
<span data-ttu-id="d2e18-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2e18-140">Here is a JSON representation of the resource.</span></span>
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





