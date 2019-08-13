---
title: deviceManagementIntentAssignment 资源类型
description: 意向分配实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c9964e3ef34cc000e102b5ecc253acdb54e92e7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371759"
---
# <a name="devicemanagementintentassignment-resource-type"></a><span data-ttu-id="93c3f-103">deviceManagementIntentAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="93c3f-103">deviceManagementIntentAssignment resource type</span></span>

> <span data-ttu-id="93c3f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="93c3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93c3f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="93c3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93c3f-106">意向分配实体</span><span class="sxs-lookup"><span data-stu-id="93c3f-106">Intent assignment entity</span></span>

## <a name="methods"></a><span data-ttu-id="93c3f-107">方法</span><span class="sxs-lookup"><span data-stu-id="93c3f-107">Methods</span></span>
|<span data-ttu-id="93c3f-108">方法</span><span class="sxs-lookup"><span data-stu-id="93c3f-108">Method</span></span>|<span data-ttu-id="93c3f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="93c3f-109">Return Type</span></span>|<span data-ttu-id="93c3f-110">说明</span><span class="sxs-lookup"><span data-stu-id="93c3f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="93c3f-111">列出 deviceManagementIntentAssignments</span><span class="sxs-lookup"><span data-stu-id="93c3f-111">List deviceManagementIntentAssignments</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|<span data-ttu-id="93c3f-112">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="93c3f-112">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="93c3f-113">列出[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="93c3f-113">List properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) objects.</span></span>|
|[<span data-ttu-id="93c3f-114">获取 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="93c3f-114">Get deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[<span data-ttu-id="93c3f-115">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="93c3f-115">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="93c3f-116">读取[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="93c3f-116">Read properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="93c3f-117">创建 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="93c3f-117">Create deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[<span data-ttu-id="93c3f-118">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="93c3f-118">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="93c3f-119">创建新的[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="93c3f-119">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="93c3f-120">删除 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="93c3f-120">Delete deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|<span data-ttu-id="93c3f-121">无</span><span class="sxs-lookup"><span data-stu-id="93c3f-121">None</span></span>|<span data-ttu-id="93c3f-122">删除[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="93c3f-122">Deletes a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>|
|[<span data-ttu-id="93c3f-123">更新 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="93c3f-123">Update deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[<span data-ttu-id="93c3f-124">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="93c3f-124">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="93c3f-125">更新[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="93c3f-125">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="93c3f-126">属性</span><span class="sxs-lookup"><span data-stu-id="93c3f-126">Properties</span></span>
|<span data-ttu-id="93c3f-127">属性</span><span class="sxs-lookup"><span data-stu-id="93c3f-127">Property</span></span>|<span data-ttu-id="93c3f-128">类型</span><span class="sxs-lookup"><span data-stu-id="93c3f-128">Type</span></span>|<span data-ttu-id="93c3f-129">说明</span><span class="sxs-lookup"><span data-stu-id="93c3f-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93c3f-130">id</span><span class="sxs-lookup"><span data-stu-id="93c3f-130">id</span></span>|<span data-ttu-id="93c3f-131">String</span><span class="sxs-lookup"><span data-stu-id="93c3f-131">String</span></span>|<span data-ttu-id="93c3f-132">工作分配 ID</span><span class="sxs-lookup"><span data-stu-id="93c3f-132">The assignment ID</span></span>|
|<span data-ttu-id="93c3f-133">target</span><span class="sxs-lookup"><span data-stu-id="93c3f-133">target</span></span>|[<span data-ttu-id="93c3f-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="93c3f-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="93c3f-135">工作分配目标</span><span class="sxs-lookup"><span data-stu-id="93c3f-135">The assignment target</span></span>|

## <a name="relationships"></a><span data-ttu-id="93c3f-136">关系</span><span class="sxs-lookup"><span data-stu-id="93c3f-136">Relationships</span></span>
<span data-ttu-id="93c3f-137">无</span><span class="sxs-lookup"><span data-stu-id="93c3f-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93c3f-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93c3f-138">JSON Representation</span></span>
<span data-ttu-id="93c3f-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93c3f-139">Here is a JSON representation of the resource.</span></span>
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



