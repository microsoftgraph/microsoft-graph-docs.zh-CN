---
title: windowsFeatureUpdateProfileAssignment 资源类型
description: 此实体包含用于将 windows 功能更新配置文件分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a71545503db977ed3ca98da9fb6d8be80d537218
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702241"
---
# <a name="windowsfeatureupdateprofileassignment-resource-type"></a><span data-ttu-id="bf773-103">windowsFeatureUpdateProfileAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf773-103">windowsFeatureUpdateProfileAssignment resource type</span></span>

<span data-ttu-id="bf773-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf773-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf773-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bf773-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf773-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf773-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf773-107">此实体包含用于将 windows 功能更新配置文件分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="bf773-107">This entity contains the properties used to assign a windows feature update profile to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="bf773-108">Methods</span><span class="sxs-lookup"><span data-stu-id="bf773-108">Methods</span></span>
|<span data-ttu-id="bf773-109">方法</span><span class="sxs-lookup"><span data-stu-id="bf773-109">Method</span></span>|<span data-ttu-id="bf773-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="bf773-110">Return Type</span></span>|<span data-ttu-id="bf773-111">说明</span><span class="sxs-lookup"><span data-stu-id="bf773-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bf773-112">列出 windowsFeatureUpdateProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="bf773-112">List windowsFeatureUpdateProfileAssignments</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-list.md)|<span data-ttu-id="bf773-113">[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bf773-113">[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) collection</span></span>|<span data-ttu-id="bf773-114">列出 [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bf773-114">List properties and relationships of the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) objects.</span></span>|
|[<span data-ttu-id="bf773-115">获取 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="bf773-115">Get windowsFeatureUpdateProfileAssignment</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-get.md)|[<span data-ttu-id="bf773-116">windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="bf773-116">windowsFeatureUpdateProfileAssignment</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|<span data-ttu-id="bf773-117">读取 [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bf773-117">Read properties and relationships of the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="bf773-118">创建 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="bf773-118">Create windowsFeatureUpdateProfileAssignment</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-create.md)|[<span data-ttu-id="bf773-119">windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="bf773-119">windowsFeatureUpdateProfileAssignment</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|<span data-ttu-id="bf773-120">创建新的 [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bf773-120">Create a new [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="bf773-121">删除 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="bf773-121">Delete windowsFeatureUpdateProfileAssignment</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-delete.md)|<span data-ttu-id="bf773-122">无</span><span class="sxs-lookup"><span data-stu-id="bf773-122">None</span></span>|<span data-ttu-id="bf773-123">删除 [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="bf773-123">Deletes a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).</span></span>|
|[<span data-ttu-id="bf773-124">更新 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="bf773-124">Update windowsFeatureUpdateProfileAssignment</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-update.md)|[<span data-ttu-id="bf773-125">windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="bf773-125">windowsFeatureUpdateProfileAssignment</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|<span data-ttu-id="bf773-126">更新 [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bf773-126">Update the properties of a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bf773-127">属性</span><span class="sxs-lookup"><span data-stu-id="bf773-127">Properties</span></span>
|<span data-ttu-id="bf773-128">属性</span><span class="sxs-lookup"><span data-stu-id="bf773-128">Property</span></span>|<span data-ttu-id="bf773-129">类型</span><span class="sxs-lookup"><span data-stu-id="bf773-129">Type</span></span>|<span data-ttu-id="bf773-130">说明</span><span class="sxs-lookup"><span data-stu-id="bf773-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf773-131">id</span><span class="sxs-lookup"><span data-stu-id="bf773-131">id</span></span>|<span data-ttu-id="bf773-132">String</span><span class="sxs-lookup"><span data-stu-id="bf773-132">String</span></span>|<span data-ttu-id="bf773-133">实体的标识符</span><span class="sxs-lookup"><span data-stu-id="bf773-133">The Identifier of the entity</span></span>|
|<span data-ttu-id="bf773-134">target</span><span class="sxs-lookup"><span data-stu-id="bf773-134">target</span></span>|[<span data-ttu-id="bf773-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bf773-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bf773-136">将功能更新配置文件分配到的工作分配目标。</span><span class="sxs-lookup"><span data-stu-id="bf773-136">The assignment target that the feature update profile is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf773-137">关系</span><span class="sxs-lookup"><span data-stu-id="bf773-137">Relationships</span></span>
<span data-ttu-id="bf773-138">无</span><span class="sxs-lookup"><span data-stu-id="bf773-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf773-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf773-139">JSON Representation</span></span>
<span data-ttu-id="bf773-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf773-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsFeatureUpdateProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```





