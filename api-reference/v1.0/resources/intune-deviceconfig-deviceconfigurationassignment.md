---
title: deviceConfigurationAssignment 资源类型
description: 设备配置分配实体将 AAD 组分配到特定设备配置。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60fb4f0a782d9502f9e3da3f0a7da2389e937a7d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573415"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="553eb-103">deviceConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="553eb-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="553eb-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="553eb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="553eb-105">设备配置分配实体将 AAD 组分配到特定设备配置。</span><span class="sxs-lookup"><span data-stu-id="553eb-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="553eb-106">方法</span><span class="sxs-lookup"><span data-stu-id="553eb-106">Methods</span></span>
|<span data-ttu-id="553eb-107">方法</span><span class="sxs-lookup"><span data-stu-id="553eb-107">Method</span></span>|<span data-ttu-id="553eb-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="553eb-108">Return Type</span></span>|<span data-ttu-id="553eb-109">说明</span><span class="sxs-lookup"><span data-stu-id="553eb-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="553eb-110">列出 deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="553eb-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="553eb-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="553eb-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="553eb-112">列出 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="553eb-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="553eb-113">获取 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="553eb-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="553eb-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="553eb-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="553eb-115">读取 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="553eb-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="553eb-116">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="553eb-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="553eb-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="553eb-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="553eb-118">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="553eb-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="553eb-119">删除 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="553eb-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="553eb-120">无</span><span class="sxs-lookup"><span data-stu-id="553eb-120">None</span></span>|<span data-ttu-id="553eb-121">删除 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="553eb-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="553eb-122">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="553eb-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="553eb-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="553eb-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="553eb-124">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="553eb-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="553eb-125">属性</span><span class="sxs-lookup"><span data-stu-id="553eb-125">Properties</span></span>
|<span data-ttu-id="553eb-126">属性</span><span class="sxs-lookup"><span data-stu-id="553eb-126">Property</span></span>|<span data-ttu-id="553eb-127">类型</span><span class="sxs-lookup"><span data-stu-id="553eb-127">Type</span></span>|<span data-ttu-id="553eb-128">说明</span><span class="sxs-lookup"><span data-stu-id="553eb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="553eb-129">id</span><span class="sxs-lookup"><span data-stu-id="553eb-129">id</span></span>|<span data-ttu-id="553eb-130">String</span><span class="sxs-lookup"><span data-stu-id="553eb-130">String</span></span>|<span data-ttu-id="553eb-131">分配的键。</span><span class="sxs-lookup"><span data-stu-id="553eb-131">The key of the assignment.</span></span>|
|<span data-ttu-id="553eb-132">target</span><span class="sxs-lookup"><span data-stu-id="553eb-132">target</span></span>|[<span data-ttu-id="553eb-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="553eb-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="553eb-134">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="553eb-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="553eb-135">关系</span><span class="sxs-lookup"><span data-stu-id="553eb-135">Relationships</span></span>
<span data-ttu-id="553eb-136">无</span><span class="sxs-lookup"><span data-stu-id="553eb-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="553eb-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="553eb-137">JSON Representation</span></span>
<span data-ttu-id="553eb-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="553eb-138">Here is a JSON representation of the resource.</span></span>
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



