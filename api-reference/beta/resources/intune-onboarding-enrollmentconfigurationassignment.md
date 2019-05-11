---
title: enrollmentConfigurationAssignment 资源类型
description: 注册配置分配
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4683997a061e756a1860349644d2a2d0cfaa5246
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940189"
---
# <a name="enrollmentconfigurationassignment-resource-type"></a><span data-ttu-id="0258d-103">enrollmentConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="0258d-103">enrollmentConfigurationAssignment resource type</span></span>

> <span data-ttu-id="0258d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0258d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0258d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0258d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0258d-106">注册配置分配</span><span class="sxs-lookup"><span data-stu-id="0258d-106">Enrollment Configuration Assignment</span></span>

## <a name="methods"></a><span data-ttu-id="0258d-107">方法</span><span class="sxs-lookup"><span data-stu-id="0258d-107">Methods</span></span>
|<span data-ttu-id="0258d-108">方法</span><span class="sxs-lookup"><span data-stu-id="0258d-108">Method</span></span>|<span data-ttu-id="0258d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0258d-109">Return Type</span></span>|<span data-ttu-id="0258d-110">说明</span><span class="sxs-lookup"><span data-stu-id="0258d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0258d-111">列出 enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="0258d-111">List enrollmentConfigurationAssignments</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-list.md)|<span data-ttu-id="0258d-112">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0258d-112">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0258d-113">列出 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0258d-113">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="0258d-114">获取 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0258d-114">Get enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-get.md)|[<span data-ttu-id="0258d-115">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0258d-115">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="0258d-116">读取 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0258d-116">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="0258d-117">创建 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0258d-117">Create enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-create.md)|[<span data-ttu-id="0258d-118">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0258d-118">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="0258d-119">创建新的 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0258d-119">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="0258d-120">删除 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0258d-120">Delete enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-delete.md)|<span data-ttu-id="0258d-121">无</span><span class="sxs-lookup"><span data-stu-id="0258d-121">None</span></span>|<span data-ttu-id="0258d-122">删除 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="0258d-122">Deletes a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="0258d-123">更新 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0258d-123">Update enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-update.md)|[<span data-ttu-id="0258d-124">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0258d-124">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="0258d-125">更新 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0258d-125">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0258d-126">属性</span><span class="sxs-lookup"><span data-stu-id="0258d-126">Properties</span></span>
|<span data-ttu-id="0258d-127">属性</span><span class="sxs-lookup"><span data-stu-id="0258d-127">Property</span></span>|<span data-ttu-id="0258d-128">类型</span><span class="sxs-lookup"><span data-stu-id="0258d-128">Type</span></span>|<span data-ttu-id="0258d-129">说明</span><span class="sxs-lookup"><span data-stu-id="0258d-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0258d-130">id</span><span class="sxs-lookup"><span data-stu-id="0258d-130">id</span></span>|<span data-ttu-id="0258d-131">String</span><span class="sxs-lookup"><span data-stu-id="0258d-131">String</span></span>|<span data-ttu-id="0258d-132">注册配置分配的键</span><span class="sxs-lookup"><span data-stu-id="0258d-132">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="0258d-133">target</span><span class="sxs-lookup"><span data-stu-id="0258d-133">target</span></span>|[<span data-ttu-id="0258d-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0258d-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0258d-135">表示对租户中托管设备的分配</span><span class="sxs-lookup"><span data-stu-id="0258d-135">Represents an assignment to managed devices in the tenant</span></span>|

## <a name="relationships"></a><span data-ttu-id="0258d-136">关系</span><span class="sxs-lookup"><span data-stu-id="0258d-136">Relationships</span></span>
<span data-ttu-id="0258d-137">无</span><span class="sxs-lookup"><span data-stu-id="0258d-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0258d-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0258d-138">JSON Representation</span></span>
<span data-ttu-id="0258d-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0258d-139">Here is a JSON representation of the resource.</span></span>
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
  }
}
```




