---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 05a19fa1dc93cad93e88f421c1bba11ec602ba33
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793435"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="43246-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="43246-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="43246-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43246-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43246-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="43246-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43246-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43246-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43246-107">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="43246-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="43246-108">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="43246-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="43246-109">属性</span><span class="sxs-lookup"><span data-stu-id="43246-109">Properties</span></span>
|<span data-ttu-id="43246-110">属性</span><span class="sxs-lookup"><span data-stu-id="43246-110">Property</span></span>|<span data-ttu-id="43246-111">类型</span><span class="sxs-lookup"><span data-stu-id="43246-111">Type</span></span>|<span data-ttu-id="43246-112">说明</span><span class="sxs-lookup"><span data-stu-id="43246-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43246-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="43246-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="43246-114">String</span><span class="sxs-lookup"><span data-stu-id="43246-114">String</span></span>|<span data-ttu-id="43246-115">目标工作分配的筛选器的 Id。</span><span class="sxs-lookup"><span data-stu-id="43246-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="43246-116">继承自[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="43246-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="43246-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="43246-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="43246-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="43246-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="43246-119">目标工作分配的筛选器类型，即 Exclude 或 Include。</span><span class="sxs-lookup"><span data-stu-id="43246-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="43246-120">继承自[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)。</span><span class="sxs-lookup"><span data-stu-id="43246-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="43246-121">可取值为：`none`、`include`。</span><span class="sxs-lookup"><span data-stu-id="43246-121">Possible values are: `none`, `include`.</span></span>|
|<span data-ttu-id="43246-122">groupId</span><span class="sxs-lookup"><span data-stu-id="43246-122">groupId</span></span>|<span data-ttu-id="43246-123">String</span><span class="sxs-lookup"><span data-stu-id="43246-123">String</span></span>|<span data-ttu-id="43246-124">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="43246-124">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="43246-125">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="43246-125">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="43246-126">关系</span><span class="sxs-lookup"><span data-stu-id="43246-126">Relationships</span></span>
<span data-ttu-id="43246-127">无</span><span class="sxs-lookup"><span data-stu-id="43246-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43246-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43246-128">JSON Representation</span></span>
<span data-ttu-id="43246-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43246-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String",
  "groupId": "String"
}
```



