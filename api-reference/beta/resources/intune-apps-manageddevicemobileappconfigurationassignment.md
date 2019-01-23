---
title: managedDeviceMobileAppConfigurationAssignment 资源类型
description: 包含用于为组分配 MDM 应用配置的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 092cbfb1cfabea1d52b58caf70a34b1129c2653b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392764"
---
# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a><span data-ttu-id="57615-103">managedDeviceMobileAppConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="57615-103">managedDeviceMobileAppConfigurationAssignment resource type</span></span>

> <span data-ttu-id="57615-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="57615-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="57615-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="57615-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57615-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57615-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57615-107">包含用于为组分配 MDM 应用配置的属性。</span><span class="sxs-lookup"><span data-stu-id="57615-107">Contains the properties used to assign an MDM app configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="57615-108">方法</span><span class="sxs-lookup"><span data-stu-id="57615-108">Methods</span></span>
|<span data-ttu-id="57615-109">方法</span><span class="sxs-lookup"><span data-stu-id="57615-109">Method</span></span>|<span data-ttu-id="57615-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="57615-110">Return Type</span></span>|<span data-ttu-id="57615-111">说明</span><span class="sxs-lookup"><span data-stu-id="57615-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="57615-112">列出 managedDeviceMobileAppConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="57615-112">List managedDeviceMobileAppConfigurationAssignments</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-list.md)|<span data-ttu-id="57615-113">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="57615-113">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="57615-114">列出 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="57615-114">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="57615-115">获取 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57615-115">Get managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-get.md)|[<span data-ttu-id="57615-116">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57615-116">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="57615-117">读取 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="57615-117">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="57615-118">创建 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57615-118">Create managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-create.md)|[<span data-ttu-id="57615-119">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57615-119">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="57615-120">创建新的 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="57615-120">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="57615-121">删除 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57615-121">Delete managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-delete.md)|<span data-ttu-id="57615-122">无</span><span class="sxs-lookup"><span data-stu-id="57615-122">None</span></span>|<span data-ttu-id="57615-123">删除 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="57615-123">Deletes a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="57615-124">更新 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57615-124">Update managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-update.md)|[<span data-ttu-id="57615-125">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57615-125">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="57615-126">更新 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="57615-126">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="57615-127">属性</span><span class="sxs-lookup"><span data-stu-id="57615-127">Properties</span></span>
|<span data-ttu-id="57615-128">属性</span><span class="sxs-lookup"><span data-stu-id="57615-128">Property</span></span>|<span data-ttu-id="57615-129">类型</span><span class="sxs-lookup"><span data-stu-id="57615-129">Type</span></span>|<span data-ttu-id="57615-130">说明</span><span class="sxs-lookup"><span data-stu-id="57615-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57615-131">id</span><span class="sxs-lookup"><span data-stu-id="57615-131">id</span></span>|<span data-ttu-id="57615-132">String</span><span class="sxs-lookup"><span data-stu-id="57615-132">String</span></span>|<span data-ttu-id="57615-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="57615-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="57615-134">target</span><span class="sxs-lookup"><span data-stu-id="57615-134">target</span></span>|[<span data-ttu-id="57615-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="57615-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="57615-136">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="57615-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57615-137">关系</span><span class="sxs-lookup"><span data-stu-id="57615-137">Relationships</span></span>
<span data-ttu-id="57615-138">无</span><span class="sxs-lookup"><span data-stu-id="57615-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57615-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57615-139">JSON Representation</span></span>
<span data-ttu-id="57615-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57615-140">Here is a JSON representation of the resource.</span></span>
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




