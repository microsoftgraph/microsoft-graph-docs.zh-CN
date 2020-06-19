---
title: enrollmentConfigurationAssignment 资源类型
description: 注册配置分配
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8d6c6137f2baa5937513ad84fd5f68b90e2568e5
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788869"
---
# <a name="enrollmentconfigurationassignment-resource-type"></a><span data-ttu-id="07926-103">enrollmentConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="07926-103">enrollmentConfigurationAssignment resource type</span></span>

<span data-ttu-id="07926-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07926-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07926-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="07926-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07926-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07926-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07926-107">注册配置分配</span><span class="sxs-lookup"><span data-stu-id="07926-107">Enrollment Configuration Assignment</span></span>

## <a name="methods"></a><span data-ttu-id="07926-108">Methods</span><span class="sxs-lookup"><span data-stu-id="07926-108">Methods</span></span>
|<span data-ttu-id="07926-109">方法</span><span class="sxs-lookup"><span data-stu-id="07926-109">Method</span></span>|<span data-ttu-id="07926-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="07926-110">Return Type</span></span>|<span data-ttu-id="07926-111">说明</span><span class="sxs-lookup"><span data-stu-id="07926-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="07926-112">列出 enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="07926-112">List enrollmentConfigurationAssignments</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-list.md)|<span data-ttu-id="07926-113">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07926-113">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="07926-114">列出 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="07926-114">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="07926-115">获取 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="07926-115">Get enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-get.md)|[<span data-ttu-id="07926-116">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="07926-116">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="07926-117">读取 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="07926-117">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="07926-118">创建 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="07926-118">Create enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-create.md)|[<span data-ttu-id="07926-119">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="07926-119">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="07926-120">创建新的 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07926-120">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="07926-121">删除 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="07926-121">Delete enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-delete.md)|<span data-ttu-id="07926-122">无</span><span class="sxs-lookup"><span data-stu-id="07926-122">None</span></span>|<span data-ttu-id="07926-123">删除 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="07926-123">Deletes a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="07926-124">更新 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="07926-124">Update enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-update.md)|[<span data-ttu-id="07926-125">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="07926-125">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="07926-126">更新 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="07926-126">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="07926-127">属性</span><span class="sxs-lookup"><span data-stu-id="07926-127">Properties</span></span>
|<span data-ttu-id="07926-128">属性</span><span class="sxs-lookup"><span data-stu-id="07926-128">Property</span></span>|<span data-ttu-id="07926-129">类型</span><span class="sxs-lookup"><span data-stu-id="07926-129">Type</span></span>|<span data-ttu-id="07926-130">说明</span><span class="sxs-lookup"><span data-stu-id="07926-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07926-131">id</span><span class="sxs-lookup"><span data-stu-id="07926-131">id</span></span>|<span data-ttu-id="07926-132">String</span><span class="sxs-lookup"><span data-stu-id="07926-132">String</span></span>|<span data-ttu-id="07926-133">注册配置分配的键</span><span class="sxs-lookup"><span data-stu-id="07926-133">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="07926-134">target</span><span class="sxs-lookup"><span data-stu-id="07926-134">target</span></span>|[<span data-ttu-id="07926-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="07926-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="07926-136">表示对租户中托管设备的分配</span><span class="sxs-lookup"><span data-stu-id="07926-136">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="07926-137">source</span><span class="sxs-lookup"><span data-stu-id="07926-137">source</span></span>|[<span data-ttu-id="07926-138">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="07926-138">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="07926-139">用于部署到组、direct 或 policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="07926-139">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="07926-140">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="07926-140">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="07926-141">sourceId</span><span class="sxs-lookup"><span data-stu-id="07926-141">sourceId</span></span>|<span data-ttu-id="07926-142">String</span><span class="sxs-lookup"><span data-stu-id="07926-142">String</span></span>|<span data-ttu-id="07926-143">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="07926-143">Identifier for resource used for deployment to a group</span></span>|

## <a name="relationships"></a><span data-ttu-id="07926-144">关系</span><span class="sxs-lookup"><span data-stu-id="07926-144">Relationships</span></span>
<span data-ttu-id="07926-145">无</span><span class="sxs-lookup"><span data-stu-id="07926-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07926-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07926-146">JSON Representation</span></span>
<span data-ttu-id="07926-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07926-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  },
  "source": "String",
  "sourceId": "String"
}
```



