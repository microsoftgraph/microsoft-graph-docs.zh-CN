---
title: targetedManagedAppPolicyAssignment 资源类型
description: 组或应用的部署类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b496dea2e39c3e8f5e4f7d15e5cc7893df259069
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263978"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a><span data-ttu-id="345af-103">targetedManagedAppPolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="345af-103">targetedManagedAppPolicyAssignment resource type</span></span>

> <span data-ttu-id="345af-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="345af-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="345af-105">组或应用的部署类型。</span><span class="sxs-lookup"><span data-stu-id="345af-105">The type for deployment of groups or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="345af-106">方法</span><span class="sxs-lookup"><span data-stu-id="345af-106">Methods</span></span>
|<span data-ttu-id="345af-107">方法</span><span class="sxs-lookup"><span data-stu-id="345af-107">Method</span></span>|<span data-ttu-id="345af-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="345af-108">Return Type</span></span>|<span data-ttu-id="345af-109">说明</span><span class="sxs-lookup"><span data-stu-id="345af-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="345af-110">列出 targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="345af-110">List targetedManagedAppPolicyAssignments</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|<span data-ttu-id="345af-111">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="345af-111">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="345af-112">列出 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="345af-112">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="345af-113">获取 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="345af-113">Get targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[<span data-ttu-id="345af-114">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="345af-114">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="345af-115">读取 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="345af-115">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="345af-116">删除 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="345af-116">Delete targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|<span data-ttu-id="345af-117">无</span><span class="sxs-lookup"><span data-stu-id="345af-117">None</span></span>|<span data-ttu-id="345af-118">删除 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="345af-118">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>|
|[<span data-ttu-id="345af-119">更新 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="345af-119">Update targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[<span data-ttu-id="345af-120">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="345af-120">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="345af-121">更新 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="345af-121">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="345af-122">属性</span><span class="sxs-lookup"><span data-stu-id="345af-122">Properties</span></span>
|<span data-ttu-id="345af-123">属性</span><span class="sxs-lookup"><span data-stu-id="345af-123">Property</span></span>|<span data-ttu-id="345af-124">类型</span><span class="sxs-lookup"><span data-stu-id="345af-124">Type</span></span>|<span data-ttu-id="345af-125">说明</span><span class="sxs-lookup"><span data-stu-id="345af-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="345af-126">id</span><span class="sxs-lookup"><span data-stu-id="345af-126">id</span></span>|<span data-ttu-id="345af-127">String</span><span class="sxs-lookup"><span data-stu-id="345af-127">String</span></span>|<span data-ttu-id="345af-128">Id</span><span class="sxs-lookup"><span data-stu-id="345af-128">Id</span></span>|
|<span data-ttu-id="345af-129">target</span><span class="sxs-lookup"><span data-stu-id="345af-129">target</span></span>|[<span data-ttu-id="345af-130">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="345af-130">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="345af-131">组或应用的部署标识符</span><span class="sxs-lookup"><span data-stu-id="345af-131">Identifier for deployment of a group or app</span></span>|

## <a name="relationships"></a><span data-ttu-id="345af-132">关系</span><span class="sxs-lookup"><span data-stu-id="345af-132">Relationships</span></span>
<span data-ttu-id="345af-133">无</span><span class="sxs-lookup"><span data-stu-id="345af-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="345af-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="345af-134">JSON Representation</span></span>
<span data-ttu-id="345af-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="345af-135">Here is a JSON representation of the resource.</span></span>
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
  }
}
```



