---
title: deviceCompliancePolicyAssignment 资源类型
description: 设备符合性策略分配。
ms.openlocfilehash: 1e553553e81a3d3d68f0766754d770c3f3f24d7f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047505"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="7b9be-103">deviceCompliancePolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b9be-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="7b9be-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7b9be-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b9be-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7b9be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b9be-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7b9be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b9be-107">设备符合性策略分配。</span><span class="sxs-lookup"><span data-stu-id="7b9be-107">Device compliance policy assignment.</span></span>
## <a name="methods"></a><span data-ttu-id="7b9be-108">方法</span><span class="sxs-lookup"><span data-stu-id="7b9be-108">Methods</span></span>
|<span data-ttu-id="7b9be-109">方法</span><span class="sxs-lookup"><span data-stu-id="7b9be-109">Method</span></span>|<span data-ttu-id="7b9be-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7b9be-110">Return Type</span></span>|<span data-ttu-id="7b9be-111">说明</span><span class="sxs-lookup"><span data-stu-id="7b9be-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7b9be-112">列出 deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="7b9be-112">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="7b9be-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b9be-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="7b9be-114">列出 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7b9be-114">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="7b9be-115">获取 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="7b9be-115">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="7b9be-116">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="7b9be-116">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="7b9be-117">读取 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7b9be-117">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="7b9be-118">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="7b9be-118">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="7b9be-119">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="7b9be-119">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="7b9be-120">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b9be-120">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="7b9be-121">删除 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="7b9be-121">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="7b9be-122">无</span><span class="sxs-lookup"><span data-stu-id="7b9be-122">None</span></span>|<span data-ttu-id="7b9be-123">删除 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="7b9be-123">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="7b9be-124">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="7b9be-124">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="7b9be-125">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="7b9be-125">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="7b9be-126">更新 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7b9be-126">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b9be-127">属性</span><span class="sxs-lookup"><span data-stu-id="7b9be-127">Properties</span></span>
|<span data-ttu-id="7b9be-128">属性</span><span class="sxs-lookup"><span data-stu-id="7b9be-128">Property</span></span>|<span data-ttu-id="7b9be-129">类型</span><span class="sxs-lookup"><span data-stu-id="7b9be-129">Type</span></span>|<span data-ttu-id="7b9be-130">说明</span><span class="sxs-lookup"><span data-stu-id="7b9be-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b9be-131">id</span><span class="sxs-lookup"><span data-stu-id="7b9be-131">id</span></span>|<span data-ttu-id="7b9be-132">String</span><span class="sxs-lookup"><span data-stu-id="7b9be-132">String</span></span>|<span data-ttu-id="7b9be-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7b9be-133">Key of the entity.</span></span>|
|<span data-ttu-id="7b9be-134">target</span><span class="sxs-lookup"><span data-stu-id="7b9be-134">target</span></span>|[<span data-ttu-id="7b9be-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7b9be-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7b9be-136">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="7b9be-136">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b9be-137">关系</span><span class="sxs-lookup"><span data-stu-id="7b9be-137">Relationships</span></span>
<span data-ttu-id="7b9be-138">无</span><span class="sxs-lookup"><span data-stu-id="7b9be-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7b9be-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b9be-139">JSON Representation</span></span>
<span data-ttu-id="7b9be-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b9be-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





