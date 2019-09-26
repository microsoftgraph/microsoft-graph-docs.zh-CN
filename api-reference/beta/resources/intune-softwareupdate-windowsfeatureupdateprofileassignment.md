---
title: windowsFeatureUpdateProfileAssignment 资源类型
description: 此实体包含用于将 windows 功能更新配置文件分配给组的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 33808607c626196ac4627ea354da6f1f36e3f4ec
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199892"
---
# <a name="windowsfeatureupdateprofileassignment-resource-type"></a><span data-ttu-id="5c603-103">windowsFeatureUpdateProfileAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c603-103">windowsFeatureUpdateProfileAssignment resource type</span></span>

> <span data-ttu-id="5c603-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5c603-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c603-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c603-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c603-106">此实体包含用于将 windows 功能更新配置文件分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="5c603-106">This entity contains the properties used to assign a windows feature update profile to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="5c603-107">方法</span><span class="sxs-lookup"><span data-stu-id="5c603-107">Methods</span></span>
|<span data-ttu-id="5c603-108">方法</span><span class="sxs-lookup"><span data-stu-id="5c603-108">Method</span></span>|<span data-ttu-id="5c603-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5c603-109">Return Type</span></span>|<span data-ttu-id="5c603-110">说明</span><span class="sxs-lookup"><span data-stu-id="5c603-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5c603-111">列出 windowsFeatureUpdateProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="5c603-111">List windowsFeatureUpdateProfileAssignments</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-list.md)|<span data-ttu-id="5c603-112">[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5c603-112">[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) collection</span></span>|<span data-ttu-id="5c603-113">列出[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5c603-113">List properties and relationships of the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) objects.</span></span>|
|[<span data-ttu-id="5c603-114">获取 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="5c603-114">Get windowsFeatureUpdateProfileAssignment</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-get.md)|[<span data-ttu-id="5c603-115">windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="5c603-115">windowsFeatureUpdateProfileAssignment</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|<span data-ttu-id="5c603-116">读取[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5c603-116">Read properties and relationships of the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="5c603-117">创建 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="5c603-117">Create windowsFeatureUpdateProfileAssignment</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-create.md)|[<span data-ttu-id="5c603-118">windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="5c603-118">windowsFeatureUpdateProfileAssignment</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|<span data-ttu-id="5c603-119">创建新的[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5c603-119">Create a new [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="5c603-120">删除 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="5c603-120">Delete windowsFeatureUpdateProfileAssignment</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-delete.md)|<span data-ttu-id="5c603-121">无</span><span class="sxs-lookup"><span data-stu-id="5c603-121">None</span></span>|<span data-ttu-id="5c603-122">删除[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="5c603-122">Deletes a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).</span></span>|
|[<span data-ttu-id="5c603-123">更新 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="5c603-123">Update windowsFeatureUpdateProfileAssignment</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-update.md)|[<span data-ttu-id="5c603-124">windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="5c603-124">windowsFeatureUpdateProfileAssignment</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|<span data-ttu-id="5c603-125">更新[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5c603-125">Update the properties of a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5c603-126">属性</span><span class="sxs-lookup"><span data-stu-id="5c603-126">Properties</span></span>
|<span data-ttu-id="5c603-127">属性</span><span class="sxs-lookup"><span data-stu-id="5c603-127">Property</span></span>|<span data-ttu-id="5c603-128">类型</span><span class="sxs-lookup"><span data-stu-id="5c603-128">Type</span></span>|<span data-ttu-id="5c603-129">说明</span><span class="sxs-lookup"><span data-stu-id="5c603-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c603-130">id</span><span class="sxs-lookup"><span data-stu-id="5c603-130">id</span></span>|<span data-ttu-id="5c603-131">String</span><span class="sxs-lookup"><span data-stu-id="5c603-131">String</span></span>|<span data-ttu-id="5c603-132">实体的标识符</span><span class="sxs-lookup"><span data-stu-id="5c603-132">The Identifier of the entity</span></span>|
|<span data-ttu-id="5c603-133">target</span><span class="sxs-lookup"><span data-stu-id="5c603-133">target</span></span>|[<span data-ttu-id="5c603-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5c603-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5c603-135">将功能更新配置文件分配到的工作分配目标。</span><span class="sxs-lookup"><span data-stu-id="5c603-135">The assignment target that the feature update profile is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c603-136">关系</span><span class="sxs-lookup"><span data-stu-id="5c603-136">Relationships</span></span>
<span data-ttu-id="5c603-137">无</span><span class="sxs-lookup"><span data-stu-id="5c603-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c603-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c603-138">JSON Representation</span></span>
<span data-ttu-id="5c603-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c603-139">Here is a JSON representation of the resource.</span></span>
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



