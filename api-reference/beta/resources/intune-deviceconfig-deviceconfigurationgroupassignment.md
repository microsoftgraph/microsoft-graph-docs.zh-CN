---
title: deviceConfigurationGroupAssignment 资源类型
description: 设备配置组工作分配。
author: tfitzmac
ms.openlocfilehash: 648edd8122c4e14ad06a6e8b19e5fb83a042affa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334634"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a><span data-ttu-id="6e802-103">deviceConfigurationGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="6e802-103">deviceConfigurationGroupAssignment resource type</span></span>

> <span data-ttu-id="6e802-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6e802-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e802-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6e802-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e802-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6e802-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e802-107">设备配置组工作分配。</span><span class="sxs-lookup"><span data-stu-id="6e802-107">Device configuration group assignment.</span></span>
## <a name="methods"></a><span data-ttu-id="6e802-108">方法</span><span class="sxs-lookup"><span data-stu-id="6e802-108">Methods</span></span>
|<span data-ttu-id="6e802-109">方法</span><span class="sxs-lookup"><span data-stu-id="6e802-109">Method</span></span>|<span data-ttu-id="6e802-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6e802-110">Return Type</span></span>|<span data-ttu-id="6e802-111">说明</span><span class="sxs-lookup"><span data-stu-id="6e802-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6e802-112">列表 deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="6e802-112">List deviceConfigurationGroupAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|<span data-ttu-id="6e802-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="6e802-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="6e802-114">列出属性和[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="6e802-114">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="6e802-115">获取 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6e802-115">Get deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[<span data-ttu-id="6e802-116">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6e802-116">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="6e802-117">读取属性和[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="6e802-117">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="6e802-118">创建 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6e802-118">Create deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[<span data-ttu-id="6e802-119">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6e802-119">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="6e802-120">创建新的[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6e802-120">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="6e802-121">删除 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6e802-121">Delete deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|<span data-ttu-id="6e802-122">无</span><span class="sxs-lookup"><span data-stu-id="6e802-122">None</span></span>|<span data-ttu-id="6e802-123">删除[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="6e802-123">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>|
|[<span data-ttu-id="6e802-124">更新 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6e802-124">Update deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[<span data-ttu-id="6e802-125">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6e802-125">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="6e802-126">更新[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6e802-126">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e802-127">属性</span><span class="sxs-lookup"><span data-stu-id="6e802-127">Properties</span></span>
|<span data-ttu-id="6e802-128">属性</span><span class="sxs-lookup"><span data-stu-id="6e802-128">Property</span></span>|<span data-ttu-id="6e802-129">类型</span><span class="sxs-lookup"><span data-stu-id="6e802-129">Type</span></span>|<span data-ttu-id="6e802-130">说明</span><span class="sxs-lookup"><span data-stu-id="6e802-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e802-131">id</span><span class="sxs-lookup"><span data-stu-id="6e802-131">id</span></span>|<span data-ttu-id="6e802-132">String</span><span class="sxs-lookup"><span data-stu-id="6e802-132">String</span></span>|<span data-ttu-id="6e802-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6e802-133">Key of the entity.</span></span>|
|<span data-ttu-id="6e802-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="6e802-134">targetGroupId</span></span>|<span data-ttu-id="6e802-135">字符串</span><span class="sxs-lookup"><span data-stu-id="6e802-135">String</span></span>|<span data-ttu-id="6e802-136">AAD 组 Id 目标到该设备的配置。</span><span class="sxs-lookup"><span data-stu-id="6e802-136">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="6e802-137">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="6e802-137">excludeGroup</span></span>|<span data-ttu-id="6e802-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e802-138">Boolean</span></span>|<span data-ttu-id="6e802-139">指示此组是否应排除。</span><span class="sxs-lookup"><span data-stu-id="6e802-139">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="6e802-140">应包含的组的默认值</span><span class="sxs-lookup"><span data-stu-id="6e802-140">Defaults that the group should be included</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e802-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="6e802-141">Relationships</span></span>
|<span data-ttu-id="6e802-142">关系</span><span class="sxs-lookup"><span data-stu-id="6e802-142">Relationship</span></span>|<span data-ttu-id="6e802-143">类型</span><span class="sxs-lookup"><span data-stu-id="6e802-143">Type</span></span>|<span data-ttu-id="6e802-144">说明</span><span class="sxs-lookup"><span data-stu-id="6e802-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e802-145">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e802-145">deviceConfiguration</span></span>|[<span data-ttu-id="6e802-146">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e802-146">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="6e802-147">导航链接到目标的设备配置。</span><span class="sxs-lookup"><span data-stu-id="6e802-147">The navigation link to the Device Configuration being targeted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e802-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6e802-148">JSON Representation</span></span>
<span data-ttu-id="6e802-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e802-149">Here is a JSON representation of the resource.</span></span>
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





