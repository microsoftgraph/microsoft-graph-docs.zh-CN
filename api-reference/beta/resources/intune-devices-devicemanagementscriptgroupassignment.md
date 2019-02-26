---
title: deviceManagementScriptGroupAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 27028d14289e3e0efdfa705d35d02d67d1fb1835
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154696"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a><span data-ttu-id="27020-103">deviceManagementScriptGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="27020-103">deviceManagementScriptGroupAssignment resource type</span></span>

> <span data-ttu-id="27020-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="27020-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27020-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27020-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27020-106">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="27020-106">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="27020-107">方法</span><span class="sxs-lookup"><span data-stu-id="27020-107">Methods</span></span>
|<span data-ttu-id="27020-108">方法</span><span class="sxs-lookup"><span data-stu-id="27020-108">Method</span></span>|<span data-ttu-id="27020-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="27020-109">Return Type</span></span>|<span data-ttu-id="27020-110">说明</span><span class="sxs-lookup"><span data-stu-id="27020-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="27020-111">列出 deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="27020-111">List deviceManagementScriptGroupAssignments</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|<span data-ttu-id="27020-112">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="27020-112">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="27020-113">列出[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="27020-113">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="27020-114">获取 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="27020-114">Get deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[<span data-ttu-id="27020-115">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="27020-115">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="27020-116">读取[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="27020-116">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="27020-117">创建 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="27020-117">Create deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[<span data-ttu-id="27020-118">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="27020-118">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="27020-119">创建新的[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="27020-119">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="27020-120">删除 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="27020-120">Delete deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|<span data-ttu-id="27020-121">无</span><span class="sxs-lookup"><span data-stu-id="27020-121">None</span></span>|<span data-ttu-id="27020-122">删除[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="27020-122">Deletes a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>|
|[<span data-ttu-id="27020-123">更新 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="27020-123">Update deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[<span data-ttu-id="27020-124">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="27020-124">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="27020-125">更新[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27020-125">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="27020-126">属性</span><span class="sxs-lookup"><span data-stu-id="27020-126">Properties</span></span>
|<span data-ttu-id="27020-127">属性</span><span class="sxs-lookup"><span data-stu-id="27020-127">Property</span></span>|<span data-ttu-id="27020-128">类型</span><span class="sxs-lookup"><span data-stu-id="27020-128">Type</span></span>|<span data-ttu-id="27020-129">说明</span><span class="sxs-lookup"><span data-stu-id="27020-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27020-130">id</span><span class="sxs-lookup"><span data-stu-id="27020-130">id</span></span>|<span data-ttu-id="27020-131">String</span><span class="sxs-lookup"><span data-stu-id="27020-131">String</span></span>|<span data-ttu-id="27020-132">device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="27020-132">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="27020-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="27020-133">targetGroupId</span></span>|<span data-ttu-id="27020-134">String</span><span class="sxs-lookup"><span data-stu-id="27020-134">String</span></span>|<span data-ttu-id="27020-135">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="27020-135">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27020-136">关系</span><span class="sxs-lookup"><span data-stu-id="27020-136">Relationships</span></span>
<span data-ttu-id="27020-137">无</span><span class="sxs-lookup"><span data-stu-id="27020-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27020-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27020-138">JSON Representation</span></span>
<span data-ttu-id="27020-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27020-139">Here is a JSON representation of the resource.</span></span>
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




