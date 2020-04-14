---
title: windowsFeatureUpdateProfileAssignment 资源类型
description: 此实体包含用于将 windows 功能更新配置文件分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 888fc7e0737f0ba7de6b7813a8f6855de60b2422
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436922"
---
# <a name="windowsfeatureupdateprofileassignment-resource-type"></a><span data-ttu-id="b7f9a-103">windowsFeatureUpdateProfileAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7f9a-103">windowsFeatureUpdateProfileAssignment resource type</span></span>

<span data-ttu-id="b7f9a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7f9a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7f9a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b7f9a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7f9a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7f9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7f9a-107">此实体包含用于将 windows 功能更新配置文件分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="b7f9a-107">This entity contains the properties used to assign a windows feature update profile to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="b7f9a-108">方法</span><span class="sxs-lookup"><span data-stu-id="b7f9a-108">Methods</span></span>
|<span data-ttu-id="b7f9a-109">方法</span><span class="sxs-lookup"><span data-stu-id="b7f9a-109">Method</span></span>|<span data-ttu-id="b7f9a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b7f9a-110">Return Type</span></span>|<span data-ttu-id="b7f9a-111">说明</span><span class="sxs-lookup"><span data-stu-id="b7f9a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b7f9a-112">列出 windowsFeatureUpdateProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="b7f9a-112">List windowsFeatureUpdateProfileAssignments</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-list.md)|<span data-ttu-id="b7f9a-113">[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="b7f9a-113">[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) collection</span></span>|<span data-ttu-id="b7f9a-114">列出[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b7f9a-114">List properties and relationships of the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) objects.</span></span>|
|[<span data-ttu-id="b7f9a-115">获取 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="b7f9a-115">Get windowsFeatureUpdateProfileAssignment</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-get.md)|[<span data-ttu-id="b7f9a-116">windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="b7f9a-116">windowsFeatureUpdateProfileAssignment</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|<span data-ttu-id="b7f9a-117">读取[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b7f9a-117">Read properties and relationships of the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="b7f9a-118">创建 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="b7f9a-118">Create windowsFeatureUpdateProfileAssignment</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-create.md)|[<span data-ttu-id="b7f9a-119">windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="b7f9a-119">windowsFeatureUpdateProfileAssignment</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|<span data-ttu-id="b7f9a-120">创建新的[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b7f9a-120">Create a new [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="b7f9a-121">删除 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="b7f9a-121">Delete windowsFeatureUpdateProfileAssignment</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-delete.md)|<span data-ttu-id="b7f9a-122">无</span><span class="sxs-lookup"><span data-stu-id="b7f9a-122">None</span></span>|<span data-ttu-id="b7f9a-123">删除[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="b7f9a-123">Deletes a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).</span></span>|
|[<span data-ttu-id="b7f9a-124">更新 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="b7f9a-124">Update windowsFeatureUpdateProfileAssignment</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-update.md)|[<span data-ttu-id="b7f9a-125">windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="b7f9a-125">windowsFeatureUpdateProfileAssignment</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|<span data-ttu-id="b7f9a-126">更新[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b7f9a-126">Update the properties of a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b7f9a-127">属性</span><span class="sxs-lookup"><span data-stu-id="b7f9a-127">Properties</span></span>
|<span data-ttu-id="b7f9a-128">属性</span><span class="sxs-lookup"><span data-stu-id="b7f9a-128">Property</span></span>|<span data-ttu-id="b7f9a-129">类型</span><span class="sxs-lookup"><span data-stu-id="b7f9a-129">Type</span></span>|<span data-ttu-id="b7f9a-130">说明</span><span class="sxs-lookup"><span data-stu-id="b7f9a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7f9a-131">id</span><span class="sxs-lookup"><span data-stu-id="b7f9a-131">id</span></span>|<span data-ttu-id="b7f9a-132">String</span><span class="sxs-lookup"><span data-stu-id="b7f9a-132">String</span></span>|<span data-ttu-id="b7f9a-133">实体的标识符</span><span class="sxs-lookup"><span data-stu-id="b7f9a-133">The Identifier of the entity</span></span>|
|<span data-ttu-id="b7f9a-134">target</span><span class="sxs-lookup"><span data-stu-id="b7f9a-134">target</span></span>|[<span data-ttu-id="b7f9a-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b7f9a-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b7f9a-136">将功能更新配置文件分配到的工作分配目标。</span><span class="sxs-lookup"><span data-stu-id="b7f9a-136">The assignment target that the feature update profile is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7f9a-137">关系</span><span class="sxs-lookup"><span data-stu-id="b7f9a-137">Relationships</span></span>
<span data-ttu-id="b7f9a-138">无</span><span class="sxs-lookup"><span data-stu-id="b7f9a-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7f9a-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7f9a-139">JSON Representation</span></span>
<span data-ttu-id="b7f9a-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7f9a-140">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



