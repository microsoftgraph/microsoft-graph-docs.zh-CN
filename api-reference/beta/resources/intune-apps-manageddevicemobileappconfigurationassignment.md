---
title: managedDeviceMobileAppConfigurationAssignment 资源类型
description: 包含用于为组分配 MDM 应用配置的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eefeef9d40931f869934d1166f6000fc83e8f445
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702591"
---
# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a><span data-ttu-id="9fa37-103">managedDeviceMobileAppConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="9fa37-103">managedDeviceMobileAppConfigurationAssignment resource type</span></span>

<span data-ttu-id="9fa37-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fa37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fa37-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9fa37-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fa37-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9fa37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fa37-107">包含用于为组分配 MDM 应用配置的属性。</span><span class="sxs-lookup"><span data-stu-id="9fa37-107">Contains the properties used to assign an MDM app configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="9fa37-108">Methods</span><span class="sxs-lookup"><span data-stu-id="9fa37-108">Methods</span></span>
|<span data-ttu-id="9fa37-109">方法</span><span class="sxs-lookup"><span data-stu-id="9fa37-109">Method</span></span>|<span data-ttu-id="9fa37-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9fa37-110">Return Type</span></span>|<span data-ttu-id="9fa37-111">说明</span><span class="sxs-lookup"><span data-stu-id="9fa37-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9fa37-112">列出 managedDeviceMobileAppConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="9fa37-112">List managedDeviceMobileAppConfigurationAssignments</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-list.md)|<span data-ttu-id="9fa37-113">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9fa37-113">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="9fa37-114">列出 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9fa37-114">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="9fa37-115">获取 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9fa37-115">Get managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-get.md)|[<span data-ttu-id="9fa37-116">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9fa37-116">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="9fa37-117">读取 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9fa37-117">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="9fa37-118">创建 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9fa37-118">Create managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-create.md)|[<span data-ttu-id="9fa37-119">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9fa37-119">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="9fa37-120">创建新的 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9fa37-120">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="9fa37-121">删除 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9fa37-121">Delete managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-delete.md)|<span data-ttu-id="9fa37-122">无</span><span class="sxs-lookup"><span data-stu-id="9fa37-122">None</span></span>|<span data-ttu-id="9fa37-123">删除 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9fa37-123">Deletes a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="9fa37-124">更新 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9fa37-124">Update managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-update.md)|[<span data-ttu-id="9fa37-125">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9fa37-125">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="9fa37-126">更新 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9fa37-126">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9fa37-127">属性</span><span class="sxs-lookup"><span data-stu-id="9fa37-127">Properties</span></span>
|<span data-ttu-id="9fa37-128">属性</span><span class="sxs-lookup"><span data-stu-id="9fa37-128">Property</span></span>|<span data-ttu-id="9fa37-129">类型</span><span class="sxs-lookup"><span data-stu-id="9fa37-129">Type</span></span>|<span data-ttu-id="9fa37-130">说明</span><span class="sxs-lookup"><span data-stu-id="9fa37-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fa37-131">id</span><span class="sxs-lookup"><span data-stu-id="9fa37-131">id</span></span>|<span data-ttu-id="9fa37-132">String</span><span class="sxs-lookup"><span data-stu-id="9fa37-132">String</span></span>|<span data-ttu-id="9fa37-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9fa37-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="9fa37-134">target</span><span class="sxs-lookup"><span data-stu-id="9fa37-134">target</span></span>|[<span data-ttu-id="9fa37-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9fa37-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9fa37-136">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="9fa37-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fa37-137">关系</span><span class="sxs-lookup"><span data-stu-id="9fa37-137">Relationships</span></span>
<span data-ttu-id="9fa37-138">无</span><span class="sxs-lookup"><span data-stu-id="9fa37-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fa37-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9fa37-139">JSON Representation</span></span>
<span data-ttu-id="9fa37-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fa37-140">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```





