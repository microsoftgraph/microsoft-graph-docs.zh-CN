---
title: embeddedSIMActivationCodePoolAssignment 资源类型
description: 嵌入的 SIM 激活代码池分配实体可将特定的 embeddedSIMActivationCodePool 分配给 AAD 设备组。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 295e30c56551a03bc671579cc37851f50e2513ec
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979247"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a><span data-ttu-id="1d1d4-103">embeddedSIMActivationCodePoolAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d1d4-103">embeddedSIMActivationCodePoolAssignment resource type</span></span>

> <span data-ttu-id="1d1d4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1d1d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d1d4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d1d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d1d4-106">嵌入的 SIM 激活代码池分配实体可将特定的 embeddedSIMActivationCodePool 分配给 AAD 设备组。</span><span class="sxs-lookup"><span data-stu-id="1d1d4-106">The embedded SIM activation code pool assignment entity assigns a specific embeddedSIMActivationCodePool to an AAD device group.</span></span>

## <a name="methods"></a><span data-ttu-id="1d1d4-107">方法</span><span class="sxs-lookup"><span data-stu-id="1d1d4-107">Methods</span></span>
|<span data-ttu-id="1d1d4-108">方法</span><span class="sxs-lookup"><span data-stu-id="1d1d4-108">Method</span></span>|<span data-ttu-id="1d1d4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1d1d4-109">Return Type</span></span>|<span data-ttu-id="1d1d4-110">说明</span><span class="sxs-lookup"><span data-stu-id="1d1d4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1d1d4-111">列出 embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="1d1d4-111">List embeddedSIMActivationCodePoolAssignments</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|<span data-ttu-id="1d1d4-112">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1d1d4-112">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="1d1d4-113">列出[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1d1d4-113">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>|
|[<span data-ttu-id="1d1d4-114">获取 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="1d1d4-114">Get embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[<span data-ttu-id="1d1d4-115">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="1d1d4-115">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="1d1d4-116">读取[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1d1d4-116">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="1d1d4-117">创建 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="1d1d4-117">Create embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[<span data-ttu-id="1d1d4-118">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="1d1d4-118">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="1d1d4-119">创建新的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1d1d4-119">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="1d1d4-120">删除 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="1d1d4-120">Delete embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|<span data-ttu-id="1d1d4-121">无</span><span class="sxs-lookup"><span data-stu-id="1d1d4-121">None</span></span>|<span data-ttu-id="1d1d4-122">删除[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="1d1d4-122">Deletes a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>|
|[<span data-ttu-id="1d1d4-123">更新 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="1d1d4-123">Update embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[<span data-ttu-id="1d1d4-124">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="1d1d4-124">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="1d1d4-125">更新[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1d1d4-125">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1d1d4-126">属性</span><span class="sxs-lookup"><span data-stu-id="1d1d4-126">Properties</span></span>
|<span data-ttu-id="1d1d4-127">属性</span><span class="sxs-lookup"><span data-stu-id="1d1d4-127">Property</span></span>|<span data-ttu-id="1d1d4-128">类型</span><span class="sxs-lookup"><span data-stu-id="1d1d4-128">Type</span></span>|<span data-ttu-id="1d1d4-129">说明</span><span class="sxs-lookup"><span data-stu-id="1d1d4-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d1d4-130">id</span><span class="sxs-lookup"><span data-stu-id="1d1d4-130">id</span></span>|<span data-ttu-id="1d1d4-131">String</span><span class="sxs-lookup"><span data-stu-id="1d1d4-131">String</span></span>|<span data-ttu-id="1d1d4-132">嵌入的 SIM 激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1d1d4-132">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="1d1d4-133">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="1d1d4-133">System generated value assigned when created.</span></span>|
|<span data-ttu-id="1d1d4-134">target</span><span class="sxs-lookup"><span data-stu-id="1d1d4-134">target</span></span>|[<span data-ttu-id="1d1d4-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1d1d4-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1d1d4-136">嵌入的 SIM 激活代码池的目标组的类型。</span><span class="sxs-lookup"><span data-stu-id="1d1d4-136">The type of groups targeted by the embedded SIM activation code pool.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d1d4-137">关系</span><span class="sxs-lookup"><span data-stu-id="1d1d4-137">Relationships</span></span>
<span data-ttu-id="1d1d4-138">无</span><span class="sxs-lookup"><span data-stu-id="1d1d4-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d1d4-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d1d4-139">JSON Representation</span></span>
<span data-ttu-id="1d1d4-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d1d4-140">Here is a JSON representation of the resource.</span></span>
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





