---
title: deviceConfigurationAssignment 资源类型
description: 设备配置分配实体将 AAD 组分配到特定设备配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ba4aae7fb8706996e0d80d3c3a227b99233b792d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333035"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="35cb8-103">deviceConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="35cb8-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="35cb8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35cb8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35cb8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35cb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35cb8-106">设备配置分配实体将 AAD 组分配到特定设备配置。</span><span class="sxs-lookup"><span data-stu-id="35cb8-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="35cb8-107">方法</span><span class="sxs-lookup"><span data-stu-id="35cb8-107">Methods</span></span>
|<span data-ttu-id="35cb8-108">方法</span><span class="sxs-lookup"><span data-stu-id="35cb8-108">Method</span></span>|<span data-ttu-id="35cb8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="35cb8-109">Return Type</span></span>|<span data-ttu-id="35cb8-110">说明</span><span class="sxs-lookup"><span data-stu-id="35cb8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="35cb8-111">列出 deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="35cb8-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="35cb8-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="35cb8-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="35cb8-113">列出 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="35cb8-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="35cb8-114">获取 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="35cb8-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="35cb8-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="35cb8-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="35cb8-116">读取 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="35cb8-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="35cb8-117">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="35cb8-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="35cb8-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="35cb8-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="35cb8-119">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="35cb8-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="35cb8-120">删除 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="35cb8-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="35cb8-121">无</span><span class="sxs-lookup"><span data-stu-id="35cb8-121">None</span></span>|<span data-ttu-id="35cb8-122">删除 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="35cb8-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="35cb8-123">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="35cb8-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="35cb8-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="35cb8-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="35cb8-125">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="35cb8-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="35cb8-126">属性</span><span class="sxs-lookup"><span data-stu-id="35cb8-126">Properties</span></span>
|<span data-ttu-id="35cb8-127">属性</span><span class="sxs-lookup"><span data-stu-id="35cb8-127">Property</span></span>|<span data-ttu-id="35cb8-128">类型</span><span class="sxs-lookup"><span data-stu-id="35cb8-128">Type</span></span>|<span data-ttu-id="35cb8-129">说明</span><span class="sxs-lookup"><span data-stu-id="35cb8-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35cb8-130">id</span><span class="sxs-lookup"><span data-stu-id="35cb8-130">id</span></span>|<span data-ttu-id="35cb8-131">String</span><span class="sxs-lookup"><span data-stu-id="35cb8-131">String</span></span>|<span data-ttu-id="35cb8-132">分配的键。</span><span class="sxs-lookup"><span data-stu-id="35cb8-132">The key of the assignment.</span></span>|
|<span data-ttu-id="35cb8-133">target</span><span class="sxs-lookup"><span data-stu-id="35cb8-133">target</span></span>|[<span data-ttu-id="35cb8-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="35cb8-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="35cb8-135">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="35cb8-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35cb8-136">关系</span><span class="sxs-lookup"><span data-stu-id="35cb8-136">Relationships</span></span>
<span data-ttu-id="35cb8-137">无</span><span class="sxs-lookup"><span data-stu-id="35cb8-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35cb8-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35cb8-138">JSON Representation</span></span>
<span data-ttu-id="35cb8-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35cb8-139">Here is a JSON representation of the resource.</span></span>
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



