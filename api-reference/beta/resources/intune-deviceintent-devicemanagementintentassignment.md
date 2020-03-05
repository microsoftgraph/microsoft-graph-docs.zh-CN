---
title: deviceManagementIntentAssignment 资源类型
description: 意向分配实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a57ae19a679c96d6ed852b47e2d9ff1ea0eb3e27
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525304"
---
# <a name="devicemanagementintentassignment-resource-type"></a><span data-ttu-id="c6cad-103">deviceManagementIntentAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6cad-103">deviceManagementIntentAssignment resource type</span></span>

<span data-ttu-id="c6cad-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c6cad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6cad-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c6cad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6cad-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6cad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6cad-107">意向分配实体</span><span class="sxs-lookup"><span data-stu-id="c6cad-107">Intent assignment entity</span></span>

## <a name="methods"></a><span data-ttu-id="c6cad-108">方法</span><span class="sxs-lookup"><span data-stu-id="c6cad-108">Methods</span></span>
|<span data-ttu-id="c6cad-109">方法</span><span class="sxs-lookup"><span data-stu-id="c6cad-109">Method</span></span>|<span data-ttu-id="c6cad-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c6cad-110">Return Type</span></span>|<span data-ttu-id="c6cad-111">说明</span><span class="sxs-lookup"><span data-stu-id="c6cad-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c6cad-112">列出 deviceManagementIntentAssignments</span><span class="sxs-lookup"><span data-stu-id="c6cad-112">List deviceManagementIntentAssignments</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|<span data-ttu-id="c6cad-113">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c6cad-113">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="c6cad-114">列出[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c6cad-114">List properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) objects.</span></span>|
|[<span data-ttu-id="c6cad-115">获取 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="c6cad-115">Get deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[<span data-ttu-id="c6cad-116">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="c6cad-116">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="c6cad-117">读取[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c6cad-117">Read properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="c6cad-118">创建 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="c6cad-118">Create deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[<span data-ttu-id="c6cad-119">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="c6cad-119">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="c6cad-120">创建新的[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c6cad-120">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="c6cad-121">删除 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="c6cad-121">Delete deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|<span data-ttu-id="c6cad-122">无</span><span class="sxs-lookup"><span data-stu-id="c6cad-122">None</span></span>|<span data-ttu-id="c6cad-123">删除[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="c6cad-123">Deletes a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>|
|[<span data-ttu-id="c6cad-124">更新 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="c6cad-124">Update deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[<span data-ttu-id="c6cad-125">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="c6cad-125">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="c6cad-126">更新[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c6cad-126">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6cad-127">属性</span><span class="sxs-lookup"><span data-stu-id="c6cad-127">Properties</span></span>
|<span data-ttu-id="c6cad-128">属性</span><span class="sxs-lookup"><span data-stu-id="c6cad-128">Property</span></span>|<span data-ttu-id="c6cad-129">类型</span><span class="sxs-lookup"><span data-stu-id="c6cad-129">Type</span></span>|<span data-ttu-id="c6cad-130">说明</span><span class="sxs-lookup"><span data-stu-id="c6cad-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6cad-131">id</span><span class="sxs-lookup"><span data-stu-id="c6cad-131">id</span></span>|<span data-ttu-id="c6cad-132">String</span><span class="sxs-lookup"><span data-stu-id="c6cad-132">String</span></span>|<span data-ttu-id="c6cad-133">工作分配 ID</span><span class="sxs-lookup"><span data-stu-id="c6cad-133">The assignment ID</span></span>|
|<span data-ttu-id="c6cad-134">target</span><span class="sxs-lookup"><span data-stu-id="c6cad-134">target</span></span>|[<span data-ttu-id="c6cad-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c6cad-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c6cad-136">工作分配目标</span><span class="sxs-lookup"><span data-stu-id="c6cad-136">The assignment target</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6cad-137">关系</span><span class="sxs-lookup"><span data-stu-id="c6cad-137">Relationships</span></span>
<span data-ttu-id="c6cad-138">无</span><span class="sxs-lookup"><span data-stu-id="c6cad-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6cad-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6cad-139">JSON Representation</span></span>
<span data-ttu-id="c6cad-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6cad-140">Here is a JSON representation of the resource.</span></span>
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



