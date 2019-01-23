---
title: embeddedSIMActivationCodePoolAssignment 资源类型
description: 嵌入的 SIM 激活代码池工作分配实体将特定 embeddedSIMActivationCodePool 分配给 AAD 设备组。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ed8918adb99e301717ed7d53e54bb3ff1ac29ba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423837"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a><span data-ttu-id="70dcf-103">embeddedSIMActivationCodePoolAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="70dcf-103">embeddedSIMActivationCodePoolAssignment resource type</span></span>

> <span data-ttu-id="70dcf-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="70dcf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="70dcf-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="70dcf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70dcf-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="70dcf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70dcf-107">嵌入的 SIM 激活代码池工作分配实体将特定 embeddedSIMActivationCodePool 分配给 AAD 设备组。</span><span class="sxs-lookup"><span data-stu-id="70dcf-107">The embedded SIM activation code pool assignment entity assigns a specific embeddedSIMActivationCodePool to an AAD device group.</span></span>

## <a name="methods"></a><span data-ttu-id="70dcf-108">方法</span><span class="sxs-lookup"><span data-stu-id="70dcf-108">Methods</span></span>
|<span data-ttu-id="70dcf-109">方法</span><span class="sxs-lookup"><span data-stu-id="70dcf-109">Method</span></span>|<span data-ttu-id="70dcf-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="70dcf-110">Return Type</span></span>|<span data-ttu-id="70dcf-111">说明</span><span class="sxs-lookup"><span data-stu-id="70dcf-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="70dcf-112">列表 embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="70dcf-112">List embeddedSIMActivationCodePoolAssignments</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|<span data-ttu-id="70dcf-113">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="70dcf-113">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="70dcf-114">列出属性和[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="70dcf-114">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>|
|[<span data-ttu-id="70dcf-115">获取 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="70dcf-115">Get embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[<span data-ttu-id="70dcf-116">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="70dcf-116">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="70dcf-117">读取属性和[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="70dcf-117">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="70dcf-118">创建 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="70dcf-118">Create embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[<span data-ttu-id="70dcf-119">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="70dcf-119">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="70dcf-120">创建新的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="70dcf-120">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="70dcf-121">删除 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="70dcf-121">Delete embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|<span data-ttu-id="70dcf-122">无</span><span class="sxs-lookup"><span data-stu-id="70dcf-122">None</span></span>|<span data-ttu-id="70dcf-123">删除[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="70dcf-123">Deletes a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>|
|[<span data-ttu-id="70dcf-124">更新 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="70dcf-124">Update embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[<span data-ttu-id="70dcf-125">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="70dcf-125">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="70dcf-126">更新[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="70dcf-126">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="70dcf-127">属性</span><span class="sxs-lookup"><span data-stu-id="70dcf-127">Properties</span></span>
|<span data-ttu-id="70dcf-128">属性</span><span class="sxs-lookup"><span data-stu-id="70dcf-128">Property</span></span>|<span data-ttu-id="70dcf-129">类型</span><span class="sxs-lookup"><span data-stu-id="70dcf-129">Type</span></span>|<span data-ttu-id="70dcf-130">说明</span><span class="sxs-lookup"><span data-stu-id="70dcf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70dcf-131">id</span><span class="sxs-lookup"><span data-stu-id="70dcf-131">id</span></span>|<span data-ttu-id="70dcf-132">String</span><span class="sxs-lookup"><span data-stu-id="70dcf-132">String</span></span>|<span data-ttu-id="70dcf-133">嵌入 SIM 激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="70dcf-133">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="70dcf-134">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="70dcf-134">System generated value assigned when created.</span></span>|
|<span data-ttu-id="70dcf-135">target</span><span class="sxs-lookup"><span data-stu-id="70dcf-135">target</span></span>|[<span data-ttu-id="70dcf-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="70dcf-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="70dcf-137">目标嵌入 SIM 激活代码池的组的类型。</span><span class="sxs-lookup"><span data-stu-id="70dcf-137">The type of groups targeted by the embedded SIM activation code pool.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70dcf-138">关系</span><span class="sxs-lookup"><span data-stu-id="70dcf-138">Relationships</span></span>
<span data-ttu-id="70dcf-139">无</span><span class="sxs-lookup"><span data-stu-id="70dcf-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="70dcf-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70dcf-140">JSON Representation</span></span>
<span data-ttu-id="70dcf-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70dcf-141">Here is a JSON representation of the resource.</span></span>
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




