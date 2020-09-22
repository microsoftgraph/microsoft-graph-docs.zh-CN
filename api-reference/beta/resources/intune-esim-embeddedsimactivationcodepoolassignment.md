---
title: embeddedSIMActivationCodePoolAssignment 资源类型
description: 嵌入的 SIM 激活代码池分配实体可将特定的 embeddedSIMActivationCodePool 分配给 AAD 设备组。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d3b3a22e7b49d96395ade47f3bbf097bfe07a8ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031464"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a><span data-ttu-id="09e0a-103">embeddedSIMActivationCodePoolAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="09e0a-103">embeddedSIMActivationCodePoolAssignment resource type</span></span>

<span data-ttu-id="09e0a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09e0a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09e0a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="09e0a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09e0a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09e0a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09e0a-107">嵌入的 SIM 激活代码池分配实体可将特定的 embeddedSIMActivationCodePool 分配给 AAD 设备组。</span><span class="sxs-lookup"><span data-stu-id="09e0a-107">The embedded SIM activation code pool assignment entity assigns a specific embeddedSIMActivationCodePool to an AAD device group.</span></span>

## <a name="methods"></a><span data-ttu-id="09e0a-108">方法</span><span class="sxs-lookup"><span data-stu-id="09e0a-108">Methods</span></span>
|<span data-ttu-id="09e0a-109">方法</span><span class="sxs-lookup"><span data-stu-id="09e0a-109">Method</span></span>|<span data-ttu-id="09e0a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="09e0a-110">Return Type</span></span>|<span data-ttu-id="09e0a-111">说明</span><span class="sxs-lookup"><span data-stu-id="09e0a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="09e0a-112">列出 embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="09e0a-112">List embeddedSIMActivationCodePoolAssignments</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|<span data-ttu-id="09e0a-113">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="09e0a-113">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="09e0a-114">列出 [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="09e0a-114">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>|
|[<span data-ttu-id="09e0a-115">获取 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0a-115">Get embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[<span data-ttu-id="09e0a-116">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0a-116">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="09e0a-117">读取 [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="09e0a-117">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="09e0a-118">创建 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0a-118">Create embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[<span data-ttu-id="09e0a-119">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0a-119">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="09e0a-120">创建新的 [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="09e0a-120">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="09e0a-121">删除 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0a-121">Delete embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|<span data-ttu-id="09e0a-122">无</span><span class="sxs-lookup"><span data-stu-id="09e0a-122">None</span></span>|<span data-ttu-id="09e0a-123">删除 [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="09e0a-123">Deletes a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>|
|[<span data-ttu-id="09e0a-124">更新 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0a-124">Update embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[<span data-ttu-id="09e0a-125">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="09e0a-125">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="09e0a-126">更新 [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="09e0a-126">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="09e0a-127">属性</span><span class="sxs-lookup"><span data-stu-id="09e0a-127">Properties</span></span>
|<span data-ttu-id="09e0a-128">属性</span><span class="sxs-lookup"><span data-stu-id="09e0a-128">Property</span></span>|<span data-ttu-id="09e0a-129">类型</span><span class="sxs-lookup"><span data-stu-id="09e0a-129">Type</span></span>|<span data-ttu-id="09e0a-130">说明</span><span class="sxs-lookup"><span data-stu-id="09e0a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09e0a-131">id</span><span class="sxs-lookup"><span data-stu-id="09e0a-131">id</span></span>|<span data-ttu-id="09e0a-132">String</span><span class="sxs-lookup"><span data-stu-id="09e0a-132">String</span></span>|<span data-ttu-id="09e0a-133">嵌入的 SIM 激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="09e0a-133">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="09e0a-134">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="09e0a-134">System generated value assigned when created.</span></span>|
|<span data-ttu-id="09e0a-135">target</span><span class="sxs-lookup"><span data-stu-id="09e0a-135">target</span></span>|[<span data-ttu-id="09e0a-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="09e0a-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="09e0a-137">嵌入的 SIM 激活代码池的目标组的类型。</span><span class="sxs-lookup"><span data-stu-id="09e0a-137">The type of groups targeted by the embedded SIM activation code pool.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09e0a-138">关系</span><span class="sxs-lookup"><span data-stu-id="09e0a-138">Relationships</span></span>
<span data-ttu-id="09e0a-139">无</span><span class="sxs-lookup"><span data-stu-id="09e0a-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09e0a-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09e0a-140">JSON Representation</span></span>
<span data-ttu-id="09e0a-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09e0a-141">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```






