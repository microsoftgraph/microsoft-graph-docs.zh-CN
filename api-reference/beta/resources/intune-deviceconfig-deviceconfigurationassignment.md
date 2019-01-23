---
title: deviceConfigurationAssignment 资源类型
description: 设备配置分配实体将 AAD 组分配到特定设备配置。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 115cbd779e53f303bdbf95dc28916879726676ee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402599"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="217c6-103">deviceConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="217c6-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="217c6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="217c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="217c6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="217c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="217c6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="217c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="217c6-107">设备配置分配实体将 AAD 组分配到特定设备配置。</span><span class="sxs-lookup"><span data-stu-id="217c6-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="217c6-108">方法</span><span class="sxs-lookup"><span data-stu-id="217c6-108">Methods</span></span>
|<span data-ttu-id="217c6-109">方法</span><span class="sxs-lookup"><span data-stu-id="217c6-109">Method</span></span>|<span data-ttu-id="217c6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="217c6-110">Return Type</span></span>|<span data-ttu-id="217c6-111">说明</span><span class="sxs-lookup"><span data-stu-id="217c6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="217c6-112">列出 deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="217c6-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="217c6-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="217c6-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="217c6-114">列出 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="217c6-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="217c6-115">获取 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="217c6-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="217c6-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="217c6-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="217c6-117">读取 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="217c6-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="217c6-118">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="217c6-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="217c6-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="217c6-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="217c6-120">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="217c6-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="217c6-121">删除 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="217c6-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="217c6-122">无</span><span class="sxs-lookup"><span data-stu-id="217c6-122">None</span></span>|<span data-ttu-id="217c6-123">删除 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="217c6-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="217c6-124">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="217c6-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="217c6-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="217c6-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="217c6-126">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="217c6-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="217c6-127">属性</span><span class="sxs-lookup"><span data-stu-id="217c6-127">Properties</span></span>
|<span data-ttu-id="217c6-128">属性</span><span class="sxs-lookup"><span data-stu-id="217c6-128">Property</span></span>|<span data-ttu-id="217c6-129">类型</span><span class="sxs-lookup"><span data-stu-id="217c6-129">Type</span></span>|<span data-ttu-id="217c6-130">说明</span><span class="sxs-lookup"><span data-stu-id="217c6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="217c6-131">id</span><span class="sxs-lookup"><span data-stu-id="217c6-131">id</span></span>|<span data-ttu-id="217c6-132">String</span><span class="sxs-lookup"><span data-stu-id="217c6-132">String</span></span>|<span data-ttu-id="217c6-133">分配的键。</span><span class="sxs-lookup"><span data-stu-id="217c6-133">The key of the assignment.</span></span>|
|<span data-ttu-id="217c6-134">target</span><span class="sxs-lookup"><span data-stu-id="217c6-134">target</span></span>|[<span data-ttu-id="217c6-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="217c6-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="217c6-136">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="217c6-136">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="217c6-137">关系</span><span class="sxs-lookup"><span data-stu-id="217c6-137">Relationships</span></span>
<span data-ttu-id="217c6-138">无</span><span class="sxs-lookup"><span data-stu-id="217c6-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="217c6-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="217c6-139">JSON Representation</span></span>
<span data-ttu-id="217c6-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="217c6-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




