---
title: managedDeviceMobileAppConfigurationAssignment 资源类型
description: 包含用于为组分配 MDM 应用配置的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c04947c63a72ebb1476ce5c863731a876987d603
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830175"
---
# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a><span data-ttu-id="52b7a-103">managedDeviceMobileAppConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="52b7a-103">managedDeviceMobileAppConfigurationAssignment resource type</span></span>

> <span data-ttu-id="52b7a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="52b7a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52b7a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="52b7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52b7a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="52b7a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52b7a-107">包含用于为组分配 MDM 应用配置的属性。</span><span class="sxs-lookup"><span data-stu-id="52b7a-107">Contains the properties used to assign an MDM app configuration to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="52b7a-108">方法</span><span class="sxs-lookup"><span data-stu-id="52b7a-108">Methods</span></span>
|<span data-ttu-id="52b7a-109">方法</span><span class="sxs-lookup"><span data-stu-id="52b7a-109">Method</span></span>|<span data-ttu-id="52b7a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="52b7a-110">Return Type</span></span>|<span data-ttu-id="52b7a-111">说明</span><span class="sxs-lookup"><span data-stu-id="52b7a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="52b7a-112">列出 managedDeviceMobileAppConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="52b7a-112">List managedDeviceMobileAppConfigurationAssignments</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-list.md)|<span data-ttu-id="52b7a-113">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="52b7a-113">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="52b7a-114">列出 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="52b7a-114">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="52b7a-115">获取 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="52b7a-115">Get managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-get.md)|[<span data-ttu-id="52b7a-116">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="52b7a-116">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="52b7a-117">读取 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="52b7a-117">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="52b7a-118">创建 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="52b7a-118">Create managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-create.md)|[<span data-ttu-id="52b7a-119">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="52b7a-119">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="52b7a-120">创建新的 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="52b7a-120">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="52b7a-121">删除 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="52b7a-121">Delete managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-delete.md)|<span data-ttu-id="52b7a-122">无</span><span class="sxs-lookup"><span data-stu-id="52b7a-122">None</span></span>|<span data-ttu-id="52b7a-123">删除 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="52b7a-123">Deletes a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="52b7a-124">更新 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="52b7a-124">Update managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-update.md)|[<span data-ttu-id="52b7a-125">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="52b7a-125">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="52b7a-126">更新 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="52b7a-126">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="52b7a-127">属性</span><span class="sxs-lookup"><span data-stu-id="52b7a-127">Properties</span></span>
|<span data-ttu-id="52b7a-128">属性</span><span class="sxs-lookup"><span data-stu-id="52b7a-128">Property</span></span>|<span data-ttu-id="52b7a-129">类型</span><span class="sxs-lookup"><span data-stu-id="52b7a-129">Type</span></span>|<span data-ttu-id="52b7a-130">说明</span><span class="sxs-lookup"><span data-stu-id="52b7a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52b7a-131">id</span><span class="sxs-lookup"><span data-stu-id="52b7a-131">id</span></span>|<span data-ttu-id="52b7a-132">String</span><span class="sxs-lookup"><span data-stu-id="52b7a-132">String</span></span>|<span data-ttu-id="52b7a-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="52b7a-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="52b7a-134">target</span><span class="sxs-lookup"><span data-stu-id="52b7a-134">target</span></span>|[<span data-ttu-id="52b7a-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="52b7a-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="52b7a-136">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="52b7a-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52b7a-137">关系</span><span class="sxs-lookup"><span data-stu-id="52b7a-137">Relationships</span></span>
<span data-ttu-id="52b7a-138">无</span><span class="sxs-lookup"><span data-stu-id="52b7a-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="52b7a-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52b7a-139">JSON Representation</span></span>
<span data-ttu-id="52b7a-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52b7a-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





