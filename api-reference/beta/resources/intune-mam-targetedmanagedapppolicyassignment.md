---
title: targetedManagedAppPolicyAssignment 资源类型
description: 组或应用的部署类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a9131a5bdfbdd33b9286d5d5f2800969a5eb03f6
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196488"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a><span data-ttu-id="b7314-103">targetedManagedAppPolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7314-103">targetedManagedAppPolicyAssignment resource type</span></span>

> <span data-ttu-id="b7314-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b7314-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7314-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7314-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7314-106">组或应用的部署类型。</span><span class="sxs-lookup"><span data-stu-id="b7314-106">The type for deployment of groups or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="b7314-107">方法</span><span class="sxs-lookup"><span data-stu-id="b7314-107">Methods</span></span>
|<span data-ttu-id="b7314-108">方法</span><span class="sxs-lookup"><span data-stu-id="b7314-108">Method</span></span>|<span data-ttu-id="b7314-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b7314-109">Return Type</span></span>|<span data-ttu-id="b7314-110">说明</span><span class="sxs-lookup"><span data-stu-id="b7314-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b7314-111">列出 targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="b7314-111">List targetedManagedAppPolicyAssignments</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|<span data-ttu-id="b7314-112">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b7314-112">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="b7314-113">列出 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b7314-113">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="b7314-114">获取 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="b7314-114">Get targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[<span data-ttu-id="b7314-115">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="b7314-115">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="b7314-116">读取 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b7314-116">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="b7314-117">删除 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="b7314-117">Delete targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|<span data-ttu-id="b7314-118">无</span><span class="sxs-lookup"><span data-stu-id="b7314-118">None</span></span>|<span data-ttu-id="b7314-119">删除 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="b7314-119">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>|
|[<span data-ttu-id="b7314-120">更新 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="b7314-120">Update targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[<span data-ttu-id="b7314-121">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="b7314-121">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="b7314-122">更新 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b7314-122">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b7314-123">属性</span><span class="sxs-lookup"><span data-stu-id="b7314-123">Properties</span></span>
|<span data-ttu-id="b7314-124">属性</span><span class="sxs-lookup"><span data-stu-id="b7314-124">Property</span></span>|<span data-ttu-id="b7314-125">类型</span><span class="sxs-lookup"><span data-stu-id="b7314-125">Type</span></span>|<span data-ttu-id="b7314-126">说明</span><span class="sxs-lookup"><span data-stu-id="b7314-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7314-127">id</span><span class="sxs-lookup"><span data-stu-id="b7314-127">id</span></span>|<span data-ttu-id="b7314-128">String</span><span class="sxs-lookup"><span data-stu-id="b7314-128">String</span></span>|<span data-ttu-id="b7314-129">Id</span><span class="sxs-lookup"><span data-stu-id="b7314-129">Id</span></span>|
|<span data-ttu-id="b7314-130">target</span><span class="sxs-lookup"><span data-stu-id="b7314-130">target</span></span>|[<span data-ttu-id="b7314-131">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b7314-131">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b7314-132">用于部署到组或应用的标识符</span><span class="sxs-lookup"><span data-stu-id="b7314-132">Identifier for deployment to a group or app</span></span>|
|<span data-ttu-id="b7314-133">source</span><span class="sxs-lookup"><span data-stu-id="b7314-133">source</span></span>|[<span data-ttu-id="b7314-134">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="b7314-134">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="b7314-135">用于部署到组、direct 或包裹/policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="b7314-135">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="b7314-136">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="b7314-136">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="b7314-137">sourceId</span><span class="sxs-lookup"><span data-stu-id="b7314-137">sourceId</span></span>|<span data-ttu-id="b7314-138">String</span><span class="sxs-lookup"><span data-stu-id="b7314-138">String</span></span>|<span data-ttu-id="b7314-139">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="b7314-139">Identifier for resource used for deployment to a group</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7314-140">关系</span><span class="sxs-lookup"><span data-stu-id="b7314-140">Relationships</span></span>
<span data-ttu-id="b7314-141">无</span><span class="sxs-lookup"><span data-stu-id="b7314-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7314-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7314-142">JSON Representation</span></span>
<span data-ttu-id="b7314-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7314-143">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "String",
  "sourceId": "String"
}
```



