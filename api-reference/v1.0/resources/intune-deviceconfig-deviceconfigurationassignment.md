---
title: deviceConfigurationAssignment 资源类型
description: 设备配置分配实体将 AAD 组分配到特定设备配置。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 522fbcadd2d8326249600dcf352d8c3dfc54cf8b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530784"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="e093e-103">deviceConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="e093e-103">deviceConfigurationAssignment resource type</span></span>

<span data-ttu-id="e093e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e093e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e093e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e093e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e093e-106">设备配置分配实体将 AAD 组分配到特定设备配置。</span><span class="sxs-lookup"><span data-stu-id="e093e-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="e093e-107">Methods</span><span class="sxs-lookup"><span data-stu-id="e093e-107">Methods</span></span>
|<span data-ttu-id="e093e-108">方法</span><span class="sxs-lookup"><span data-stu-id="e093e-108">Method</span></span>|<span data-ttu-id="e093e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e093e-109">Return Type</span></span>|<span data-ttu-id="e093e-110">说明</span><span class="sxs-lookup"><span data-stu-id="e093e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e093e-111">列出 deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="e093e-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="e093e-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e093e-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e093e-113">列出 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e093e-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="e093e-114">获取 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e093e-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="e093e-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e093e-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="e093e-116">读取 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e093e-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="e093e-117">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e093e-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="e093e-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e093e-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="e093e-119">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e093e-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="e093e-120">删除 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e093e-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="e093e-121">无</span><span class="sxs-lookup"><span data-stu-id="e093e-121">None</span></span>|<span data-ttu-id="e093e-122">删除 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="e093e-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="e093e-123">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e093e-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="e093e-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e093e-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="e093e-125">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e093e-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e093e-126">属性</span><span class="sxs-lookup"><span data-stu-id="e093e-126">Properties</span></span>
|<span data-ttu-id="e093e-127">属性</span><span class="sxs-lookup"><span data-stu-id="e093e-127">Property</span></span>|<span data-ttu-id="e093e-128">类型</span><span class="sxs-lookup"><span data-stu-id="e093e-128">Type</span></span>|<span data-ttu-id="e093e-129">说明</span><span class="sxs-lookup"><span data-stu-id="e093e-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e093e-130">id</span><span class="sxs-lookup"><span data-stu-id="e093e-130">id</span></span>|<span data-ttu-id="e093e-131">字符串</span><span class="sxs-lookup"><span data-stu-id="e093e-131">String</span></span>|<span data-ttu-id="e093e-132">分配的键。</span><span class="sxs-lookup"><span data-stu-id="e093e-132">The key of the assignment.</span></span>|
|<span data-ttu-id="e093e-133">target</span><span class="sxs-lookup"><span data-stu-id="e093e-133">target</span></span>|[<span data-ttu-id="e093e-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e093e-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e093e-135">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="e093e-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e093e-136">关系</span><span class="sxs-lookup"><span data-stu-id="e093e-136">Relationships</span></span>
<span data-ttu-id="e093e-137">无</span><span class="sxs-lookup"><span data-stu-id="e093e-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e093e-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e093e-138">JSON Representation</span></span>
<span data-ttu-id="e093e-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e093e-139">Here is a JSON representation of the resource.</span></span>
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




