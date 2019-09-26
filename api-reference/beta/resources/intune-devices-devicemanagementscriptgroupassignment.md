---
title: deviceManagementScriptGroupAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aabd0ae86be9d423cc209f0ac932f975efcb45ce
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196999"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a><span data-ttu-id="aee2c-103">deviceManagementScriptGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="aee2c-103">deviceManagementScriptGroupAssignment resource type</span></span>

> <span data-ttu-id="aee2c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aee2c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aee2c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aee2c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aee2c-106">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="aee2c-106">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="aee2c-107">方法</span><span class="sxs-lookup"><span data-stu-id="aee2c-107">Methods</span></span>
|<span data-ttu-id="aee2c-108">方法</span><span class="sxs-lookup"><span data-stu-id="aee2c-108">Method</span></span>|<span data-ttu-id="aee2c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="aee2c-109">Return Type</span></span>|<span data-ttu-id="aee2c-110">说明</span><span class="sxs-lookup"><span data-stu-id="aee2c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aee2c-111">列出 deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="aee2c-111">List deviceManagementScriptGroupAssignments</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|<span data-ttu-id="aee2c-112">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="aee2c-112">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="aee2c-113">列出[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aee2c-113">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="aee2c-114">获取 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="aee2c-114">Get deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[<span data-ttu-id="aee2c-115">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="aee2c-115">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="aee2c-116">读取[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aee2c-116">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="aee2c-117">创建 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="aee2c-117">Create deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[<span data-ttu-id="aee2c-118">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="aee2c-118">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="aee2c-119">创建新的[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aee2c-119">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="aee2c-120">删除 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="aee2c-120">Delete deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|<span data-ttu-id="aee2c-121">无</span><span class="sxs-lookup"><span data-stu-id="aee2c-121">None</span></span>|<span data-ttu-id="aee2c-122">删除[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="aee2c-122">Deletes a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>|
|[<span data-ttu-id="aee2c-123">更新 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="aee2c-123">Update deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[<span data-ttu-id="aee2c-124">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="aee2c-124">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="aee2c-125">更新[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aee2c-125">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aee2c-126">属性</span><span class="sxs-lookup"><span data-stu-id="aee2c-126">Properties</span></span>
|<span data-ttu-id="aee2c-127">属性</span><span class="sxs-lookup"><span data-stu-id="aee2c-127">Property</span></span>|<span data-ttu-id="aee2c-128">类型</span><span class="sxs-lookup"><span data-stu-id="aee2c-128">Type</span></span>|<span data-ttu-id="aee2c-129">说明</span><span class="sxs-lookup"><span data-stu-id="aee2c-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aee2c-130">id</span><span class="sxs-lookup"><span data-stu-id="aee2c-130">id</span></span>|<span data-ttu-id="aee2c-131">String</span><span class="sxs-lookup"><span data-stu-id="aee2c-131">String</span></span>|<span data-ttu-id="aee2c-132">Device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="aee2c-132">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="aee2c-133">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="aee2c-133">This property is read-only.</span></span>|
|<span data-ttu-id="aee2c-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="aee2c-134">targetGroupId</span></span>|<span data-ttu-id="aee2c-135">String</span><span class="sxs-lookup"><span data-stu-id="aee2c-135">String</span></span>|<span data-ttu-id="aee2c-136">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="aee2c-136">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aee2c-137">关系</span><span class="sxs-lookup"><span data-stu-id="aee2c-137">Relationships</span></span>
<span data-ttu-id="aee2c-138">无</span><span class="sxs-lookup"><span data-stu-id="aee2c-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aee2c-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aee2c-139">JSON Representation</span></span>
<span data-ttu-id="aee2c-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aee2c-140">Here is a JSON representation of the resource.</span></span>
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



