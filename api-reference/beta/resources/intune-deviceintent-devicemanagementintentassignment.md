---
title: deviceManagementIntentAssignment 资源类型
description: 意向分配实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9a5d5ce8d55f70684ef4ce5e0a3c5ff6bf7e536
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964008"
---
# <a name="devicemanagementintentassignment-resource-type"></a><span data-ttu-id="4706e-103">deviceManagementIntentAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="4706e-103">deviceManagementIntentAssignment resource type</span></span>

> <span data-ttu-id="4706e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4706e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4706e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4706e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4706e-106">意向分配实体</span><span class="sxs-lookup"><span data-stu-id="4706e-106">Intent assignment entity</span></span>

## <a name="methods"></a><span data-ttu-id="4706e-107">方法</span><span class="sxs-lookup"><span data-stu-id="4706e-107">Methods</span></span>
|<span data-ttu-id="4706e-108">方法</span><span class="sxs-lookup"><span data-stu-id="4706e-108">Method</span></span>|<span data-ttu-id="4706e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4706e-109">Return Type</span></span>|<span data-ttu-id="4706e-110">说明</span><span class="sxs-lookup"><span data-stu-id="4706e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4706e-111">列出 deviceManagementIntentAssignments</span><span class="sxs-lookup"><span data-stu-id="4706e-111">List deviceManagementIntentAssignments</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|<span data-ttu-id="4706e-112">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="4706e-112">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="4706e-113">列出[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4706e-113">List properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) objects.</span></span>|
|[<span data-ttu-id="4706e-114">获取 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="4706e-114">Get deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[<span data-ttu-id="4706e-115">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="4706e-115">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="4706e-116">读取[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4706e-116">Read properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="4706e-117">创建 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="4706e-117">Create deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[<span data-ttu-id="4706e-118">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="4706e-118">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="4706e-119">创建新的[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4706e-119">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="4706e-120">删除 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="4706e-120">Delete deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|<span data-ttu-id="4706e-121">无</span><span class="sxs-lookup"><span data-stu-id="4706e-121">None</span></span>|<span data-ttu-id="4706e-122">删除[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="4706e-122">Deletes a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>|
|[<span data-ttu-id="4706e-123">更新 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="4706e-123">Update deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[<span data-ttu-id="4706e-124">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="4706e-124">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="4706e-125">更新[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4706e-125">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4706e-126">属性</span><span class="sxs-lookup"><span data-stu-id="4706e-126">Properties</span></span>
|<span data-ttu-id="4706e-127">属性</span><span class="sxs-lookup"><span data-stu-id="4706e-127">Property</span></span>|<span data-ttu-id="4706e-128">类型</span><span class="sxs-lookup"><span data-stu-id="4706e-128">Type</span></span>|<span data-ttu-id="4706e-129">说明</span><span class="sxs-lookup"><span data-stu-id="4706e-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4706e-130">id</span><span class="sxs-lookup"><span data-stu-id="4706e-130">id</span></span>|<span data-ttu-id="4706e-131">String</span><span class="sxs-lookup"><span data-stu-id="4706e-131">String</span></span>|<span data-ttu-id="4706e-132">工作分配 ID</span><span class="sxs-lookup"><span data-stu-id="4706e-132">The assignment ID</span></span>|
|<span data-ttu-id="4706e-133">target</span><span class="sxs-lookup"><span data-stu-id="4706e-133">target</span></span>|[<span data-ttu-id="4706e-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4706e-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4706e-135">工作分配目标</span><span class="sxs-lookup"><span data-stu-id="4706e-135">The assignment target</span></span>|

## <a name="relationships"></a><span data-ttu-id="4706e-136">关系</span><span class="sxs-lookup"><span data-stu-id="4706e-136">Relationships</span></span>
<span data-ttu-id="4706e-137">无</span><span class="sxs-lookup"><span data-stu-id="4706e-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4706e-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4706e-138">JSON Representation</span></span>
<span data-ttu-id="4706e-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4706e-139">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





