---
title: policySetAssignment 资源类型
description: 包含用于 PolicySet 分配的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 14789c8c57b766dae61dfc467514ba6d095b764f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463365"
---
# <a name="policysetassignment-resource-type"></a><span data-ttu-id="790c9-103">policySetAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="790c9-103">policySetAssignment resource type</span></span>

<span data-ttu-id="790c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="790c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="790c9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="790c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="790c9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="790c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="790c9-107">包含用于 PolicySet 分配的属性的类。</span><span class="sxs-lookup"><span data-stu-id="790c9-107">A class containing the properties used for PolicySet Assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="790c9-108">方法</span><span class="sxs-lookup"><span data-stu-id="790c9-108">Methods</span></span>
|<span data-ttu-id="790c9-109">方法</span><span class="sxs-lookup"><span data-stu-id="790c9-109">Method</span></span>|<span data-ttu-id="790c9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="790c9-110">Return Type</span></span>|<span data-ttu-id="790c9-111">说明</span><span class="sxs-lookup"><span data-stu-id="790c9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="790c9-112">列出 policySetAssignments</span><span class="sxs-lookup"><span data-stu-id="790c9-112">List policySetAssignments</span></span>](../api/intune-policyset-policysetassignment-list.md)|<span data-ttu-id="790c9-113">[policySetAssignment](../resources/intune-policyset-policysetassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="790c9-113">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="790c9-114">列出[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="790c9-114">List properties and relationships of the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) objects.</span></span>|
|[<span data-ttu-id="790c9-115">获取 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="790c9-115">Get policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-get.md)|[<span data-ttu-id="790c9-116">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="790c9-116">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="790c9-117">读取[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="790c9-117">Read properties and relationships of the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|
|[<span data-ttu-id="790c9-118">创建 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="790c9-118">Create policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-create.md)|[<span data-ttu-id="790c9-119">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="790c9-119">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="790c9-120">创建新的[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="790c9-120">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|
|[<span data-ttu-id="790c9-121">删除 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="790c9-121">Delete policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-delete.md)|<span data-ttu-id="790c9-122">无</span><span class="sxs-lookup"><span data-stu-id="790c9-122">None</span></span>|<span data-ttu-id="790c9-123">删除[policySetAssignment](../resources/intune-policyset-policysetassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="790c9-123">Deletes a [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span></span>|
|[<span data-ttu-id="790c9-124">更新 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="790c9-124">Update policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-update.md)|[<span data-ttu-id="790c9-125">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="790c9-125">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="790c9-126">更新[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="790c9-126">Update the properties of a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="790c9-127">属性</span><span class="sxs-lookup"><span data-stu-id="790c9-127">Properties</span></span>
|<span data-ttu-id="790c9-128">属性</span><span class="sxs-lookup"><span data-stu-id="790c9-128">Property</span></span>|<span data-ttu-id="790c9-129">类型</span><span class="sxs-lookup"><span data-stu-id="790c9-129">Type</span></span>|<span data-ttu-id="790c9-130">说明</span><span class="sxs-lookup"><span data-stu-id="790c9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="790c9-131">id</span><span class="sxs-lookup"><span data-stu-id="790c9-131">id</span></span>|<span data-ttu-id="790c9-132">String</span><span class="sxs-lookup"><span data-stu-id="790c9-132">String</span></span>|<span data-ttu-id="790c9-133">PolicySetAssignment 的键。</span><span class="sxs-lookup"><span data-stu-id="790c9-133">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="790c9-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="790c9-134">lastModifiedDateTime</span></span>|<span data-ttu-id="790c9-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="790c9-135">DateTimeOffset</span></span>|<span data-ttu-id="790c9-136">PolicySetAssignment 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="790c9-136">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="790c9-137">target</span><span class="sxs-lookup"><span data-stu-id="790c9-137">target</span></span>|[<span data-ttu-id="790c9-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="790c9-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="790c9-139">PolicySetAssignment 的目标组</span><span class="sxs-lookup"><span data-stu-id="790c9-139">The target group of PolicySetAssignment</span></span>|

## <a name="relationships"></a><span data-ttu-id="790c9-140">关系</span><span class="sxs-lookup"><span data-stu-id="790c9-140">Relationships</span></span>
<span data-ttu-id="790c9-141">无</span><span class="sxs-lookup"><span data-stu-id="790c9-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="790c9-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="790c9-142">JSON Representation</span></span>
<span data-ttu-id="790c9-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="790c9-143">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



