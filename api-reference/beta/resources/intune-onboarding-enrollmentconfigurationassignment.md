---
title: enrollmentConfigurationAssignment 资源类型
description: 注册配置分配
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d74b8462dc99476b120f3b468e34b731c3db314b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538985"
---
# <a name="enrollmentconfigurationassignment-resource-type"></a><span data-ttu-id="9628f-103">enrollmentConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="9628f-103">enrollmentConfigurationAssignment resource type</span></span>

> <span data-ttu-id="9628f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9628f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9628f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9628f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9628f-106">注册配置分配</span><span class="sxs-lookup"><span data-stu-id="9628f-106">Enrollment Configuration Assignment</span></span>

## <a name="methods"></a><span data-ttu-id="9628f-107">方法</span><span class="sxs-lookup"><span data-stu-id="9628f-107">Methods</span></span>
|<span data-ttu-id="9628f-108">方法</span><span class="sxs-lookup"><span data-stu-id="9628f-108">Method</span></span>|<span data-ttu-id="9628f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9628f-109">Return Type</span></span>|<span data-ttu-id="9628f-110">说明</span><span class="sxs-lookup"><span data-stu-id="9628f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9628f-111">列出 enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="9628f-111">List enrollmentConfigurationAssignments</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-list.md)|<span data-ttu-id="9628f-112">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9628f-112">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="9628f-113">列出 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9628f-113">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="9628f-114">获取 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9628f-114">Get enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-get.md)|[<span data-ttu-id="9628f-115">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9628f-115">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="9628f-116">读取 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9628f-116">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="9628f-117">创建 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9628f-117">Create enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-create.md)|[<span data-ttu-id="9628f-118">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9628f-118">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="9628f-119">创建新的 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9628f-119">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="9628f-120">删除 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9628f-120">Delete enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-delete.md)|<span data-ttu-id="9628f-121">无</span><span class="sxs-lookup"><span data-stu-id="9628f-121">None</span></span>|<span data-ttu-id="9628f-122">删除 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="9628f-122">Deletes a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="9628f-123">更新 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9628f-123">Update enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-update.md)|[<span data-ttu-id="9628f-124">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9628f-124">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="9628f-125">更新 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9628f-125">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9628f-126">属性</span><span class="sxs-lookup"><span data-stu-id="9628f-126">Properties</span></span>
|<span data-ttu-id="9628f-127">属性</span><span class="sxs-lookup"><span data-stu-id="9628f-127">Property</span></span>|<span data-ttu-id="9628f-128">类型</span><span class="sxs-lookup"><span data-stu-id="9628f-128">Type</span></span>|<span data-ttu-id="9628f-129">说明</span><span class="sxs-lookup"><span data-stu-id="9628f-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9628f-130">id</span><span class="sxs-lookup"><span data-stu-id="9628f-130">id</span></span>|<span data-ttu-id="9628f-131">字符串</span><span class="sxs-lookup"><span data-stu-id="9628f-131">String</span></span>|<span data-ttu-id="9628f-132">注册配置分配的键</span><span class="sxs-lookup"><span data-stu-id="9628f-132">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="9628f-133">target</span><span class="sxs-lookup"><span data-stu-id="9628f-133">target</span></span>|[<span data-ttu-id="9628f-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9628f-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9628f-135">表示对租户中托管设备的分配</span><span class="sxs-lookup"><span data-stu-id="9628f-135">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="9628f-136">source</span><span class="sxs-lookup"><span data-stu-id="9628f-136">source</span></span>|[<span data-ttu-id="9628f-137">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="9628f-137">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="9628f-138">用于部署到组、direct 或 policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="9628f-138">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="9628f-139">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="9628f-139">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="9628f-140">sourceId</span><span class="sxs-lookup"><span data-stu-id="9628f-140">sourceId</span></span>|<span data-ttu-id="9628f-141">字符串</span><span class="sxs-lookup"><span data-stu-id="9628f-141">String</span></span>|<span data-ttu-id="9628f-142">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="9628f-142">Identifier for resource used for deployment to a group</span></span>|

## <a name="relationships"></a><span data-ttu-id="9628f-143">关系</span><span class="sxs-lookup"><span data-stu-id="9628f-143">Relationships</span></span>
<span data-ttu-id="9628f-144">无</span><span class="sxs-lookup"><span data-stu-id="9628f-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9628f-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9628f-145">JSON Representation</span></span>
<span data-ttu-id="9628f-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9628f-146">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "String",
  "sourceId": "String"
}
```



