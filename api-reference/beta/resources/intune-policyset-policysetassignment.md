---
title: policySetAssignment 资源类型
description: 包含用于 PolicySet 分配的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 480e05dafdf4d10ab500271c44b4dd3421877a0c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199958"
---
# <a name="policysetassignment-resource-type"></a><span data-ttu-id="baceb-103">policySetAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="baceb-103">policySetAssignment resource type</span></span>

> <span data-ttu-id="baceb-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="baceb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="baceb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="baceb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baceb-106">包含用于 PolicySet 分配的属性的类。</span><span class="sxs-lookup"><span data-stu-id="baceb-106">A class containing the properties used for PolicySet Assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="baceb-107">方法</span><span class="sxs-lookup"><span data-stu-id="baceb-107">Methods</span></span>
|<span data-ttu-id="baceb-108">方法</span><span class="sxs-lookup"><span data-stu-id="baceb-108">Method</span></span>|<span data-ttu-id="baceb-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="baceb-109">Return Type</span></span>|<span data-ttu-id="baceb-110">说明</span><span class="sxs-lookup"><span data-stu-id="baceb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="baceb-111">列出 policySetAssignments</span><span class="sxs-lookup"><span data-stu-id="baceb-111">List policySetAssignments</span></span>](../api/intune-policyset-policysetassignment-list.md)|<span data-ttu-id="baceb-112">[policySetAssignment](../resources/intune-policyset-policysetassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="baceb-112">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="baceb-113">列出[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="baceb-113">List properties and relationships of the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) objects.</span></span>|
|[<span data-ttu-id="baceb-114">获取 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="baceb-114">Get policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-get.md)|[<span data-ttu-id="baceb-115">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="baceb-115">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="baceb-116">读取[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="baceb-116">Read properties and relationships of the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|
|[<span data-ttu-id="baceb-117">创建 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="baceb-117">Create policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-create.md)|[<span data-ttu-id="baceb-118">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="baceb-118">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="baceb-119">创建新的[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="baceb-119">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|
|[<span data-ttu-id="baceb-120">删除 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="baceb-120">Delete policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-delete.md)|<span data-ttu-id="baceb-121">无</span><span class="sxs-lookup"><span data-stu-id="baceb-121">None</span></span>|<span data-ttu-id="baceb-122">删除[policySetAssignment](../resources/intune-policyset-policysetassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="baceb-122">Deletes a [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span></span>|
|[<span data-ttu-id="baceb-123">更新 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="baceb-123">Update policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-update.md)|[<span data-ttu-id="baceb-124">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="baceb-124">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="baceb-125">更新[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="baceb-125">Update the properties of a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="baceb-126">属性</span><span class="sxs-lookup"><span data-stu-id="baceb-126">Properties</span></span>
|<span data-ttu-id="baceb-127">属性</span><span class="sxs-lookup"><span data-stu-id="baceb-127">Property</span></span>|<span data-ttu-id="baceb-128">类型</span><span class="sxs-lookup"><span data-stu-id="baceb-128">Type</span></span>|<span data-ttu-id="baceb-129">说明</span><span class="sxs-lookup"><span data-stu-id="baceb-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baceb-130">id</span><span class="sxs-lookup"><span data-stu-id="baceb-130">id</span></span>|<span data-ttu-id="baceb-131">String</span><span class="sxs-lookup"><span data-stu-id="baceb-131">String</span></span>|<span data-ttu-id="baceb-132">PolicySetAssignment 的键。</span><span class="sxs-lookup"><span data-stu-id="baceb-132">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="baceb-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="baceb-133">lastModifiedDateTime</span></span>|<span data-ttu-id="baceb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baceb-134">DateTimeOffset</span></span>|<span data-ttu-id="baceb-135">PolicySetAssignment 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="baceb-135">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="baceb-136">target</span><span class="sxs-lookup"><span data-stu-id="baceb-136">target</span></span>|[<span data-ttu-id="baceb-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="baceb-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="baceb-138">PolicySetAssignment 的目标组</span><span class="sxs-lookup"><span data-stu-id="baceb-138">The target group of PolicySetAssignment</span></span>|

## <a name="relationships"></a><span data-ttu-id="baceb-139">关系</span><span class="sxs-lookup"><span data-stu-id="baceb-139">Relationships</span></span>
<span data-ttu-id="baceb-140">无</span><span class="sxs-lookup"><span data-stu-id="baceb-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="baceb-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="baceb-141">JSON Representation</span></span>
<span data-ttu-id="baceb-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="baceb-142">Here is a JSON representation of the resource.</span></span>
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



