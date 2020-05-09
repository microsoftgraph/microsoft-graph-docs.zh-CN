---
title: targetedManagedAppPolicyAssignment 资源类型
description: 组或应用的部署类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b0a5cea38b4f0cf7bd24207ddf67a8f41a690d5
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178379"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a><span data-ttu-id="a9387-103">targetedManagedAppPolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9387-103">targetedManagedAppPolicyAssignment resource type</span></span>

<span data-ttu-id="a9387-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9387-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9387-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9387-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9387-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9387-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9387-107">组或应用的部署类型。</span><span class="sxs-lookup"><span data-stu-id="a9387-107">The type for deployment of groups or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="a9387-108">方法</span><span class="sxs-lookup"><span data-stu-id="a9387-108">Methods</span></span>
|<span data-ttu-id="a9387-109">方法</span><span class="sxs-lookup"><span data-stu-id="a9387-109">Method</span></span>|<span data-ttu-id="a9387-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a9387-110">Return Type</span></span>|<span data-ttu-id="a9387-111">说明</span><span class="sxs-lookup"><span data-stu-id="a9387-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a9387-112">列出 targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="a9387-112">List targetedManagedAppPolicyAssignments</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|<span data-ttu-id="a9387-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a9387-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="a9387-114">列出 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a9387-114">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="a9387-115">获取 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="a9387-115">Get targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[<span data-ttu-id="a9387-116">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="a9387-116">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="a9387-117">读取 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a9387-117">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="a9387-118">删除 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="a9387-118">Delete targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|<span data-ttu-id="a9387-119">无</span><span class="sxs-lookup"><span data-stu-id="a9387-119">None</span></span>|<span data-ttu-id="a9387-120">删除 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="a9387-120">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>|
|[<span data-ttu-id="a9387-121">更新 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="a9387-121">Update targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[<span data-ttu-id="a9387-122">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="a9387-122">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="a9387-123">更新 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a9387-123">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a9387-124">属性</span><span class="sxs-lookup"><span data-stu-id="a9387-124">Properties</span></span>
|<span data-ttu-id="a9387-125">属性</span><span class="sxs-lookup"><span data-stu-id="a9387-125">Property</span></span>|<span data-ttu-id="a9387-126">类型</span><span class="sxs-lookup"><span data-stu-id="a9387-126">Type</span></span>|<span data-ttu-id="a9387-127">说明</span><span class="sxs-lookup"><span data-stu-id="a9387-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9387-128">id</span><span class="sxs-lookup"><span data-stu-id="a9387-128">id</span></span>|<span data-ttu-id="a9387-129">字符串</span><span class="sxs-lookup"><span data-stu-id="a9387-129">String</span></span>|<span data-ttu-id="a9387-130">Id</span><span class="sxs-lookup"><span data-stu-id="a9387-130">Id</span></span>|
|<span data-ttu-id="a9387-131">target</span><span class="sxs-lookup"><span data-stu-id="a9387-131">target</span></span>|[<span data-ttu-id="a9387-132">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a9387-132">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a9387-133">用于部署到组或应用的标识符</span><span class="sxs-lookup"><span data-stu-id="a9387-133">Identifier for deployment to a group or app</span></span>|
|<span data-ttu-id="a9387-134">source</span><span class="sxs-lookup"><span data-stu-id="a9387-134">source</span></span>|[<span data-ttu-id="a9387-135">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="a9387-135">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="a9387-136">用于部署到组、direct 或包裹/policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="a9387-136">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="a9387-137">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="a9387-137">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="a9387-138">sourceId</span><span class="sxs-lookup"><span data-stu-id="a9387-138">sourceId</span></span>|<span data-ttu-id="a9387-139">字符串</span><span class="sxs-lookup"><span data-stu-id="a9387-139">String</span></span>|<span data-ttu-id="a9387-140">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="a9387-140">Identifier for resource used for deployment to a group</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9387-141">关系</span><span class="sxs-lookup"><span data-stu-id="a9387-141">Relationships</span></span>
<span data-ttu-id="a9387-142">无</span><span class="sxs-lookup"><span data-stu-id="a9387-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9387-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9387-143">JSON Representation</span></span>
<span data-ttu-id="a9387-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9387-144">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  },
  "source": "String",
  "sourceId": "String"
}
```



