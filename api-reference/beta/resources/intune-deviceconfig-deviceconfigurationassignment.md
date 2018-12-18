---
title: deviceConfigurationAssignment 资源类型
description: 设备配置分配实体将 AAD 组分配到特定设备配置。
author: tfitzmac
ms.openlocfilehash: ef5a9156b98eb8915471dbc042f6e028542be768
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343292"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="d6b05-103">deviceConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6b05-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="d6b05-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d6b05-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6b05-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d6b05-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6b05-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d6b05-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6b05-107">设备配置分配实体将 AAD 组分配到特定设备配置。</span><span class="sxs-lookup"><span data-stu-id="d6b05-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="d6b05-108">方法</span><span class="sxs-lookup"><span data-stu-id="d6b05-108">Methods</span></span>
|<span data-ttu-id="d6b05-109">方法</span><span class="sxs-lookup"><span data-stu-id="d6b05-109">Method</span></span>|<span data-ttu-id="d6b05-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d6b05-110">Return Type</span></span>|<span data-ttu-id="d6b05-111">说明</span><span class="sxs-lookup"><span data-stu-id="d6b05-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d6b05-112">列出 deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="d6b05-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="d6b05-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d6b05-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d6b05-114">列出 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d6b05-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="d6b05-115">获取 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d6b05-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="d6b05-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d6b05-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="d6b05-117">读取 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d6b05-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="d6b05-118">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d6b05-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="d6b05-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d6b05-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="d6b05-120">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6b05-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="d6b05-121">删除 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d6b05-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="d6b05-122">无</span><span class="sxs-lookup"><span data-stu-id="d6b05-122">None</span></span>|<span data-ttu-id="d6b05-123">删除 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="d6b05-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="d6b05-124">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d6b05-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="d6b05-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d6b05-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="d6b05-126">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d6b05-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d6b05-127">属性</span><span class="sxs-lookup"><span data-stu-id="d6b05-127">Properties</span></span>
|<span data-ttu-id="d6b05-128">属性</span><span class="sxs-lookup"><span data-stu-id="d6b05-128">Property</span></span>|<span data-ttu-id="d6b05-129">类型</span><span class="sxs-lookup"><span data-stu-id="d6b05-129">Type</span></span>|<span data-ttu-id="d6b05-130">说明</span><span class="sxs-lookup"><span data-stu-id="d6b05-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6b05-131">id</span><span class="sxs-lookup"><span data-stu-id="d6b05-131">id</span></span>|<span data-ttu-id="d6b05-132">String</span><span class="sxs-lookup"><span data-stu-id="d6b05-132">String</span></span>|<span data-ttu-id="d6b05-133">分配的键。</span><span class="sxs-lookup"><span data-stu-id="d6b05-133">The key of the assignment.</span></span>|
|<span data-ttu-id="d6b05-134">target</span><span class="sxs-lookup"><span data-stu-id="d6b05-134">target</span></span>|[<span data-ttu-id="d6b05-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d6b05-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d6b05-136">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="d6b05-136">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6b05-137">关系</span><span class="sxs-lookup"><span data-stu-id="d6b05-137">Relationships</span></span>
<span data-ttu-id="d6b05-138">无</span><span class="sxs-lookup"><span data-stu-id="d6b05-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6b05-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6b05-139">JSON Representation</span></span>
<span data-ttu-id="d6b05-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6b05-140">Here is a JSON representation of the resource.</span></span>
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





