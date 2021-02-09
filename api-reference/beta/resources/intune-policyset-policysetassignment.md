---
title: policySetAssignment 资源类型
description: 一个包含用于 PolicySet Assignment 的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da5049ecfbfd7f6516c77b1aa662cc35d648b13c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158420"
---
# <a name="policysetassignment-resource-type"></a><span data-ttu-id="6709c-103">policySetAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="6709c-103">policySetAssignment resource type</span></span>

<span data-ttu-id="6709c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6709c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6709c-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6709c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6709c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6709c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6709c-107">一个包含用于 PolicySet Assignment 的属性的类。</span><span class="sxs-lookup"><span data-stu-id="6709c-107">A class containing the properties used for PolicySet Assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="6709c-108">方法</span><span class="sxs-lookup"><span data-stu-id="6709c-108">Methods</span></span>
|<span data-ttu-id="6709c-109">方法</span><span class="sxs-lookup"><span data-stu-id="6709c-109">Method</span></span>|<span data-ttu-id="6709c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6709c-110">Return Type</span></span>|<span data-ttu-id="6709c-111">说明</span><span class="sxs-lookup"><span data-stu-id="6709c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6709c-112">列出 policySetAssignments</span><span class="sxs-lookup"><span data-stu-id="6709c-112">List policySetAssignments</span></span>](../api/intune-policyset-policysetassignment-list.md)|<span data-ttu-id="6709c-113">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6709c-113">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="6709c-114">列出 [policySetAssignment 对象的属性和](../resources/intune-policyset-policysetassignment.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="6709c-114">List properties and relationships of the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) objects.</span></span>|
|[<span data-ttu-id="6709c-115">获取 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="6709c-115">Get policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-get.md)|[<span data-ttu-id="6709c-116">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="6709c-116">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="6709c-117">读取 [policySetAssignment 对象的属性和](../resources/intune-policyset-policysetassignment.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="6709c-117">Read properties and relationships of the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|
|[<span data-ttu-id="6709c-118">创建 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="6709c-118">Create policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-create.md)|[<span data-ttu-id="6709c-119">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="6709c-119">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="6709c-120">创建新的 [policySetAssignment](../resources/intune-policyset-policysetassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6709c-120">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|
|[<span data-ttu-id="6709c-121">删除 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="6709c-121">Delete policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-delete.md)|<span data-ttu-id="6709c-122">无</span><span class="sxs-lookup"><span data-stu-id="6709c-122">None</span></span>|<span data-ttu-id="6709c-123">删除 [policySetAssignment](../resources/intune-policyset-policysetassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="6709c-123">Deletes a [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span></span>|
|[<span data-ttu-id="6709c-124">更新 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="6709c-124">Update policySetAssignment</span></span>](../api/intune-policyset-policysetassignment-update.md)|[<span data-ttu-id="6709c-125">policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="6709c-125">policySetAssignment</span></span>](../resources/intune-policyset-policysetassignment.md)|<span data-ttu-id="6709c-126">更新 [policySetAssignment 对象](../resources/intune-policyset-policysetassignment.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="6709c-126">Update the properties of a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6709c-127">属性</span><span class="sxs-lookup"><span data-stu-id="6709c-127">Properties</span></span>
|<span data-ttu-id="6709c-128">属性</span><span class="sxs-lookup"><span data-stu-id="6709c-128">Property</span></span>|<span data-ttu-id="6709c-129">类型</span><span class="sxs-lookup"><span data-stu-id="6709c-129">Type</span></span>|<span data-ttu-id="6709c-130">说明</span><span class="sxs-lookup"><span data-stu-id="6709c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6709c-131">id</span><span class="sxs-lookup"><span data-stu-id="6709c-131">id</span></span>|<span data-ttu-id="6709c-132">String</span><span class="sxs-lookup"><span data-stu-id="6709c-132">String</span></span>|<span data-ttu-id="6709c-133">PolicySetAssignment 的键。</span><span class="sxs-lookup"><span data-stu-id="6709c-133">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="6709c-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6709c-134">lastModifiedDateTime</span></span>|<span data-ttu-id="6709c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6709c-135">DateTimeOffset</span></span>|<span data-ttu-id="6709c-136">PolicySetAssignment 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="6709c-136">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="6709c-137">target</span><span class="sxs-lookup"><span data-stu-id="6709c-137">target</span></span>|[<span data-ttu-id="6709c-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6709c-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6709c-139">PolicySetAssignment 的目标组</span><span class="sxs-lookup"><span data-stu-id="6709c-139">The target group of PolicySetAssignment</span></span>|

## <a name="relationships"></a><span data-ttu-id="6709c-140">关系</span><span class="sxs-lookup"><span data-stu-id="6709c-140">Relationships</span></span>
<span data-ttu-id="6709c-141">无</span><span class="sxs-lookup"><span data-stu-id="6709c-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6709c-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6709c-142">JSON Representation</span></span>
<span data-ttu-id="6709c-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6709c-143">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




