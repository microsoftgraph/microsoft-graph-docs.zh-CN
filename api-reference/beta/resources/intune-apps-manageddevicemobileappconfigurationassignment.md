---
title: managedDeviceMobileAppConfigurationAssignment 资源类型
description: 包含用于为组分配 MDM 应用配置的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a5e67c6399c2f7782c9edbaeeb73d5e5bab0c00f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797949"
---
# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a><span data-ttu-id="57de0-103">managedDeviceMobileAppConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="57de0-103">managedDeviceMobileAppConfigurationAssignment resource type</span></span>

> <span data-ttu-id="57de0-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="57de0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57de0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57de0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57de0-106">包含用于为组分配 MDM 应用配置的属性。</span><span class="sxs-lookup"><span data-stu-id="57de0-106">Contains the properties used to assign an MDM app configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="57de0-107">方法</span><span class="sxs-lookup"><span data-stu-id="57de0-107">Methods</span></span>
|<span data-ttu-id="57de0-108">方法</span><span class="sxs-lookup"><span data-stu-id="57de0-108">Method</span></span>|<span data-ttu-id="57de0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="57de0-109">Return Type</span></span>|<span data-ttu-id="57de0-110">说明</span><span class="sxs-lookup"><span data-stu-id="57de0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="57de0-111">列出 managedDeviceMobileAppConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="57de0-111">List managedDeviceMobileAppConfigurationAssignments</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-list.md)|<span data-ttu-id="57de0-112">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="57de0-112">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="57de0-113">列出 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="57de0-113">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="57de0-114">获取 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57de0-114">Get managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-get.md)|[<span data-ttu-id="57de0-115">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57de0-115">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="57de0-116">读取 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="57de0-116">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="57de0-117">创建 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57de0-117">Create managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-create.md)|[<span data-ttu-id="57de0-118">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57de0-118">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="57de0-119">创建新的 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="57de0-119">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="57de0-120">删除 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57de0-120">Delete managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-delete.md)|<span data-ttu-id="57de0-121">无</span><span class="sxs-lookup"><span data-stu-id="57de0-121">None</span></span>|<span data-ttu-id="57de0-122">删除 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="57de0-122">Deletes a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="57de0-123">更新 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57de0-123">Update managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-update.md)|[<span data-ttu-id="57de0-124">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="57de0-124">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="57de0-125">更新 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="57de0-125">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="57de0-126">属性</span><span class="sxs-lookup"><span data-stu-id="57de0-126">Properties</span></span>
|<span data-ttu-id="57de0-127">属性</span><span class="sxs-lookup"><span data-stu-id="57de0-127">Property</span></span>|<span data-ttu-id="57de0-128">类型</span><span class="sxs-lookup"><span data-stu-id="57de0-128">Type</span></span>|<span data-ttu-id="57de0-129">说明</span><span class="sxs-lookup"><span data-stu-id="57de0-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57de0-130">id</span><span class="sxs-lookup"><span data-stu-id="57de0-130">id</span></span>|<span data-ttu-id="57de0-131">String</span><span class="sxs-lookup"><span data-stu-id="57de0-131">String</span></span>|<span data-ttu-id="57de0-132">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="57de0-132">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="57de0-133">target</span><span class="sxs-lookup"><span data-stu-id="57de0-133">target</span></span>|[<span data-ttu-id="57de0-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="57de0-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="57de0-135">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="57de0-135">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57de0-136">关系</span><span class="sxs-lookup"><span data-stu-id="57de0-136">Relationships</span></span>
<span data-ttu-id="57de0-137">无</span><span class="sxs-lookup"><span data-stu-id="57de0-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57de0-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57de0-138">JSON Representation</span></span>
<span data-ttu-id="57de0-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57de0-139">Here is a JSON representation of the resource.</span></span>
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



