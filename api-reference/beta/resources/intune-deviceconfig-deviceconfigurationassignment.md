---
title: deviceConfigurationAssignment 资源类型
description: 设备配置分配实体将 AAD 组分配到特定设备配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3580454eae767f9a9ca84e3ab196d66fb0c363d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993163"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="23402-103">deviceConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="23402-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="23402-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23402-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23402-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23402-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23402-106">设备配置分配实体将 AAD 组分配到特定设备配置。</span><span class="sxs-lookup"><span data-stu-id="23402-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="23402-107">方法</span><span class="sxs-lookup"><span data-stu-id="23402-107">Methods</span></span>
|<span data-ttu-id="23402-108">方法</span><span class="sxs-lookup"><span data-stu-id="23402-108">Method</span></span>|<span data-ttu-id="23402-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="23402-109">Return Type</span></span>|<span data-ttu-id="23402-110">说明</span><span class="sxs-lookup"><span data-stu-id="23402-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="23402-111">列出 deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="23402-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="23402-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="23402-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="23402-113">列出 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="23402-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="23402-114">获取 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="23402-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="23402-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="23402-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="23402-116">读取 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="23402-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="23402-117">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="23402-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="23402-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="23402-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="23402-119">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="23402-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="23402-120">删除 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="23402-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="23402-121">无</span><span class="sxs-lookup"><span data-stu-id="23402-121">None</span></span>|<span data-ttu-id="23402-122">删除 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="23402-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="23402-123">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="23402-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="23402-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="23402-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="23402-125">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="23402-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="23402-126">属性</span><span class="sxs-lookup"><span data-stu-id="23402-126">Properties</span></span>
|<span data-ttu-id="23402-127">属性</span><span class="sxs-lookup"><span data-stu-id="23402-127">Property</span></span>|<span data-ttu-id="23402-128">类型</span><span class="sxs-lookup"><span data-stu-id="23402-128">Type</span></span>|<span data-ttu-id="23402-129">说明</span><span class="sxs-lookup"><span data-stu-id="23402-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23402-130">id</span><span class="sxs-lookup"><span data-stu-id="23402-130">id</span></span>|<span data-ttu-id="23402-131">String</span><span class="sxs-lookup"><span data-stu-id="23402-131">String</span></span>|<span data-ttu-id="23402-132">分配的键。</span><span class="sxs-lookup"><span data-stu-id="23402-132">The key of the assignment.</span></span>|
|<span data-ttu-id="23402-133">target</span><span class="sxs-lookup"><span data-stu-id="23402-133">target</span></span>|[<span data-ttu-id="23402-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="23402-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="23402-135">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="23402-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23402-136">关系</span><span class="sxs-lookup"><span data-stu-id="23402-136">Relationships</span></span>
<span data-ttu-id="23402-137">无</span><span class="sxs-lookup"><span data-stu-id="23402-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23402-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23402-138">JSON Representation</span></span>
<span data-ttu-id="23402-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23402-139">Here is a JSON representation of the resource.</span></span>
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





