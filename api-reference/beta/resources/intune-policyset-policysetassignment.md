---
title: policySetAssignment 资源类型
description: 包含用于 PolicySet 分配的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 620a7f92d1105a0eb5d17d27dfa2f5455944be37
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527600"
---
# <a name="policysetassignment-resource-type"></a><span data-ttu-id="bb0c4-103">policySetAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb0c4-103">policySetAssignment resource type</span></span>

<span data-ttu-id="bb0c4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="bb0c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb0c4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb0c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb0c4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb0c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb0c4-107">包含用于 PolicySet 分配的属性的类。</span><span class="sxs-lookup"><span data-stu-id="bb0c4-107">A class containing the properties used for PolicySet Assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="bb0c4-108">方法</span><span class="sxs-lookup"><span data-stu-id="bb0c4-108">Methods</span></span>
|<span data-ttu-id="bb0c4-109">方法</span><span class="sxs-lookup"><span data-stu-id="bb0c4-109">Method</span></span>|<span data-ttu-id="bb0c4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="bb0c4-110">Return Type</span></span>|<span data-ttu-id="bb0c4-111">说明</span><span class="sxs-lookup"><span data-stu-id="bb0c4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb0c4-112">列出 policySetAssignments</span><span class="sxs-lookup"><span data-stu-id="bb0c4-112">List policySetAssignments</span></span>](../api/intune-policyset-policysetassignment-list.md)|<span data-ttu-id="bb0c4-113">[policySetAssignment](../resources/intune-policyset-policysetassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="bb0c4-113">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="bb0c4-114">列出[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb0c4-114">List properties and relationships of the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) objects.</span></span>|
|[<span data-ttu-id="bb0c4-115">获取 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="bb0c4-115">Get policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-get.md)|[<span data-ttu-id="bb0c4-116">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="bb0c4-116">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="bb0c4-117">读取[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb0c4-117">Read properties and relationships of the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|
|[<span data-ttu-id="bb0c4-118">创建 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="bb0c4-118">Create policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-create.md)|[<span data-ttu-id="bb0c4-119">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="bb0c4-119">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="bb0c4-120">创建新的[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bb0c4-120">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|
|[<span data-ttu-id="bb0c4-121">删除 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="bb0c4-121">Delete policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-delete.md)|<span data-ttu-id="bb0c4-122">无</span><span class="sxs-lookup"><span data-stu-id="bb0c4-122">None</span></span>|<span data-ttu-id="bb0c4-123">删除[policySetAssignment](../resources/intune-policyset-policysetassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="bb0c4-123">Deletes a [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span></span>|
|[<span data-ttu-id="bb0c4-124">更新 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="bb0c4-124">Update policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-update.md)|[<span data-ttu-id="bb0c4-125">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="bb0c4-125">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="bb0c4-126">更新[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bb0c4-126">Update the properties of a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb0c4-127">属性</span><span class="sxs-lookup"><span data-stu-id="bb0c4-127">Properties</span></span>
|<span data-ttu-id="bb0c4-128">属性</span><span class="sxs-lookup"><span data-stu-id="bb0c4-128">Property</span></span>|<span data-ttu-id="bb0c4-129">类型</span><span class="sxs-lookup"><span data-stu-id="bb0c4-129">Type</span></span>|<span data-ttu-id="bb0c4-130">说明</span><span class="sxs-lookup"><span data-stu-id="bb0c4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb0c4-131">id</span><span class="sxs-lookup"><span data-stu-id="bb0c4-131">id</span></span>|<span data-ttu-id="bb0c4-132">String</span><span class="sxs-lookup"><span data-stu-id="bb0c4-132">String</span></span>|<span data-ttu-id="bb0c4-133">PolicySetAssignment 的键。</span><span class="sxs-lookup"><span data-stu-id="bb0c4-133">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="bb0c4-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb0c4-134">lastModifiedDateTime</span></span>|<span data-ttu-id="bb0c4-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb0c4-135">DateTimeOffset</span></span>|<span data-ttu-id="bb0c4-136">PolicySetAssignment 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="bb0c4-136">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="bb0c4-137">target</span><span class="sxs-lookup"><span data-stu-id="bb0c4-137">target</span></span>|[<span data-ttu-id="bb0c4-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bb0c4-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bb0c4-139">PolicySetAssignment 的目标组</span><span class="sxs-lookup"><span data-stu-id="bb0c4-139">The target group of PolicySetAssignment</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb0c4-140">关系</span><span class="sxs-lookup"><span data-stu-id="bb0c4-140">Relationships</span></span>
<span data-ttu-id="bb0c4-141">无</span><span class="sxs-lookup"><span data-stu-id="bb0c4-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb0c4-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb0c4-142">JSON Representation</span></span>
<span data-ttu-id="bb0c4-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb0c4-143">Here is a JSON representation of the resource.</span></span>
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



