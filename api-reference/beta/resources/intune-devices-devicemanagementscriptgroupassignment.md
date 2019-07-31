---
title: deviceManagementScriptGroupAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cc5b440fbdf5ca0f6ebb7ef28fbf3e4ce868af63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968447"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a><span data-ttu-id="fe352-103">deviceManagementScriptGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe352-103">deviceManagementScriptGroupAssignment resource type</span></span>

> <span data-ttu-id="fe352-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fe352-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe352-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe352-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe352-106">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="fe352-106">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="fe352-107">方法</span><span class="sxs-lookup"><span data-stu-id="fe352-107">Methods</span></span>
|<span data-ttu-id="fe352-108">方法</span><span class="sxs-lookup"><span data-stu-id="fe352-108">Method</span></span>|<span data-ttu-id="fe352-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="fe352-109">Return Type</span></span>|<span data-ttu-id="fe352-110">说明</span><span class="sxs-lookup"><span data-stu-id="fe352-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fe352-111">列出 deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="fe352-111">List deviceManagementScriptGroupAssignments</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|<span data-ttu-id="fe352-112">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="fe352-112">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="fe352-113">列出[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fe352-113">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="fe352-114">获取 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="fe352-114">Get deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[<span data-ttu-id="fe352-115">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="fe352-115">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="fe352-116">读取[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fe352-116">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="fe352-117">创建 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="fe352-117">Create deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[<span data-ttu-id="fe352-118">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="fe352-118">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="fe352-119">创建新的[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fe352-119">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="fe352-120">删除 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="fe352-120">Delete deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|<span data-ttu-id="fe352-121">无</span><span class="sxs-lookup"><span data-stu-id="fe352-121">None</span></span>|<span data-ttu-id="fe352-122">删除[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="fe352-122">Deletes a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>|
|[<span data-ttu-id="fe352-123">更新 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="fe352-123">Update deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[<span data-ttu-id="fe352-124">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="fe352-124">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="fe352-125">更新[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fe352-125">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fe352-126">属性</span><span class="sxs-lookup"><span data-stu-id="fe352-126">Properties</span></span>
|<span data-ttu-id="fe352-127">属性</span><span class="sxs-lookup"><span data-stu-id="fe352-127">Property</span></span>|<span data-ttu-id="fe352-128">类型</span><span class="sxs-lookup"><span data-stu-id="fe352-128">Type</span></span>|<span data-ttu-id="fe352-129">说明</span><span class="sxs-lookup"><span data-stu-id="fe352-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe352-130">id</span><span class="sxs-lookup"><span data-stu-id="fe352-130">id</span></span>|<span data-ttu-id="fe352-131">String</span><span class="sxs-lookup"><span data-stu-id="fe352-131">String</span></span>|<span data-ttu-id="fe352-132">Device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="fe352-132">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="fe352-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="fe352-133">targetGroupId</span></span>|<span data-ttu-id="fe352-134">String</span><span class="sxs-lookup"><span data-stu-id="fe352-134">String</span></span>|<span data-ttu-id="fe352-135">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="fe352-135">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe352-136">关系</span><span class="sxs-lookup"><span data-stu-id="fe352-136">Relationships</span></span>
<span data-ttu-id="fe352-137">无</span><span class="sxs-lookup"><span data-stu-id="fe352-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe352-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe352-138">JSON Representation</span></span>
<span data-ttu-id="fe352-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe352-139">Here is a JSON representation of the resource.</span></span>
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





