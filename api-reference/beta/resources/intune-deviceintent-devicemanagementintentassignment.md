---
title: deviceManagementIntentAssignment 资源类型
description: 意向分配实体
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a955187e079e1f77accb21361bfe49689f52108
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522424"
---
# <a name="devicemanagementintentassignment-resource-type"></a><span data-ttu-id="0bd2b-103">deviceManagementIntentAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="0bd2b-103">deviceManagementIntentAssignment resource type</span></span>

> <span data-ttu-id="0bd2b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0bd2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bd2b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0bd2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bd2b-106">意向分配实体</span><span class="sxs-lookup"><span data-stu-id="0bd2b-106">Intent assignment entity</span></span>

## <a name="methods"></a><span data-ttu-id="0bd2b-107">方法</span><span class="sxs-lookup"><span data-stu-id="0bd2b-107">Methods</span></span>
|<span data-ttu-id="0bd2b-108">方法</span><span class="sxs-lookup"><span data-stu-id="0bd2b-108">Method</span></span>|<span data-ttu-id="0bd2b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0bd2b-109">Return Type</span></span>|<span data-ttu-id="0bd2b-110">说明</span><span class="sxs-lookup"><span data-stu-id="0bd2b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0bd2b-111">列出 deviceManagementIntentAssignments</span><span class="sxs-lookup"><span data-stu-id="0bd2b-111">List deviceManagementIntentAssignments</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|<span data-ttu-id="0bd2b-112">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0bd2b-112">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="0bd2b-113">列出[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0bd2b-113">List properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) objects.</span></span>|
|[<span data-ttu-id="0bd2b-114">获取 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="0bd2b-114">Get deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[<span data-ttu-id="0bd2b-115">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="0bd2b-115">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="0bd2b-116">读取[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0bd2b-116">Read properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="0bd2b-117">创建 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="0bd2b-117">Create deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[<span data-ttu-id="0bd2b-118">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="0bd2b-118">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="0bd2b-119">创建新的[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0bd2b-119">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="0bd2b-120">删除 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="0bd2b-120">Delete deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|<span data-ttu-id="0bd2b-121">无</span><span class="sxs-lookup"><span data-stu-id="0bd2b-121">None</span></span>|<span data-ttu-id="0bd2b-122">删除[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="0bd2b-122">Deletes a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>|
|[<span data-ttu-id="0bd2b-123">更新 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="0bd2b-123">Update deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[<span data-ttu-id="0bd2b-124">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="0bd2b-124">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="0bd2b-125">更新[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0bd2b-125">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0bd2b-126">属性</span><span class="sxs-lookup"><span data-stu-id="0bd2b-126">Properties</span></span>
|<span data-ttu-id="0bd2b-127">属性</span><span class="sxs-lookup"><span data-stu-id="0bd2b-127">Property</span></span>|<span data-ttu-id="0bd2b-128">类型</span><span class="sxs-lookup"><span data-stu-id="0bd2b-128">Type</span></span>|<span data-ttu-id="0bd2b-129">说明</span><span class="sxs-lookup"><span data-stu-id="0bd2b-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bd2b-130">id</span><span class="sxs-lookup"><span data-stu-id="0bd2b-130">id</span></span>|<span data-ttu-id="0bd2b-131">String</span><span class="sxs-lookup"><span data-stu-id="0bd2b-131">String</span></span>|<span data-ttu-id="0bd2b-132">工作分配 ID</span><span class="sxs-lookup"><span data-stu-id="0bd2b-132">The assignment ID</span></span>|
|<span data-ttu-id="0bd2b-133">target</span><span class="sxs-lookup"><span data-stu-id="0bd2b-133">target</span></span>|[<span data-ttu-id="0bd2b-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0bd2b-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0bd2b-135">工作分配目标</span><span class="sxs-lookup"><span data-stu-id="0bd2b-135">The assignment target</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bd2b-136">关系</span><span class="sxs-lookup"><span data-stu-id="0bd2b-136">Relationships</span></span>
<span data-ttu-id="0bd2b-137">无</span><span class="sxs-lookup"><span data-stu-id="0bd2b-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bd2b-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0bd2b-138">JSON Representation</span></span>
<span data-ttu-id="0bd2b-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0bd2b-139">Here is a JSON representation of the resource.</span></span>
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







