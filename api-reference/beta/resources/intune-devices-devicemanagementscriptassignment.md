---
title: deviceManagementScriptAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3cfcc04631f3917c013507b849dfdaa5a7569893
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43375027"
---
# <a name="devicemanagementscriptassignment-resource-type"></a><span data-ttu-id="10b30-103">deviceManagementScriptAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="10b30-103">deviceManagementScriptAssignment resource type</span></span>

<span data-ttu-id="10b30-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10b30-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10b30-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="10b30-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10b30-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10b30-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10b30-107">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="10b30-107">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="10b30-108">方法</span><span class="sxs-lookup"><span data-stu-id="10b30-108">Methods</span></span>
|<span data-ttu-id="10b30-109">方法</span><span class="sxs-lookup"><span data-stu-id="10b30-109">Method</span></span>|<span data-ttu-id="10b30-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="10b30-110">Return Type</span></span>|<span data-ttu-id="10b30-111">说明</span><span class="sxs-lookup"><span data-stu-id="10b30-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="10b30-112">列出 deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="10b30-112">List deviceManagementScriptAssignments</span></span>](../api/intune-devices-devicemanagementscriptassignment-list.md)|<span data-ttu-id="10b30-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="10b30-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="10b30-114">列出[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10b30-114">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="10b30-115">获取 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="10b30-115">Get deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-get.md)|[<span data-ttu-id="10b30-116">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="10b30-116">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="10b30-117">读取[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10b30-117">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="10b30-118">创建 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="10b30-118">Create deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-create.md)|[<span data-ttu-id="10b30-119">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="10b30-119">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="10b30-120">创建新的[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="10b30-120">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="10b30-121">删除 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="10b30-121">Delete deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-delete.md)|<span data-ttu-id="10b30-122">无</span><span class="sxs-lookup"><span data-stu-id="10b30-122">None</span></span>|<span data-ttu-id="10b30-123">删除[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="10b30-123">Deletes a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>|
|[<span data-ttu-id="10b30-124">更新 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="10b30-124">Update deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-update.md)|[<span data-ttu-id="10b30-125">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="10b30-125">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="10b30-126">更新[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="10b30-126">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10b30-127">属性</span><span class="sxs-lookup"><span data-stu-id="10b30-127">Properties</span></span>
|<span data-ttu-id="10b30-128">属性</span><span class="sxs-lookup"><span data-stu-id="10b30-128">Property</span></span>|<span data-ttu-id="10b30-129">类型</span><span class="sxs-lookup"><span data-stu-id="10b30-129">Type</span></span>|<span data-ttu-id="10b30-130">说明</span><span class="sxs-lookup"><span data-stu-id="10b30-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10b30-131">id</span><span class="sxs-lookup"><span data-stu-id="10b30-131">id</span></span>|<span data-ttu-id="10b30-132">字符串</span><span class="sxs-lookup"><span data-stu-id="10b30-132">String</span></span>|<span data-ttu-id="10b30-133">Device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="10b30-133">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="10b30-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="10b30-134">This property is read-only.</span></span>|
|<span data-ttu-id="10b30-135">target</span><span class="sxs-lookup"><span data-stu-id="10b30-135">target</span></span>|[<span data-ttu-id="10b30-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="10b30-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="10b30-137">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="10b30-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10b30-138">关系</span><span class="sxs-lookup"><span data-stu-id="10b30-138">Relationships</span></span>
<span data-ttu-id="10b30-139">无</span><span class="sxs-lookup"><span data-stu-id="10b30-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10b30-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10b30-140">JSON Representation</span></span>
<span data-ttu-id="10b30-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10b30-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



