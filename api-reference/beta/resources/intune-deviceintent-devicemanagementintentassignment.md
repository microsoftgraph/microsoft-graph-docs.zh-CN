---
title: deviceManagementIntentAssignment 资源类型
description: 意图分配实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5dc2fc81635f3c5e4c61fb70a3bab5f176ee09a8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161507"
---
# <a name="devicemanagementintentassignment-resource-type"></a><span data-ttu-id="2e2e6-103">deviceManagementIntentAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e2e6-103">deviceManagementIntentAssignment resource type</span></span>

<span data-ttu-id="2e2e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e2e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e2e6-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2e2e6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e2e6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2e2e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e2e6-107">意图分配实体</span><span class="sxs-lookup"><span data-stu-id="2e2e6-107">Intent assignment entity</span></span>

## <a name="methods"></a><span data-ttu-id="2e2e6-108">方法</span><span class="sxs-lookup"><span data-stu-id="2e2e6-108">Methods</span></span>
|<span data-ttu-id="2e2e6-109">方法</span><span class="sxs-lookup"><span data-stu-id="2e2e6-109">Method</span></span>|<span data-ttu-id="2e2e6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2e2e6-110">Return Type</span></span>|<span data-ttu-id="2e2e6-111">说明</span><span class="sxs-lookup"><span data-stu-id="2e2e6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2e2e6-112">列出 deviceManagementIntentAssignments</span><span class="sxs-lookup"><span data-stu-id="2e2e6-112">List deviceManagementIntentAssignments</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|<span data-ttu-id="2e2e6-113">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2e2e6-113">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="2e2e6-114">列出 [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2e2e6-114">List properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) objects.</span></span>|
|[<span data-ttu-id="2e2e6-115">获取 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="2e2e6-115">Get deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[<span data-ttu-id="2e2e6-116">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="2e2e6-116">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="2e2e6-117">读取 [deviceManagementIntentAssignment 对象的属性和](../resources/intune-deviceintent-devicemanagementintentassignment.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="2e2e6-117">Read properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="2e2e6-118">创建 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="2e2e6-118">Create deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[<span data-ttu-id="2e2e6-119">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="2e2e6-119">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="2e2e6-120">创建新的 [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2e2e6-120">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="2e2e6-121">删除 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="2e2e6-121">Delete deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|<span data-ttu-id="2e2e6-122">无</span><span class="sxs-lookup"><span data-stu-id="2e2e6-122">None</span></span>|<span data-ttu-id="2e2e6-123">删除 [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="2e2e6-123">Deletes a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>|
|[<span data-ttu-id="2e2e6-124">更新 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="2e2e6-124">Update deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[<span data-ttu-id="2e2e6-125">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="2e2e6-125">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="2e2e6-126">更新 [deviceManagementIntentAssignment 对象](../resources/intune-deviceintent-devicemanagementintentassignment.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="2e2e6-126">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2e2e6-127">属性</span><span class="sxs-lookup"><span data-stu-id="2e2e6-127">Properties</span></span>
|<span data-ttu-id="2e2e6-128">属性</span><span class="sxs-lookup"><span data-stu-id="2e2e6-128">Property</span></span>|<span data-ttu-id="2e2e6-129">类型</span><span class="sxs-lookup"><span data-stu-id="2e2e6-129">Type</span></span>|<span data-ttu-id="2e2e6-130">说明</span><span class="sxs-lookup"><span data-stu-id="2e2e6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e2e6-131">id</span><span class="sxs-lookup"><span data-stu-id="2e2e6-131">id</span></span>|<span data-ttu-id="2e2e6-132">String</span><span class="sxs-lookup"><span data-stu-id="2e2e6-132">String</span></span>|<span data-ttu-id="2e2e6-133">工作分配 ID</span><span class="sxs-lookup"><span data-stu-id="2e2e6-133">The assignment ID</span></span>|
|<span data-ttu-id="2e2e6-134">target</span><span class="sxs-lookup"><span data-stu-id="2e2e6-134">target</span></span>|[<span data-ttu-id="2e2e6-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2e2e6-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2e2e6-136">工作分配目标</span><span class="sxs-lookup"><span data-stu-id="2e2e6-136">The assignment target</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e2e6-137">关系</span><span class="sxs-lookup"><span data-stu-id="2e2e6-137">Relationships</span></span>
<span data-ttu-id="2e2e6-138">无</span><span class="sxs-lookup"><span data-stu-id="2e2e6-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e2e6-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e2e6-139">JSON Representation</span></span>
<span data-ttu-id="2e2e6-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e2e6-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




