---
title: targetedManagedAppPolicyAssignment 资源类型
description: 组或应用的部署类型。
ms.openlocfilehash: 8bbd93835a673aab8d621218d9bcf975d94d0c95
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049038"
---
# <a name="targetedmanagedapppolicyassignment-resource-type"></a><span data-ttu-id="7323f-103">targetedManagedAppPolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="7323f-103">targetedManagedAppPolicyAssignment resource type</span></span>

> <span data-ttu-id="7323f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7323f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7323f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7323f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7323f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7323f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7323f-107">组或应用的部署类型。</span><span class="sxs-lookup"><span data-stu-id="7323f-107">The type for deployment of groups or apps.</span></span>
## <a name="methods"></a><span data-ttu-id="7323f-108">方法</span><span class="sxs-lookup"><span data-stu-id="7323f-108">Methods</span></span>
|<span data-ttu-id="7323f-109">方法</span><span class="sxs-lookup"><span data-stu-id="7323f-109">Method</span></span>|<span data-ttu-id="7323f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7323f-110">Return Type</span></span>|<span data-ttu-id="7323f-111">说明</span><span class="sxs-lookup"><span data-stu-id="7323f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7323f-112">列出 targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="7323f-112">List targetedManagedAppPolicyAssignments</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-list.md)|<span data-ttu-id="7323f-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7323f-113">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="7323f-114">列出 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7323f-114">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="7323f-115">获取 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="7323f-115">Get targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-get.md)|[<span data-ttu-id="7323f-116">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="7323f-116">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="7323f-117">读取 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7323f-117">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="7323f-118">删除 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="7323f-118">Delete targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-delete.md)|<span data-ttu-id="7323f-119">无</span><span class="sxs-lookup"><span data-stu-id="7323f-119">None</span></span>|<span data-ttu-id="7323f-120">删除 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="7323f-120">Deletes a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>|
|[<span data-ttu-id="7323f-121">更新 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="7323f-121">Update targetedManagedAppPolicyAssignment</span></span>](../api/intune-mam-targetedmanagedapppolicyassignment-update.md)|[<span data-ttu-id="7323f-122">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="7323f-122">targetedManagedAppPolicyAssignment</span></span>](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|<span data-ttu-id="7323f-123">更新 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7323f-123">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7323f-124">属性</span><span class="sxs-lookup"><span data-stu-id="7323f-124">Properties</span></span>
|<span data-ttu-id="7323f-125">属性</span><span class="sxs-lookup"><span data-stu-id="7323f-125">Property</span></span>|<span data-ttu-id="7323f-126">类型</span><span class="sxs-lookup"><span data-stu-id="7323f-126">Type</span></span>|<span data-ttu-id="7323f-127">说明</span><span class="sxs-lookup"><span data-stu-id="7323f-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7323f-128">id</span><span class="sxs-lookup"><span data-stu-id="7323f-128">id</span></span>|<span data-ttu-id="7323f-129">String</span><span class="sxs-lookup"><span data-stu-id="7323f-129">String</span></span>|<span data-ttu-id="7323f-130">Id</span><span class="sxs-lookup"><span data-stu-id="7323f-130">Id</span></span>|
|<span data-ttu-id="7323f-131">target</span><span class="sxs-lookup"><span data-stu-id="7323f-131">target</span></span>|[<span data-ttu-id="7323f-132">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7323f-132">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7323f-133">组或应用的部署标识符</span><span class="sxs-lookup"><span data-stu-id="7323f-133">Identifier for deployment of a group or app</span></span>|

## <a name="relationships"></a><span data-ttu-id="7323f-134">关系</span><span class="sxs-lookup"><span data-stu-id="7323f-134">Relationships</span></span>
<span data-ttu-id="7323f-135">无</span><span class="sxs-lookup"><span data-stu-id="7323f-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7323f-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7323f-136">JSON Representation</span></span>
<span data-ttu-id="7323f-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7323f-137">Here is a JSON representation of the resource.</span></span>
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





