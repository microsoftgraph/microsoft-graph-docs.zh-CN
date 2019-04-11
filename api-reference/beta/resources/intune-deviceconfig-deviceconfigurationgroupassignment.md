---
title: deviceConfigurationGroupAssignment 资源类型
description: 设备配置组分配。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1805cb29e8920876d8a340c9379d7b3200c4c779
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789162"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a><span data-ttu-id="098d0-103">deviceConfigurationGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="098d0-103">deviceConfigurationGroupAssignment resource type</span></span>

> <span data-ttu-id="098d0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="098d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="098d0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="098d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="098d0-106">设备配置组分配。</span><span class="sxs-lookup"><span data-stu-id="098d0-106">Device configuration group assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="098d0-107">方法</span><span class="sxs-lookup"><span data-stu-id="098d0-107">Methods</span></span>
|<span data-ttu-id="098d0-108">方法</span><span class="sxs-lookup"><span data-stu-id="098d0-108">Method</span></span>|<span data-ttu-id="098d0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="098d0-109">Return Type</span></span>|<span data-ttu-id="098d0-110">说明</span><span class="sxs-lookup"><span data-stu-id="098d0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="098d0-111">列出 deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="098d0-111">List deviceConfigurationGroupAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|<span data-ttu-id="098d0-112">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="098d0-112">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="098d0-113">列出[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="098d0-113">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="098d0-114">获取 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="098d0-114">Get deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[<span data-ttu-id="098d0-115">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="098d0-115">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="098d0-116">读取[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="098d0-116">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="098d0-117">创建 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="098d0-117">Create deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[<span data-ttu-id="098d0-118">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="098d0-118">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="098d0-119">创建新的[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="098d0-119">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="098d0-120">删除 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="098d0-120">Delete deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|<span data-ttu-id="098d0-121">无</span><span class="sxs-lookup"><span data-stu-id="098d0-121">None</span></span>|<span data-ttu-id="098d0-122">删除[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="098d0-122">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>|
|[<span data-ttu-id="098d0-123">更新 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="098d0-123">Update deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[<span data-ttu-id="098d0-124">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="098d0-124">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="098d0-125">更新[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="098d0-125">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="098d0-126">属性</span><span class="sxs-lookup"><span data-stu-id="098d0-126">Properties</span></span>
|<span data-ttu-id="098d0-127">属性</span><span class="sxs-lookup"><span data-stu-id="098d0-127">Property</span></span>|<span data-ttu-id="098d0-128">类型</span><span class="sxs-lookup"><span data-stu-id="098d0-128">Type</span></span>|<span data-ttu-id="098d0-129">说明</span><span class="sxs-lookup"><span data-stu-id="098d0-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="098d0-130">id</span><span class="sxs-lookup"><span data-stu-id="098d0-130">id</span></span>|<span data-ttu-id="098d0-131">String</span><span class="sxs-lookup"><span data-stu-id="098d0-131">String</span></span>|<span data-ttu-id="098d0-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="098d0-132">Key of the entity.</span></span>|
|<span data-ttu-id="098d0-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="098d0-133">targetGroupId</span></span>|<span data-ttu-id="098d0-134">String</span><span class="sxs-lookup"><span data-stu-id="098d0-134">String</span></span>|<span data-ttu-id="098d0-135">要将设备配置定向到的 AAD 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="098d0-135">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="098d0-136">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="098d0-136">excludeGroup</span></span>|<span data-ttu-id="098d0-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="098d0-137">Boolean</span></span>|<span data-ttu-id="098d0-138">指示是否应排除此组。</span><span class="sxs-lookup"><span data-stu-id="098d0-138">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="098d0-139">应包含组的默认值</span><span class="sxs-lookup"><span data-stu-id="098d0-139">Defaults that the group should be included</span></span>|

## <a name="relationships"></a><span data-ttu-id="098d0-140">关系</span><span class="sxs-lookup"><span data-stu-id="098d0-140">Relationships</span></span>
|<span data-ttu-id="098d0-141">关系</span><span class="sxs-lookup"><span data-stu-id="098d0-141">Relationship</span></span>|<span data-ttu-id="098d0-142">类型</span><span class="sxs-lookup"><span data-stu-id="098d0-142">Type</span></span>|<span data-ttu-id="098d0-143">说明</span><span class="sxs-lookup"><span data-stu-id="098d0-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="098d0-144">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="098d0-144">deviceConfiguration</span></span>|[<span data-ttu-id="098d0-145">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="098d0-145">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="098d0-146">指向要定向的设备配置的导航链接。</span><span class="sxs-lookup"><span data-stu-id="098d0-146">The navigation link to the Device Configuration being targeted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="098d0-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="098d0-147">JSON Representation</span></span>
<span data-ttu-id="098d0-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="098d0-148">Here is a JSON representation of the resource.</span></span>
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





