---
title: deviceConfigurationGroupAssignment 资源类型
description: 设备配置组分配。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ae84489009eac1e01d399c2b90f81ed12e5b5da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026773"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a><span data-ttu-id="4bb94-103">deviceConfigurationGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="4bb94-103">deviceConfigurationGroupAssignment resource type</span></span>

<span data-ttu-id="4bb94-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bb94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4bb94-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4bb94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bb94-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4bb94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bb94-107">设备配置组分配。</span><span class="sxs-lookup"><span data-stu-id="4bb94-107">Device configuration group assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="4bb94-108">方法</span><span class="sxs-lookup"><span data-stu-id="4bb94-108">Methods</span></span>
|<span data-ttu-id="4bb94-109">方法</span><span class="sxs-lookup"><span data-stu-id="4bb94-109">Method</span></span>|<span data-ttu-id="4bb94-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4bb94-110">Return Type</span></span>|<span data-ttu-id="4bb94-111">说明</span><span class="sxs-lookup"><span data-stu-id="4bb94-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4bb94-112">列出 deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="4bb94-112">List deviceConfigurationGroupAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|<span data-ttu-id="4bb94-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4bb94-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="4bb94-114">列出 [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4bb94-114">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="4bb94-115">获取 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4bb94-115">Get deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[<span data-ttu-id="4bb94-116">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4bb94-116">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="4bb94-117">读取 [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4bb94-117">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="4bb94-118">创建 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4bb94-118">Create deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[<span data-ttu-id="4bb94-119">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4bb94-119">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="4bb94-120">创建新的 [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4bb94-120">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="4bb94-121">删除 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4bb94-121">Delete deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|<span data-ttu-id="4bb94-122">无</span><span class="sxs-lookup"><span data-stu-id="4bb94-122">None</span></span>|<span data-ttu-id="4bb94-123">删除 [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="4bb94-123">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>|
|[<span data-ttu-id="4bb94-124">更新 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4bb94-124">Update deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[<span data-ttu-id="4bb94-125">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4bb94-125">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="4bb94-126">更新 [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4bb94-126">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4bb94-127">属性</span><span class="sxs-lookup"><span data-stu-id="4bb94-127">Properties</span></span>
|<span data-ttu-id="4bb94-128">属性</span><span class="sxs-lookup"><span data-stu-id="4bb94-128">Property</span></span>|<span data-ttu-id="4bb94-129">类型</span><span class="sxs-lookup"><span data-stu-id="4bb94-129">Type</span></span>|<span data-ttu-id="4bb94-130">说明</span><span class="sxs-lookup"><span data-stu-id="4bb94-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bb94-131">id</span><span class="sxs-lookup"><span data-stu-id="4bb94-131">id</span></span>|<span data-ttu-id="4bb94-132">String</span><span class="sxs-lookup"><span data-stu-id="4bb94-132">String</span></span>|<span data-ttu-id="4bb94-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4bb94-133">Key of the entity.</span></span>|
|<span data-ttu-id="4bb94-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="4bb94-134">targetGroupId</span></span>|<span data-ttu-id="4bb94-135">String</span><span class="sxs-lookup"><span data-stu-id="4bb94-135">String</span></span>|<span data-ttu-id="4bb94-136">要将设备配置定向到的 AAD 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="4bb94-136">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="4bb94-137">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="4bb94-137">excludeGroup</span></span>|<span data-ttu-id="4bb94-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bb94-138">Boolean</span></span>|<span data-ttu-id="4bb94-139">指示是否应排除此组。</span><span class="sxs-lookup"><span data-stu-id="4bb94-139">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="4bb94-140">应包含组的默认值</span><span class="sxs-lookup"><span data-stu-id="4bb94-140">Defaults that the group should be included</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bb94-141">关系</span><span class="sxs-lookup"><span data-stu-id="4bb94-141">Relationships</span></span>
|<span data-ttu-id="4bb94-142">关系</span><span class="sxs-lookup"><span data-stu-id="4bb94-142">Relationship</span></span>|<span data-ttu-id="4bb94-143">类型</span><span class="sxs-lookup"><span data-stu-id="4bb94-143">Type</span></span>|<span data-ttu-id="4bb94-144">说明</span><span class="sxs-lookup"><span data-stu-id="4bb94-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bb94-145">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4bb94-145">deviceConfiguration</span></span>|[<span data-ttu-id="4bb94-146">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4bb94-146">deviceConfiguration</span></span>](../resources/intune-shared-deviceconfiguration.md)|<span data-ttu-id="4bb94-147">指向要定向的设备配置的导航链接。</span><span class="sxs-lookup"><span data-stu-id="4bb94-147">The navigation link to the Device Configuration being targeted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4bb94-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4bb94-148">JSON Representation</span></span>
<span data-ttu-id="4bb94-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4bb94-149">Here is a JSON representation of the resource.</span></span>
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






