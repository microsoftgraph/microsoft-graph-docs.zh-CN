---
title: deviceManagementIntentAssignment 资源类型
description: 意向分配实体
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a0aa4794953120fd1250c14638f4c6cfb0488dc1
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793505"
---
# <a name="devicemanagementintentassignment-resource-type"></a><span data-ttu-id="1b7f7-103">deviceManagementIntentAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b7f7-103">deviceManagementIntentAssignment resource type</span></span>

<span data-ttu-id="1b7f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b7f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b7f7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1b7f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b7f7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b7f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b7f7-107">意向分配实体</span><span class="sxs-lookup"><span data-stu-id="1b7f7-107">Intent assignment entity</span></span>

## <a name="methods"></a><span data-ttu-id="1b7f7-108">Methods</span><span class="sxs-lookup"><span data-stu-id="1b7f7-108">Methods</span></span>
|<span data-ttu-id="1b7f7-109">方法</span><span class="sxs-lookup"><span data-stu-id="1b7f7-109">Method</span></span>|<span data-ttu-id="1b7f7-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1b7f7-110">Return Type</span></span>|<span data-ttu-id="1b7f7-111">说明</span><span class="sxs-lookup"><span data-stu-id="1b7f7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1b7f7-112">列出 deviceManagementIntentAssignments</span><span class="sxs-lookup"><span data-stu-id="1b7f7-112">List deviceManagementIntentAssignments</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|<span data-ttu-id="1b7f7-113">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1b7f7-113">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="1b7f7-114">列出[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b7f7-114">List properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) objects.</span></span>|
|[<span data-ttu-id="1b7f7-115">获取 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="1b7f7-115">Get deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[<span data-ttu-id="1b7f7-116">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="1b7f7-116">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="1b7f7-117">读取[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b7f7-117">Read properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="1b7f7-118">创建 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="1b7f7-118">Create deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[<span data-ttu-id="1b7f7-119">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="1b7f7-119">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="1b7f7-120">创建新的[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1b7f7-120">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="1b7f7-121">删除 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="1b7f7-121">Delete deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|<span data-ttu-id="1b7f7-122">无</span><span class="sxs-lookup"><span data-stu-id="1b7f7-122">None</span></span>|<span data-ttu-id="1b7f7-123">删除[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="1b7f7-123">Deletes a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>|
|[<span data-ttu-id="1b7f7-124">更新 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="1b7f7-124">Update deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[<span data-ttu-id="1b7f7-125">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="1b7f7-125">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="1b7f7-126">更新[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1b7f7-126">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1b7f7-127">属性</span><span class="sxs-lookup"><span data-stu-id="1b7f7-127">Properties</span></span>
|<span data-ttu-id="1b7f7-128">属性</span><span class="sxs-lookup"><span data-stu-id="1b7f7-128">Property</span></span>|<span data-ttu-id="1b7f7-129">类型</span><span class="sxs-lookup"><span data-stu-id="1b7f7-129">Type</span></span>|<span data-ttu-id="1b7f7-130">说明</span><span class="sxs-lookup"><span data-stu-id="1b7f7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b7f7-131">id</span><span class="sxs-lookup"><span data-stu-id="1b7f7-131">id</span></span>|<span data-ttu-id="1b7f7-132">String</span><span class="sxs-lookup"><span data-stu-id="1b7f7-132">String</span></span>|<span data-ttu-id="1b7f7-133">工作分配 ID</span><span class="sxs-lookup"><span data-stu-id="1b7f7-133">The assignment ID</span></span>|
|<span data-ttu-id="1b7f7-134">target</span><span class="sxs-lookup"><span data-stu-id="1b7f7-134">target</span></span>|[<span data-ttu-id="1b7f7-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1b7f7-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1b7f7-136">工作分配目标</span><span class="sxs-lookup"><span data-stu-id="1b7f7-136">The assignment target</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b7f7-137">关系</span><span class="sxs-lookup"><span data-stu-id="1b7f7-137">Relationships</span></span>
<span data-ttu-id="1b7f7-138">无</span><span class="sxs-lookup"><span data-stu-id="1b7f7-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b7f7-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b7f7-139">JSON Representation</span></span>
<span data-ttu-id="1b7f7-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b7f7-140">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```



