---
title: enrollmentConfigurationAssignment 资源类型
description: 注册配置分配
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8a972a1004a749c2103663d7aeb0335dc0c42433
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752446"
---
# <a name="enrollmentconfigurationassignment-resource-type"></a><span data-ttu-id="95c1f-103">enrollmentConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="95c1f-103">enrollmentConfigurationAssignment resource type</span></span>

<span data-ttu-id="95c1f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95c1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95c1f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95c1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95c1f-106">注册配置分配</span><span class="sxs-lookup"><span data-stu-id="95c1f-106">Enrollment Configuration Assignment</span></span>

## <a name="methods"></a><span data-ttu-id="95c1f-107">Methods</span><span class="sxs-lookup"><span data-stu-id="95c1f-107">Methods</span></span>
|<span data-ttu-id="95c1f-108">方法</span><span class="sxs-lookup"><span data-stu-id="95c1f-108">Method</span></span>|<span data-ttu-id="95c1f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="95c1f-109">Return Type</span></span>|<span data-ttu-id="95c1f-110">Description</span><span class="sxs-lookup"><span data-stu-id="95c1f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="95c1f-111">列出 enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="95c1f-111">List enrollmentConfigurationAssignments</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-list.md)|<span data-ttu-id="95c1f-112">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="95c1f-112">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="95c1f-113">列出 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="95c1f-113">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="95c1f-114">获取 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="95c1f-114">Get enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-get.md)|[<span data-ttu-id="95c1f-115">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="95c1f-115">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="95c1f-116">读取 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="95c1f-116">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="95c1f-117">创建 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="95c1f-117">Create enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-create.md)|[<span data-ttu-id="95c1f-118">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="95c1f-118">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="95c1f-119">创建新的 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95c1f-119">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="95c1f-120">删除 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="95c1f-120">Delete enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-delete.md)|<span data-ttu-id="95c1f-121">无</span><span class="sxs-lookup"><span data-stu-id="95c1f-121">None</span></span>|<span data-ttu-id="95c1f-122">删除 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="95c1f-122">Deletes a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="95c1f-123">更新 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="95c1f-123">Update enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-update.md)|[<span data-ttu-id="95c1f-124">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="95c1f-124">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="95c1f-125">更新 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="95c1f-125">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="95c1f-126">属性</span><span class="sxs-lookup"><span data-stu-id="95c1f-126">Properties</span></span>
|<span data-ttu-id="95c1f-127">属性</span><span class="sxs-lookup"><span data-stu-id="95c1f-127">Property</span></span>|<span data-ttu-id="95c1f-128">类型</span><span class="sxs-lookup"><span data-stu-id="95c1f-128">Type</span></span>|<span data-ttu-id="95c1f-129">说明</span><span class="sxs-lookup"><span data-stu-id="95c1f-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95c1f-130">id</span><span class="sxs-lookup"><span data-stu-id="95c1f-130">id</span></span>|<span data-ttu-id="95c1f-131">String</span><span class="sxs-lookup"><span data-stu-id="95c1f-131">String</span></span>|<span data-ttu-id="95c1f-132">注册配置分配密钥</span><span class="sxs-lookup"><span data-stu-id="95c1f-132">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="95c1f-133">target</span><span class="sxs-lookup"><span data-stu-id="95c1f-133">target</span></span>|[<span data-ttu-id="95c1f-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="95c1f-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="95c1f-135">表示对租户中托管设备的分配</span><span class="sxs-lookup"><span data-stu-id="95c1f-135">Represents an assignment to managed devices in the tenant</span></span>|

## <a name="relationships"></a><span data-ttu-id="95c1f-136">关系</span><span class="sxs-lookup"><span data-stu-id="95c1f-136">Relationships</span></span>
<span data-ttu-id="95c1f-137">无</span><span class="sxs-lookup"><span data-stu-id="95c1f-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95c1f-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95c1f-138">JSON Representation</span></span>
<span data-ttu-id="95c1f-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95c1f-139">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "String"
  }
}
```




