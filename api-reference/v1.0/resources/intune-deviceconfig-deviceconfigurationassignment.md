---
title: deviceConfigurationAssignment 资源类型
description: 设备配置分配实体将 AAD 组分配到特定设备配置。
author: tfitzmac
ms.openlocfilehash: 26afc67312ab8544b395b5e20b89a01558fc75d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306242"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="19395-103">deviceConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="19395-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="19395-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="19395-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19395-105">设备配置分配实体将 AAD 组分配到特定设备配置。</span><span class="sxs-lookup"><span data-stu-id="19395-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="19395-106">方法</span><span class="sxs-lookup"><span data-stu-id="19395-106">Methods</span></span>
|<span data-ttu-id="19395-107">方法</span><span class="sxs-lookup"><span data-stu-id="19395-107">Method</span></span>|<span data-ttu-id="19395-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="19395-108">Return Type</span></span>|<span data-ttu-id="19395-109">说明</span><span class="sxs-lookup"><span data-stu-id="19395-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="19395-110">列出 deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="19395-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="19395-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="19395-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="19395-112">列出 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="19395-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="19395-113">获取 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="19395-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="19395-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="19395-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="19395-115">读取 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="19395-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="19395-116">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="19395-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="19395-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="19395-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="19395-118">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19395-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="19395-119">删除 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="19395-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="19395-120">无</span><span class="sxs-lookup"><span data-stu-id="19395-120">None</span></span>|<span data-ttu-id="19395-121">删除 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="19395-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="19395-122">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="19395-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="19395-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="19395-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="19395-124">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="19395-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="19395-125">属性</span><span class="sxs-lookup"><span data-stu-id="19395-125">Properties</span></span>
|<span data-ttu-id="19395-126">属性</span><span class="sxs-lookup"><span data-stu-id="19395-126">Property</span></span>|<span data-ttu-id="19395-127">类型</span><span class="sxs-lookup"><span data-stu-id="19395-127">Type</span></span>|<span data-ttu-id="19395-128">说明</span><span class="sxs-lookup"><span data-stu-id="19395-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19395-129">id</span><span class="sxs-lookup"><span data-stu-id="19395-129">id</span></span>|<span data-ttu-id="19395-130">String</span><span class="sxs-lookup"><span data-stu-id="19395-130">String</span></span>|<span data-ttu-id="19395-131">分配的键。</span><span class="sxs-lookup"><span data-stu-id="19395-131">The key of the assignment.</span></span>|
|<span data-ttu-id="19395-132">target</span><span class="sxs-lookup"><span data-stu-id="19395-132">target</span></span>|[<span data-ttu-id="19395-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="19395-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="19395-134">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="19395-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19395-135">关系</span><span class="sxs-lookup"><span data-stu-id="19395-135">Relationships</span></span>
<span data-ttu-id="19395-136">无</span><span class="sxs-lookup"><span data-stu-id="19395-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="19395-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19395-137">JSON Representation</span></span>
<span data-ttu-id="19395-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19395-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



