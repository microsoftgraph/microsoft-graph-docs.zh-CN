---
title: targetedManagedAppPolicyAssignment 资源类型
description: 组或应用的部署类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c40c2d7c8c998fc4a271e1efeff10062388522f3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395942"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a><span data-ttu-id="8b671-103">targetedManagedAppPolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b671-103">targetedManagedAppPolicyAssignment resource type</span></span>

> <span data-ttu-id="8b671-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="8b671-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8b671-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8b671-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b671-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8b671-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b671-107">组或应用的部署类型。</span><span class="sxs-lookup"><span data-stu-id="8b671-107">The type for deployment of groups or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="8b671-108">方法</span><span class="sxs-lookup"><span data-stu-id="8b671-108">Methods</span></span>
|<span data-ttu-id="8b671-109">方法</span><span class="sxs-lookup"><span data-stu-id="8b671-109">Method</span></span>|<span data-ttu-id="8b671-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8b671-110">Return Type</span></span>|<span data-ttu-id="8b671-111">说明</span><span class="sxs-lookup"><span data-stu-id="8b671-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8b671-112">列出 targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="8b671-112">List targetedManagedAppPolicyAssignments</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|<span data-ttu-id="8b671-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8b671-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="8b671-114">列出 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8b671-114">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="8b671-115">获取 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8b671-115">Get targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[<span data-ttu-id="8b671-116">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8b671-116">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="8b671-117">读取 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8b671-117">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="8b671-118">删除 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8b671-118">Delete targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|<span data-ttu-id="8b671-119">无</span><span class="sxs-lookup"><span data-stu-id="8b671-119">None</span></span>|<span data-ttu-id="8b671-120">删除 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="8b671-120">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>|
|[<span data-ttu-id="8b671-121">更新 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8b671-121">Update targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[<span data-ttu-id="8b671-122">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8b671-122">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="8b671-123">更新 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8b671-123">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8b671-124">属性</span><span class="sxs-lookup"><span data-stu-id="8b671-124">Properties</span></span>
|<span data-ttu-id="8b671-125">属性</span><span class="sxs-lookup"><span data-stu-id="8b671-125">Property</span></span>|<span data-ttu-id="8b671-126">类型</span><span class="sxs-lookup"><span data-stu-id="8b671-126">Type</span></span>|<span data-ttu-id="8b671-127">说明</span><span class="sxs-lookup"><span data-stu-id="8b671-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b671-128">id</span><span class="sxs-lookup"><span data-stu-id="8b671-128">id</span></span>|<span data-ttu-id="8b671-129">String</span><span class="sxs-lookup"><span data-stu-id="8b671-129">String</span></span>|<span data-ttu-id="8b671-130">Id</span><span class="sxs-lookup"><span data-stu-id="8b671-130">Id</span></span>|
|<span data-ttu-id="8b671-131">target</span><span class="sxs-lookup"><span data-stu-id="8b671-131">target</span></span>|[<span data-ttu-id="8b671-132">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8b671-132">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8b671-133">组或应用的部署标识符</span><span class="sxs-lookup"><span data-stu-id="8b671-133">Identifier for deployment of a group or app</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b671-134">关系</span><span class="sxs-lookup"><span data-stu-id="8b671-134">Relationships</span></span>
<span data-ttu-id="8b671-135">无</span><span class="sxs-lookup"><span data-stu-id="8b671-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b671-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b671-136">JSON Representation</span></span>
<span data-ttu-id="8b671-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b671-137">Here is a JSON representation of the resource.</span></span>
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




