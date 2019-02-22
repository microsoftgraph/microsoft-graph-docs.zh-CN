---
title: embeddedSIMActivationCodePoolAssignment 资源类型
description: 嵌入的 SIM 激活代码池分配实体可将特定的 embeddedSIMActivationCodePool 分配给 AAD 设备组。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60b92a7b1232ba19a4166171fa118b18f7a263b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163390"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a><span data-ttu-id="cdc2d-103">embeddedSIMActivationCodePoolAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="cdc2d-103">embeddedSIMActivationCodePoolAssignment resource type</span></span>

> <span data-ttu-id="cdc2d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cdc2d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdc2d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cdc2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdc2d-106">嵌入的 SIM 激活代码池分配实体可将特定的 embeddedSIMActivationCodePool 分配给 AAD 设备组。</span><span class="sxs-lookup"><span data-stu-id="cdc2d-106">The embedded SIM activation code pool assignment entity assigns a specific embeddedSIMActivationCodePool to an AAD device group.</span></span>

## <a name="methods"></a><span data-ttu-id="cdc2d-107">方法</span><span class="sxs-lookup"><span data-stu-id="cdc2d-107">Methods</span></span>
|<span data-ttu-id="cdc2d-108">方法</span><span class="sxs-lookup"><span data-stu-id="cdc2d-108">Method</span></span>|<span data-ttu-id="cdc2d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cdc2d-109">Return Type</span></span>|<span data-ttu-id="cdc2d-110">说明</span><span class="sxs-lookup"><span data-stu-id="cdc2d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cdc2d-111">列出 embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="cdc2d-111">List embeddedSIMActivationCodePoolAssignments</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|<span data-ttu-id="cdc2d-112">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="cdc2d-112">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="cdc2d-113">列出[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cdc2d-113">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>|
|[<span data-ttu-id="cdc2d-114">获取 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="cdc2d-114">Get embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[<span data-ttu-id="cdc2d-115">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="cdc2d-115">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="cdc2d-116">读取[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cdc2d-116">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="cdc2d-117">创建 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="cdc2d-117">Create embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[<span data-ttu-id="cdc2d-118">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="cdc2d-118">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="cdc2d-119">创建新的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cdc2d-119">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="cdc2d-120">删除 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="cdc2d-120">Delete embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|<span data-ttu-id="cdc2d-121">无</span><span class="sxs-lookup"><span data-stu-id="cdc2d-121">None</span></span>|<span data-ttu-id="cdc2d-122">删除[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="cdc2d-122">Deletes a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>|
|[<span data-ttu-id="cdc2d-123">更新 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="cdc2d-123">Update embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[<span data-ttu-id="cdc2d-124">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="cdc2d-124">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="cdc2d-125">更新[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cdc2d-125">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cdc2d-126">属性</span><span class="sxs-lookup"><span data-stu-id="cdc2d-126">Properties</span></span>
|<span data-ttu-id="cdc2d-127">属性</span><span class="sxs-lookup"><span data-stu-id="cdc2d-127">Property</span></span>|<span data-ttu-id="cdc2d-128">类型</span><span class="sxs-lookup"><span data-stu-id="cdc2d-128">Type</span></span>|<span data-ttu-id="cdc2d-129">说明</span><span class="sxs-lookup"><span data-stu-id="cdc2d-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdc2d-130">id</span><span class="sxs-lookup"><span data-stu-id="cdc2d-130">id</span></span>|<span data-ttu-id="cdc2d-131">字符串</span><span class="sxs-lookup"><span data-stu-id="cdc2d-131">String</span></span>|<span data-ttu-id="cdc2d-132">嵌入的 SIM 激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cdc2d-132">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="cdc2d-133">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="cdc2d-133">System generated value assigned when created.</span></span>|
|<span data-ttu-id="cdc2d-134">target</span><span class="sxs-lookup"><span data-stu-id="cdc2d-134">target</span></span>|[<span data-ttu-id="cdc2d-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cdc2d-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cdc2d-136">嵌入的 SIM 激活代码池的目标组的类型。</span><span class="sxs-lookup"><span data-stu-id="cdc2d-136">The type of groups targeted by the embedded SIM activation code pool.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdc2d-137">关系</span><span class="sxs-lookup"><span data-stu-id="cdc2d-137">Relationships</span></span>
<span data-ttu-id="cdc2d-138">无</span><span class="sxs-lookup"><span data-stu-id="cdc2d-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdc2d-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cdc2d-139">JSON Representation</span></span>
<span data-ttu-id="cdc2d-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cdc2d-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePoolAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




