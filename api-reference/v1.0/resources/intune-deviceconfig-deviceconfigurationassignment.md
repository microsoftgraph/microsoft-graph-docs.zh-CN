---
title: deviceConfigurationAssignment 资源类型
description: 设备配置分配实体将 AAD 组分配到特定设备配置。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da23212914f7ffa5a04b1d976140e2baf69df11c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359528"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="2a278-103">deviceConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a278-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="2a278-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a278-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a278-105">设备配置分配实体将 AAD 组分配到特定设备配置。</span><span class="sxs-lookup"><span data-stu-id="2a278-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="2a278-106">方法</span><span class="sxs-lookup"><span data-stu-id="2a278-106">Methods</span></span>
|<span data-ttu-id="2a278-107">方法</span><span class="sxs-lookup"><span data-stu-id="2a278-107">Method</span></span>|<span data-ttu-id="2a278-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2a278-108">Return Type</span></span>|<span data-ttu-id="2a278-109">说明</span><span class="sxs-lookup"><span data-stu-id="2a278-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2a278-110">列出 deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="2a278-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="2a278-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2a278-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2a278-112">列出 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2a278-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="2a278-113">获取 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a278-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="2a278-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a278-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="2a278-115">读取 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2a278-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="2a278-116">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a278-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="2a278-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a278-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="2a278-118">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a278-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="2a278-119">删除 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a278-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="2a278-120">无</span><span class="sxs-lookup"><span data-stu-id="2a278-120">None</span></span>|<span data-ttu-id="2a278-121">删除 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="2a278-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="2a278-122">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a278-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="2a278-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a278-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="2a278-124">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2a278-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a278-125">属性</span><span class="sxs-lookup"><span data-stu-id="2a278-125">Properties</span></span>
|<span data-ttu-id="2a278-126">属性</span><span class="sxs-lookup"><span data-stu-id="2a278-126">Property</span></span>|<span data-ttu-id="2a278-127">类型</span><span class="sxs-lookup"><span data-stu-id="2a278-127">Type</span></span>|<span data-ttu-id="2a278-128">说明</span><span class="sxs-lookup"><span data-stu-id="2a278-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a278-129">id</span><span class="sxs-lookup"><span data-stu-id="2a278-129">id</span></span>|<span data-ttu-id="2a278-130">String</span><span class="sxs-lookup"><span data-stu-id="2a278-130">String</span></span>|<span data-ttu-id="2a278-131">分配的键。</span><span class="sxs-lookup"><span data-stu-id="2a278-131">The key of the assignment.</span></span>|
|<span data-ttu-id="2a278-132">target</span><span class="sxs-lookup"><span data-stu-id="2a278-132">target</span></span>|[<span data-ttu-id="2a278-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2a278-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2a278-134">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="2a278-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a278-135">关系</span><span class="sxs-lookup"><span data-stu-id="2a278-135">Relationships</span></span>
<span data-ttu-id="2a278-136">无</span><span class="sxs-lookup"><span data-stu-id="2a278-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a278-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a278-137">JSON Representation</span></span>
<span data-ttu-id="2a278-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a278-138">Here is a JSON representation of the resource.</span></span>
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




