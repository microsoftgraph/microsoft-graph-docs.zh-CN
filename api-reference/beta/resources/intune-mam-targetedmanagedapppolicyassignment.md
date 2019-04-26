---
title: targetedManagedAppPolicyAssignment 资源类型
description: 组或应用的部署类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ced81e320608e34fba6d4b2b96b101f61aebaa59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553902"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a><span data-ttu-id="8535f-103">targetedManagedAppPolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="8535f-103">targetedManagedAppPolicyAssignment resource type</span></span>

> <span data-ttu-id="8535f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8535f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8535f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8535f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8535f-106">组或应用的部署类型。</span><span class="sxs-lookup"><span data-stu-id="8535f-106">The type for deployment of groups or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="8535f-107">方法</span><span class="sxs-lookup"><span data-stu-id="8535f-107">Methods</span></span>
|<span data-ttu-id="8535f-108">方法</span><span class="sxs-lookup"><span data-stu-id="8535f-108">Method</span></span>|<span data-ttu-id="8535f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8535f-109">Return Type</span></span>|<span data-ttu-id="8535f-110">说明</span><span class="sxs-lookup"><span data-stu-id="8535f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8535f-111">列出 targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="8535f-111">List targetedManagedAppPolicyAssignments</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|<span data-ttu-id="8535f-112">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8535f-112">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="8535f-113">列出 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8535f-113">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="8535f-114">获取 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8535f-114">Get targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[<span data-ttu-id="8535f-115">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8535f-115">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="8535f-116">读取 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8535f-116">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="8535f-117">删除 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8535f-117">Delete targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|<span data-ttu-id="8535f-118">无</span><span class="sxs-lookup"><span data-stu-id="8535f-118">None</span></span>|<span data-ttu-id="8535f-119">删除 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="8535f-119">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>|
|[<span data-ttu-id="8535f-120">更新 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8535f-120">Update targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[<span data-ttu-id="8535f-121">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8535f-121">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="8535f-122">更新 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8535f-122">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8535f-123">属性</span><span class="sxs-lookup"><span data-stu-id="8535f-123">Properties</span></span>
|<span data-ttu-id="8535f-124">属性</span><span class="sxs-lookup"><span data-stu-id="8535f-124">Property</span></span>|<span data-ttu-id="8535f-125">类型</span><span class="sxs-lookup"><span data-stu-id="8535f-125">Type</span></span>|<span data-ttu-id="8535f-126">说明</span><span class="sxs-lookup"><span data-stu-id="8535f-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8535f-127">id</span><span class="sxs-lookup"><span data-stu-id="8535f-127">id</span></span>|<span data-ttu-id="8535f-128">String</span><span class="sxs-lookup"><span data-stu-id="8535f-128">String</span></span>|<span data-ttu-id="8535f-129">Id</span><span class="sxs-lookup"><span data-stu-id="8535f-129">Id</span></span>|
|<span data-ttu-id="8535f-130">target</span><span class="sxs-lookup"><span data-stu-id="8535f-130">target</span></span>|[<span data-ttu-id="8535f-131">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8535f-131">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8535f-132">组或应用的部署标识符</span><span class="sxs-lookup"><span data-stu-id="8535f-132">Identifier for deployment of a group or app</span></span>|

## <a name="relationships"></a><span data-ttu-id="8535f-133">关系</span><span class="sxs-lookup"><span data-stu-id="8535f-133">Relationships</span></span>
<span data-ttu-id="8535f-134">无</span><span class="sxs-lookup"><span data-stu-id="8535f-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8535f-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8535f-135">JSON Representation</span></span>
<span data-ttu-id="8535f-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8535f-136">Here is a JSON representation of the resource.</span></span>
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





