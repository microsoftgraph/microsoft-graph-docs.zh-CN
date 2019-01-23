---
title: deviceConfigurationGroupAssignment 资源类型
description: 设备配置组工作分配。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ed94f08fb33fe4a999e71b85808f58853d40cad4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406820"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a><span data-ttu-id="3b8f2-103">deviceConfigurationGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b8f2-103">deviceConfigurationGroupAssignment resource type</span></span>

> <span data-ttu-id="3b8f2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="3b8f2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3b8f2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3b8f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b8f2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3b8f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b8f2-107">设备配置组工作分配。</span><span class="sxs-lookup"><span data-stu-id="3b8f2-107">Device configuration group assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="3b8f2-108">方法</span><span class="sxs-lookup"><span data-stu-id="3b8f2-108">Methods</span></span>
|<span data-ttu-id="3b8f2-109">方法</span><span class="sxs-lookup"><span data-stu-id="3b8f2-109">Method</span></span>|<span data-ttu-id="3b8f2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="3b8f2-110">Return Type</span></span>|<span data-ttu-id="3b8f2-111">说明</span><span class="sxs-lookup"><span data-stu-id="3b8f2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3b8f2-112">列表 deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="3b8f2-112">List deviceConfigurationGroupAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|<span data-ttu-id="3b8f2-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="3b8f2-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="3b8f2-114">列出属性和[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="3b8f2-114">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="3b8f2-115">获取 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3b8f2-115">Get deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[<span data-ttu-id="3b8f2-116">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3b8f2-116">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="3b8f2-117">读取属性和[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="3b8f2-117">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="3b8f2-118">创建 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3b8f2-118">Create deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[<span data-ttu-id="3b8f2-119">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3b8f2-119">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="3b8f2-120">创建新的[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3b8f2-120">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="3b8f2-121">删除 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3b8f2-121">Delete deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|<span data-ttu-id="3b8f2-122">无</span><span class="sxs-lookup"><span data-stu-id="3b8f2-122">None</span></span>|<span data-ttu-id="3b8f2-123">删除[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="3b8f2-123">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>|
|[<span data-ttu-id="3b8f2-124">更新 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3b8f2-124">Update deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[<span data-ttu-id="3b8f2-125">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3b8f2-125">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="3b8f2-126">更新[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3b8f2-126">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b8f2-127">属性</span><span class="sxs-lookup"><span data-stu-id="3b8f2-127">Properties</span></span>
|<span data-ttu-id="3b8f2-128">属性</span><span class="sxs-lookup"><span data-stu-id="3b8f2-128">Property</span></span>|<span data-ttu-id="3b8f2-129">类型</span><span class="sxs-lookup"><span data-stu-id="3b8f2-129">Type</span></span>|<span data-ttu-id="3b8f2-130">说明</span><span class="sxs-lookup"><span data-stu-id="3b8f2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b8f2-131">id</span><span class="sxs-lookup"><span data-stu-id="3b8f2-131">id</span></span>|<span data-ttu-id="3b8f2-132">String</span><span class="sxs-lookup"><span data-stu-id="3b8f2-132">String</span></span>|<span data-ttu-id="3b8f2-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3b8f2-133">Key of the entity.</span></span>|
|<span data-ttu-id="3b8f2-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="3b8f2-134">targetGroupId</span></span>|<span data-ttu-id="3b8f2-135">String</span><span class="sxs-lookup"><span data-stu-id="3b8f2-135">String</span></span>|<span data-ttu-id="3b8f2-136">AAD 组 Id 目标到该设备的配置。</span><span class="sxs-lookup"><span data-stu-id="3b8f2-136">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="3b8f2-137">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="3b8f2-137">excludeGroup</span></span>|<span data-ttu-id="3b8f2-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b8f2-138">Boolean</span></span>|<span data-ttu-id="3b8f2-139">指示此组是否应排除。</span><span class="sxs-lookup"><span data-stu-id="3b8f2-139">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="3b8f2-140">应包含的组的默认值</span><span class="sxs-lookup"><span data-stu-id="3b8f2-140">Defaults that the group should be included</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b8f2-141">关系</span><span class="sxs-lookup"><span data-stu-id="3b8f2-141">Relationships</span></span>
|<span data-ttu-id="3b8f2-142">关系</span><span class="sxs-lookup"><span data-stu-id="3b8f2-142">Relationship</span></span>|<span data-ttu-id="3b8f2-143">类型</span><span class="sxs-lookup"><span data-stu-id="3b8f2-143">Type</span></span>|<span data-ttu-id="3b8f2-144">说明</span><span class="sxs-lookup"><span data-stu-id="3b8f2-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b8f2-145">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3b8f2-145">deviceConfiguration</span></span>|[<span data-ttu-id="3b8f2-146">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3b8f2-146">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="3b8f2-147">导航链接到目标的设备配置。</span><span class="sxs-lookup"><span data-stu-id="3b8f2-147">The navigation link to the Device Configuration being targeted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b8f2-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b8f2-148">JSON Representation</span></span>
<span data-ttu-id="3b8f2-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b8f2-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String",
  "excludeGroup": true
}
```




