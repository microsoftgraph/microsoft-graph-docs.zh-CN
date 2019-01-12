---
title: embeddedSIMActivationCodePoolAssignment 资源类型
description: 嵌入的 SIM 激活代码池工作分配实体将特定 embeddedSIMActivationCodePool 分配给 AAD 设备组。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5178e794f4843975dde0f05d019b4233611764fb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967096"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a><span data-ttu-id="26c1d-103">embeddedSIMActivationCodePoolAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="26c1d-103">embeddedSIMActivationCodePoolAssignment resource type</span></span>

> <span data-ttu-id="26c1d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="26c1d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26c1d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="26c1d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26c1d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="26c1d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26c1d-107">嵌入的 SIM 激活代码池工作分配实体将特定 embeddedSIMActivationCodePool 分配给 AAD 设备组。</span><span class="sxs-lookup"><span data-stu-id="26c1d-107">The embedded SIM activation code pool assignment entity assigns a specific embeddedSIMActivationCodePool to an AAD device group.</span></span>
## <a name="methods"></a><span data-ttu-id="26c1d-108">方法</span><span class="sxs-lookup"><span data-stu-id="26c1d-108">Methods</span></span>
|<span data-ttu-id="26c1d-109">方法</span><span class="sxs-lookup"><span data-stu-id="26c1d-109">Method</span></span>|<span data-ttu-id="26c1d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="26c1d-110">Return Type</span></span>|<span data-ttu-id="26c1d-111">说明</span><span class="sxs-lookup"><span data-stu-id="26c1d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="26c1d-112">列表 embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="26c1d-112">List embeddedSIMActivationCodePoolAssignments</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|<span data-ttu-id="26c1d-113">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="26c1d-113">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="26c1d-114">列出属性和[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="26c1d-114">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>|
|[<span data-ttu-id="26c1d-115">获取 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="26c1d-115">Get embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[<span data-ttu-id="26c1d-116">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="26c1d-116">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="26c1d-117">读取属性和[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="26c1d-117">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="26c1d-118">创建 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="26c1d-118">Create embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[<span data-ttu-id="26c1d-119">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="26c1d-119">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="26c1d-120">创建新的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26c1d-120">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="26c1d-121">删除 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="26c1d-121">Delete embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|<span data-ttu-id="26c1d-122">无</span><span class="sxs-lookup"><span data-stu-id="26c1d-122">None</span></span>|<span data-ttu-id="26c1d-123">删除[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="26c1d-123">Deletes a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>|
|[<span data-ttu-id="26c1d-124">更新 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="26c1d-124">Update embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[<span data-ttu-id="26c1d-125">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="26c1d-125">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="26c1d-126">更新[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="26c1d-126">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="26c1d-127">属性</span><span class="sxs-lookup"><span data-stu-id="26c1d-127">Properties</span></span>
|<span data-ttu-id="26c1d-128">属性</span><span class="sxs-lookup"><span data-stu-id="26c1d-128">Property</span></span>|<span data-ttu-id="26c1d-129">类型</span><span class="sxs-lookup"><span data-stu-id="26c1d-129">Type</span></span>|<span data-ttu-id="26c1d-130">说明</span><span class="sxs-lookup"><span data-stu-id="26c1d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26c1d-131">id</span><span class="sxs-lookup"><span data-stu-id="26c1d-131">id</span></span>|<span data-ttu-id="26c1d-132">字符串</span><span class="sxs-lookup"><span data-stu-id="26c1d-132">String</span></span>|<span data-ttu-id="26c1d-133">嵌入 SIM 激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="26c1d-133">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="26c1d-134">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="26c1d-134">System generated value assigned when created.</span></span>|
|<span data-ttu-id="26c1d-135">target</span><span class="sxs-lookup"><span data-stu-id="26c1d-135">target</span></span>|[<span data-ttu-id="26c1d-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="26c1d-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="26c1d-137">目标嵌入 SIM 激活代码池的组的类型。</span><span class="sxs-lookup"><span data-stu-id="26c1d-137">The type of groups targeted by the embedded SIM activation code pool.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26c1d-138">Relationships</span><span class="sxs-lookup"><span data-stu-id="26c1d-138">Relationships</span></span>
<span data-ttu-id="26c1d-139">无</span><span class="sxs-lookup"><span data-stu-id="26c1d-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="26c1d-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26c1d-140">JSON Representation</span></span>
<span data-ttu-id="26c1d-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26c1d-141">Here is a JSON representation of the resource.</span></span>
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





