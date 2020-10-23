---
title: targetedManagedAppPolicyAssignment 资源类型
description: 组或应用的部署类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d71b74274234139ef4645098031e59d8bd32999b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722800"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a><span data-ttu-id="74b71-103">targetedManagedAppPolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="74b71-103">targetedManagedAppPolicyAssignment resource type</span></span>

<span data-ttu-id="74b71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74b71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74b71-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="74b71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74b71-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74b71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74b71-107">组或应用的部署类型。</span><span class="sxs-lookup"><span data-stu-id="74b71-107">The type for deployment of groups or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="74b71-108">Methods</span><span class="sxs-lookup"><span data-stu-id="74b71-108">Methods</span></span>
|<span data-ttu-id="74b71-109">方法</span><span class="sxs-lookup"><span data-stu-id="74b71-109">Method</span></span>|<span data-ttu-id="74b71-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="74b71-110">Return Type</span></span>|<span data-ttu-id="74b71-111">说明</span><span class="sxs-lookup"><span data-stu-id="74b71-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="74b71-112">列出 targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="74b71-112">List targetedManagedAppPolicyAssignments</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|<span data-ttu-id="74b71-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="74b71-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="74b71-114">列出 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="74b71-114">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="74b71-115">获取 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="74b71-115">Get targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[<span data-ttu-id="74b71-116">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="74b71-116">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="74b71-117">读取 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="74b71-117">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="74b71-118">删除 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="74b71-118">Delete targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|<span data-ttu-id="74b71-119">无</span><span class="sxs-lookup"><span data-stu-id="74b71-119">None</span></span>|<span data-ttu-id="74b71-120">删除 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="74b71-120">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>|
|[<span data-ttu-id="74b71-121">更新 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="74b71-121">Update targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[<span data-ttu-id="74b71-122">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="74b71-122">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="74b71-123">更新 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="74b71-123">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="74b71-124">属性</span><span class="sxs-lookup"><span data-stu-id="74b71-124">Properties</span></span>
|<span data-ttu-id="74b71-125">属性</span><span class="sxs-lookup"><span data-stu-id="74b71-125">Property</span></span>|<span data-ttu-id="74b71-126">类型</span><span class="sxs-lookup"><span data-stu-id="74b71-126">Type</span></span>|<span data-ttu-id="74b71-127">说明</span><span class="sxs-lookup"><span data-stu-id="74b71-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74b71-128">id</span><span class="sxs-lookup"><span data-stu-id="74b71-128">id</span></span>|<span data-ttu-id="74b71-129">String</span><span class="sxs-lookup"><span data-stu-id="74b71-129">String</span></span>|<span data-ttu-id="74b71-130">Id</span><span class="sxs-lookup"><span data-stu-id="74b71-130">Id</span></span>|
|<span data-ttu-id="74b71-131">target</span><span class="sxs-lookup"><span data-stu-id="74b71-131">target</span></span>|[<span data-ttu-id="74b71-132">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="74b71-132">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="74b71-133">用于部署到组或应用的标识符</span><span class="sxs-lookup"><span data-stu-id="74b71-133">Identifier for deployment to a group or app</span></span>|
|<span data-ttu-id="74b71-134">source</span><span class="sxs-lookup"><span data-stu-id="74b71-134">source</span></span>|[<span data-ttu-id="74b71-135">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="74b71-135">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="74b71-136">用于部署到组、direct 或包裹/policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="74b71-136">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="74b71-137">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="74b71-137">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="74b71-138">sourceId</span><span class="sxs-lookup"><span data-stu-id="74b71-138">sourceId</span></span>|<span data-ttu-id="74b71-139">String</span><span class="sxs-lookup"><span data-stu-id="74b71-139">String</span></span>|<span data-ttu-id="74b71-140">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="74b71-140">Identifier for resource used for deployment to a group</span></span>|

## <a name="relationships"></a><span data-ttu-id="74b71-141">关系</span><span class="sxs-lookup"><span data-stu-id="74b71-141">Relationships</span></span>
<span data-ttu-id="74b71-142">无</span><span class="sxs-lookup"><span data-stu-id="74b71-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74b71-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74b71-143">JSON Representation</span></span>
<span data-ttu-id="74b71-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74b71-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
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





