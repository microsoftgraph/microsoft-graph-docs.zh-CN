---
title: deviceManagementScriptGroupAssignment 资源类型
description: 包含用于分配给组的设备管理脚本的属性。
author: tfitzmac
ms.openlocfilehash: 446e293ee3d4c0cc2071f6a93e01bcdf8cf72a2c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345939"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a><span data-ttu-id="416b6-103">deviceManagementScriptGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="416b6-103">deviceManagementScriptGroupAssignment resource type</span></span>

> <span data-ttu-id="416b6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="416b6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="416b6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="416b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="416b6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="416b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="416b6-107">包含用于分配给组的设备管理脚本的属性。</span><span class="sxs-lookup"><span data-stu-id="416b6-107">Contains properties used to assign a device management script to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="416b6-108">方法</span><span class="sxs-lookup"><span data-stu-id="416b6-108">Methods</span></span>
|<span data-ttu-id="416b6-109">方法</span><span class="sxs-lookup"><span data-stu-id="416b6-109">Method</span></span>|<span data-ttu-id="416b6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="416b6-110">Return Type</span></span>|<span data-ttu-id="416b6-111">说明</span><span class="sxs-lookup"><span data-stu-id="416b6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="416b6-112">列表 deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="416b6-112">List deviceManagementScriptGroupAssignments</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|<span data-ttu-id="416b6-113">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="416b6-113">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="416b6-114">列出属性和[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="416b6-114">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="416b6-115">获取 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="416b6-115">Get deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[<span data-ttu-id="416b6-116">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="416b6-116">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="416b6-117">读取属性和[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="416b6-117">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="416b6-118">创建 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="416b6-118">Create deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[<span data-ttu-id="416b6-119">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="416b6-119">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="416b6-120">创建新的[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="416b6-120">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="416b6-121">删除 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="416b6-121">Delete deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|<span data-ttu-id="416b6-122">无</span><span class="sxs-lookup"><span data-stu-id="416b6-122">None</span></span>|<span data-ttu-id="416b6-123">删除[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="416b6-123">Deletes a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>|
|[<span data-ttu-id="416b6-124">更新 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="416b6-124">Update deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[<span data-ttu-id="416b6-125">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="416b6-125">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="416b6-126">更新[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="416b6-126">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="416b6-127">属性</span><span class="sxs-lookup"><span data-stu-id="416b6-127">Properties</span></span>
|<span data-ttu-id="416b6-128">属性</span><span class="sxs-lookup"><span data-stu-id="416b6-128">Property</span></span>|<span data-ttu-id="416b6-129">类型</span><span class="sxs-lookup"><span data-stu-id="416b6-129">Type</span></span>|<span data-ttu-id="416b6-130">说明</span><span class="sxs-lookup"><span data-stu-id="416b6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="416b6-131">id</span><span class="sxs-lookup"><span data-stu-id="416b6-131">id</span></span>|<span data-ttu-id="416b6-132">字符串</span><span class="sxs-lookup"><span data-stu-id="416b6-132">String</span></span>|<span data-ttu-id="416b6-133">设备管理脚本组工作分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="416b6-133">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="416b6-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="416b6-134">targetGroupId</span></span>|<span data-ttu-id="416b6-135">字符串</span><span class="sxs-lookup"><span data-stu-id="416b6-135">String</span></span>|<span data-ttu-id="416b6-136">Azure Active Directory 组的 Id 目标脚本。</span><span class="sxs-lookup"><span data-stu-id="416b6-136">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="416b6-137">Relationships</span><span class="sxs-lookup"><span data-stu-id="416b6-137">Relationships</span></span>
<span data-ttu-id="416b6-138">无</span><span class="sxs-lookup"><span data-stu-id="416b6-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="416b6-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="416b6-139">JSON Representation</span></span>
<span data-ttu-id="416b6-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="416b6-140">Here is a JSON representation of the resource.</span></span>
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





