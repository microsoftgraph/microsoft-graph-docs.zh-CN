---
title: targetedManagedAppPolicyAssignment 资源类型
description: 组或应用的部署类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ef08bf86618fae9d4899cc3335742b1b49962bee
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156803"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a><span data-ttu-id="617c3-103">targetedManagedAppPolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="617c3-103">targetedManagedAppPolicyAssignment resource type</span></span>

<span data-ttu-id="617c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="617c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="617c3-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="617c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="617c3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="617c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="617c3-107">组或应用的部署类型。</span><span class="sxs-lookup"><span data-stu-id="617c3-107">The type for deployment of groups or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="617c3-108">方法</span><span class="sxs-lookup"><span data-stu-id="617c3-108">Methods</span></span>
|<span data-ttu-id="617c3-109">方法</span><span class="sxs-lookup"><span data-stu-id="617c3-109">Method</span></span>|<span data-ttu-id="617c3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="617c3-110">Return Type</span></span>|<span data-ttu-id="617c3-111">说明</span><span class="sxs-lookup"><span data-stu-id="617c3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="617c3-112">列出 targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="617c3-112">List targetedManagedAppPolicyAssignments</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|<span data-ttu-id="617c3-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="617c3-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="617c3-114">列出 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="617c3-114">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="617c3-115">获取 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="617c3-115">Get targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[<span data-ttu-id="617c3-116">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="617c3-116">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="617c3-117">读取 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="617c3-117">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="617c3-118">删除 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="617c3-118">Delete targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|<span data-ttu-id="617c3-119">无</span><span class="sxs-lookup"><span data-stu-id="617c3-119">None</span></span>|<span data-ttu-id="617c3-120">删除 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="617c3-120">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>|
|[<span data-ttu-id="617c3-121">更新 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="617c3-121">Update targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[<span data-ttu-id="617c3-122">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="617c3-122">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="617c3-123">更新 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="617c3-123">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="617c3-124">属性</span><span class="sxs-lookup"><span data-stu-id="617c3-124">Properties</span></span>
|<span data-ttu-id="617c3-125">属性</span><span class="sxs-lookup"><span data-stu-id="617c3-125">Property</span></span>|<span data-ttu-id="617c3-126">类型</span><span class="sxs-lookup"><span data-stu-id="617c3-126">Type</span></span>|<span data-ttu-id="617c3-127">说明</span><span class="sxs-lookup"><span data-stu-id="617c3-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="617c3-128">id</span><span class="sxs-lookup"><span data-stu-id="617c3-128">id</span></span>|<span data-ttu-id="617c3-129">String</span><span class="sxs-lookup"><span data-stu-id="617c3-129">String</span></span>|<span data-ttu-id="617c3-130">Id</span><span class="sxs-lookup"><span data-stu-id="617c3-130">Id</span></span>|
|<span data-ttu-id="617c3-131">target</span><span class="sxs-lookup"><span data-stu-id="617c3-131">target</span></span>|[<span data-ttu-id="617c3-132">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="617c3-132">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="617c3-133">部署到组或应用的标识符</span><span class="sxs-lookup"><span data-stu-id="617c3-133">Identifier for deployment to a group or app</span></span>|
|<span data-ttu-id="617c3-134">source</span><span class="sxs-lookup"><span data-stu-id="617c3-134">source</span></span>|[<span data-ttu-id="617c3-135">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="617c3-135">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="617c3-136">用于部署到组的资源类型、直接资源或项目/策略集。</span><span class="sxs-lookup"><span data-stu-id="617c3-136">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="617c3-137">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="617c3-137">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="617c3-138">sourceId</span><span class="sxs-lookup"><span data-stu-id="617c3-138">sourceId</span></span>|<span data-ttu-id="617c3-139">String</span><span class="sxs-lookup"><span data-stu-id="617c3-139">String</span></span>|<span data-ttu-id="617c3-140">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="617c3-140">Identifier for resource used for deployment to a group</span></span>|

## <a name="relationships"></a><span data-ttu-id="617c3-141">关系</span><span class="sxs-lookup"><span data-stu-id="617c3-141">Relationships</span></span>
<span data-ttu-id="617c3-142">无</span><span class="sxs-lookup"><span data-stu-id="617c3-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="617c3-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="617c3-143">JSON Representation</span></span>
<span data-ttu-id="617c3-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="617c3-144">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  },
  "source": "String",
  "sourceId": "String"
}
```




