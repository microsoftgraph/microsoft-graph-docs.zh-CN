---
title: deviceManagementScriptGroupAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 00b3650cefa15f0a8e7fb070b5786ff0e5104156
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43374997"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a><span data-ttu-id="254e8-103">deviceManagementScriptGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="254e8-103">deviceManagementScriptGroupAssignment resource type</span></span>

<span data-ttu-id="254e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="254e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="254e8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="254e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="254e8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="254e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="254e8-107">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="254e8-107">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="254e8-108">方法</span><span class="sxs-lookup"><span data-stu-id="254e8-108">Methods</span></span>
|<span data-ttu-id="254e8-109">方法</span><span class="sxs-lookup"><span data-stu-id="254e8-109">Method</span></span>|<span data-ttu-id="254e8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="254e8-110">Return Type</span></span>|<span data-ttu-id="254e8-111">说明</span><span class="sxs-lookup"><span data-stu-id="254e8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="254e8-112">列出 deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="254e8-112">List deviceManagementScriptGroupAssignments</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|<span data-ttu-id="254e8-113">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="254e8-113">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="254e8-114">列出[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="254e8-114">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="254e8-115">获取 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="254e8-115">Get deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[<span data-ttu-id="254e8-116">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="254e8-116">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="254e8-117">读取[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="254e8-117">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="254e8-118">创建 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="254e8-118">Create deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[<span data-ttu-id="254e8-119">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="254e8-119">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="254e8-120">创建新的[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="254e8-120">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="254e8-121">删除 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="254e8-121">Delete deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|<span data-ttu-id="254e8-122">无</span><span class="sxs-lookup"><span data-stu-id="254e8-122">None</span></span>|<span data-ttu-id="254e8-123">删除[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="254e8-123">Deletes a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>|
|[<span data-ttu-id="254e8-124">更新 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="254e8-124">Update deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[<span data-ttu-id="254e8-125">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="254e8-125">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="254e8-126">更新[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="254e8-126">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="254e8-127">属性</span><span class="sxs-lookup"><span data-stu-id="254e8-127">Properties</span></span>
|<span data-ttu-id="254e8-128">属性</span><span class="sxs-lookup"><span data-stu-id="254e8-128">Property</span></span>|<span data-ttu-id="254e8-129">类型</span><span class="sxs-lookup"><span data-stu-id="254e8-129">Type</span></span>|<span data-ttu-id="254e8-130">说明</span><span class="sxs-lookup"><span data-stu-id="254e8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="254e8-131">id</span><span class="sxs-lookup"><span data-stu-id="254e8-131">id</span></span>|<span data-ttu-id="254e8-132">字符串</span><span class="sxs-lookup"><span data-stu-id="254e8-132">String</span></span>|<span data-ttu-id="254e8-133">Device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="254e8-133">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="254e8-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="254e8-134">This property is read-only.</span></span>|
|<span data-ttu-id="254e8-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="254e8-135">targetGroupId</span></span>|<span data-ttu-id="254e8-136">字符串</span><span class="sxs-lookup"><span data-stu-id="254e8-136">String</span></span>|<span data-ttu-id="254e8-137">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="254e8-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="254e8-138">关系</span><span class="sxs-lookup"><span data-stu-id="254e8-138">Relationships</span></span>
<span data-ttu-id="254e8-139">无</span><span class="sxs-lookup"><span data-stu-id="254e8-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="254e8-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="254e8-140">JSON Representation</span></span>
<span data-ttu-id="254e8-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="254e8-141">Here is a JSON representation of the resource.</span></span>
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



