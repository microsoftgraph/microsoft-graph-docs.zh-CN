---
title: deviceManagementScriptGroupAssignment 资源类型
description: 包含用于分配给组的设备管理脚本的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6dfeca71b20ffae27f99fdd4af0909332338b4f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832205"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a><span data-ttu-id="9e0d5-103">deviceManagementScriptGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e0d5-103">deviceManagementScriptGroupAssignment resource type</span></span>

> <span data-ttu-id="9e0d5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9e0d5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e0d5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9e0d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e0d5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9e0d5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e0d5-107">包含用于分配给组的设备管理脚本的属性。</span><span class="sxs-lookup"><span data-stu-id="9e0d5-107">Contains properties used to assign a device management script to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="9e0d5-108">方法</span><span class="sxs-lookup"><span data-stu-id="9e0d5-108">Methods</span></span>
|<span data-ttu-id="9e0d5-109">方法</span><span class="sxs-lookup"><span data-stu-id="9e0d5-109">Method</span></span>|<span data-ttu-id="9e0d5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9e0d5-110">Return Type</span></span>|<span data-ttu-id="9e0d5-111">说明</span><span class="sxs-lookup"><span data-stu-id="9e0d5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9e0d5-112">列表 deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="9e0d5-112">List deviceManagementScriptGroupAssignments</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|<span data-ttu-id="9e0d5-113">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="9e0d5-113">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="9e0d5-114">列出属性和[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="9e0d5-114">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="9e0d5-115">获取 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="9e0d5-115">Get deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[<span data-ttu-id="9e0d5-116">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="9e0d5-116">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="9e0d5-117">读取属性和[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="9e0d5-117">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="9e0d5-118">创建 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="9e0d5-118">Create deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[<span data-ttu-id="9e0d5-119">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="9e0d5-119">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="9e0d5-120">创建新的[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9e0d5-120">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="9e0d5-121">删除 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="9e0d5-121">Delete deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|<span data-ttu-id="9e0d5-122">无</span><span class="sxs-lookup"><span data-stu-id="9e0d5-122">None</span></span>|<span data-ttu-id="9e0d5-123">删除[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="9e0d5-123">Deletes a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>|
|[<span data-ttu-id="9e0d5-124">更新 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="9e0d5-124">Update deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[<span data-ttu-id="9e0d5-125">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="9e0d5-125">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="9e0d5-126">更新[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9e0d5-126">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9e0d5-127">属性</span><span class="sxs-lookup"><span data-stu-id="9e0d5-127">Properties</span></span>
|<span data-ttu-id="9e0d5-128">属性</span><span class="sxs-lookup"><span data-stu-id="9e0d5-128">Property</span></span>|<span data-ttu-id="9e0d5-129">类型</span><span class="sxs-lookup"><span data-stu-id="9e0d5-129">Type</span></span>|<span data-ttu-id="9e0d5-130">说明</span><span class="sxs-lookup"><span data-stu-id="9e0d5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e0d5-131">id</span><span class="sxs-lookup"><span data-stu-id="9e0d5-131">id</span></span>|<span data-ttu-id="9e0d5-132">字符串</span><span class="sxs-lookup"><span data-stu-id="9e0d5-132">String</span></span>|<span data-ttu-id="9e0d5-133">设备管理脚本组工作分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="9e0d5-133">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="9e0d5-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="9e0d5-134">targetGroupId</span></span>|<span data-ttu-id="9e0d5-135">字符串</span><span class="sxs-lookup"><span data-stu-id="9e0d5-135">String</span></span>|<span data-ttu-id="9e0d5-136">Azure Active Directory 组的 Id 目标脚本。</span><span class="sxs-lookup"><span data-stu-id="9e0d5-136">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e0d5-137">Relationships</span><span class="sxs-lookup"><span data-stu-id="9e0d5-137">Relationships</span></span>
<span data-ttu-id="9e0d5-138">无</span><span class="sxs-lookup"><span data-stu-id="9e0d5-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e0d5-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e0d5-139">JSON Representation</span></span>
<span data-ttu-id="9e0d5-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e0d5-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```





