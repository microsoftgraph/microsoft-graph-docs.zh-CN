---
title: embeddedSIMActivationCodePoolAssignment 资源类型
description: 嵌入的 SIM 激活代码池分配实体可将特定的 embeddedSIMActivationCodePool 分配给 AAD 设备组。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5ec64384bd5620b74f9cdca2148e6b3064e9c98
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571133"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a><span data-ttu-id="efe3e-103">embeddedSIMActivationCodePoolAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="efe3e-103">embeddedSIMActivationCodePoolAssignment resource type</span></span>

> <span data-ttu-id="efe3e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="efe3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efe3e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="efe3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efe3e-106">嵌入的 SIM 激活代码池分配实体可将特定的 embeddedSIMActivationCodePool 分配给 AAD 设备组。</span><span class="sxs-lookup"><span data-stu-id="efe3e-106">The embedded SIM activation code pool assignment entity assigns a specific embeddedSIMActivationCodePool to an AAD device group.</span></span>

## <a name="methods"></a><span data-ttu-id="efe3e-107">方法</span><span class="sxs-lookup"><span data-stu-id="efe3e-107">Methods</span></span>
|<span data-ttu-id="efe3e-108">方法</span><span class="sxs-lookup"><span data-stu-id="efe3e-108">Method</span></span>|<span data-ttu-id="efe3e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="efe3e-109">Return Type</span></span>|<span data-ttu-id="efe3e-110">说明</span><span class="sxs-lookup"><span data-stu-id="efe3e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="efe3e-111">列出 embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="efe3e-111">List embeddedSIMActivationCodePoolAssignments</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|<span data-ttu-id="efe3e-112">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="efe3e-112">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="efe3e-113">列出[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="efe3e-113">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>|
|[<span data-ttu-id="efe3e-114">获取 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="efe3e-114">Get embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[<span data-ttu-id="efe3e-115">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="efe3e-115">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="efe3e-116">读取[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="efe3e-116">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="efe3e-117">创建 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="efe3e-117">Create embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[<span data-ttu-id="efe3e-118">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="efe3e-118">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="efe3e-119">创建新的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="efe3e-119">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="efe3e-120">删除 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="efe3e-120">Delete embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|<span data-ttu-id="efe3e-121">无</span><span class="sxs-lookup"><span data-stu-id="efe3e-121">None</span></span>|<span data-ttu-id="efe3e-122">删除[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="efe3e-122">Deletes a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>|
|[<span data-ttu-id="efe3e-123">更新 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="efe3e-123">Update embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[<span data-ttu-id="efe3e-124">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="efe3e-124">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="efe3e-125">更新[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="efe3e-125">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="efe3e-126">属性</span><span class="sxs-lookup"><span data-stu-id="efe3e-126">Properties</span></span>
|<span data-ttu-id="efe3e-127">属性</span><span class="sxs-lookup"><span data-stu-id="efe3e-127">Property</span></span>|<span data-ttu-id="efe3e-128">类型</span><span class="sxs-lookup"><span data-stu-id="efe3e-128">Type</span></span>|<span data-ttu-id="efe3e-129">说明</span><span class="sxs-lookup"><span data-stu-id="efe3e-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efe3e-130">id</span><span class="sxs-lookup"><span data-stu-id="efe3e-130">id</span></span>|<span data-ttu-id="efe3e-131">String</span><span class="sxs-lookup"><span data-stu-id="efe3e-131">String</span></span>|<span data-ttu-id="efe3e-132">嵌入的 SIM 激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="efe3e-132">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="efe3e-133">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="efe3e-133">System generated value assigned when created.</span></span>|
|<span data-ttu-id="efe3e-134">target</span><span class="sxs-lookup"><span data-stu-id="efe3e-134">target</span></span>|[<span data-ttu-id="efe3e-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="efe3e-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="efe3e-136">嵌入的 SIM 激活代码池的目标组的类型。</span><span class="sxs-lookup"><span data-stu-id="efe3e-136">The type of groups targeted by the embedded SIM activation code pool.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efe3e-137">关系</span><span class="sxs-lookup"><span data-stu-id="efe3e-137">Relationships</span></span>
<span data-ttu-id="efe3e-138">无</span><span class="sxs-lookup"><span data-stu-id="efe3e-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efe3e-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="efe3e-139">JSON Representation</span></span>
<span data-ttu-id="efe3e-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efe3e-140">Here is a JSON representation of the resource.</span></span>
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





