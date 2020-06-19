---
title: policySetAssignment 资源类型
description: 包含用于 PolicySet 分配的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f7d3ff168f01a7b89c5e7abb46100de0120c677a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793764"
---
# <a name="policysetassignment-resource-type"></a><span data-ttu-id="5c1d2-103">policySetAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c1d2-103">policySetAssignment resource type</span></span>

<span data-ttu-id="5c1d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c1d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c1d2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5c1d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c1d2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c1d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c1d2-107">包含用于 PolicySet 分配的属性的类。</span><span class="sxs-lookup"><span data-stu-id="5c1d2-107">A class containing the properties used for PolicySet Assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="5c1d2-108">Methods</span><span class="sxs-lookup"><span data-stu-id="5c1d2-108">Methods</span></span>
|<span data-ttu-id="5c1d2-109">方法</span><span class="sxs-lookup"><span data-stu-id="5c1d2-109">Method</span></span>|<span data-ttu-id="5c1d2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5c1d2-110">Return Type</span></span>|<span data-ttu-id="5c1d2-111">说明</span><span class="sxs-lookup"><span data-stu-id="5c1d2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5c1d2-112">列出 policySetAssignments</span><span class="sxs-lookup"><span data-stu-id="5c1d2-112">List policySetAssignments</span></span>](../api/intune-policyset-policysetassignment-list.md)|<span data-ttu-id="5c1d2-113">[policySetAssignment](../resources/intune-policyset-policysetassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5c1d2-113">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="5c1d2-114">列出[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5c1d2-114">List properties and relationships of the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) objects.</span></span>|
|[<span data-ttu-id="5c1d2-115">获取 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="5c1d2-115">Get policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-get.md)|[<span data-ttu-id="5c1d2-116">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="5c1d2-116">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="5c1d2-117">读取[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5c1d2-117">Read properties and relationships of the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|
|[<span data-ttu-id="5c1d2-118">创建 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="5c1d2-118">Create policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-create.md)|[<span data-ttu-id="5c1d2-119">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="5c1d2-119">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="5c1d2-120">创建新的[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5c1d2-120">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|
|[<span data-ttu-id="5c1d2-121">删除 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="5c1d2-121">Delete policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-delete.md)|<span data-ttu-id="5c1d2-122">无</span><span class="sxs-lookup"><span data-stu-id="5c1d2-122">None</span></span>|<span data-ttu-id="5c1d2-123">删除[policySetAssignment](../resources/intune-policyset-policysetassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="5c1d2-123">Deletes a [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span></span>|
|[<span data-ttu-id="5c1d2-124">更新 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="5c1d2-124">Update policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-update.md)|[<span data-ttu-id="5c1d2-125">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="5c1d2-125">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="5c1d2-126">更新[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5c1d2-126">Update the properties of a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5c1d2-127">属性</span><span class="sxs-lookup"><span data-stu-id="5c1d2-127">Properties</span></span>
|<span data-ttu-id="5c1d2-128">属性</span><span class="sxs-lookup"><span data-stu-id="5c1d2-128">Property</span></span>|<span data-ttu-id="5c1d2-129">类型</span><span class="sxs-lookup"><span data-stu-id="5c1d2-129">Type</span></span>|<span data-ttu-id="5c1d2-130">说明</span><span class="sxs-lookup"><span data-stu-id="5c1d2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c1d2-131">id</span><span class="sxs-lookup"><span data-stu-id="5c1d2-131">id</span></span>|<span data-ttu-id="5c1d2-132">String</span><span class="sxs-lookup"><span data-stu-id="5c1d2-132">String</span></span>|<span data-ttu-id="5c1d2-133">PolicySetAssignment 的键。</span><span class="sxs-lookup"><span data-stu-id="5c1d2-133">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="5c1d2-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c1d2-134">lastModifiedDateTime</span></span>|<span data-ttu-id="5c1d2-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c1d2-135">DateTimeOffset</span></span>|<span data-ttu-id="5c1d2-136">PolicySetAssignment 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="5c1d2-136">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="5c1d2-137">target</span><span class="sxs-lookup"><span data-stu-id="5c1d2-137">target</span></span>|[<span data-ttu-id="5c1d2-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5c1d2-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5c1d2-139">PolicySetAssignment 的目标组</span><span class="sxs-lookup"><span data-stu-id="5c1d2-139">The target group of PolicySetAssignment</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c1d2-140">关系</span><span class="sxs-lookup"><span data-stu-id="5c1d2-140">Relationships</span></span>
<span data-ttu-id="5c1d2-141">无</span><span class="sxs-lookup"><span data-stu-id="5c1d2-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c1d2-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c1d2-142">JSON Representation</span></span>
<span data-ttu-id="5c1d2-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c1d2-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySetAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```



