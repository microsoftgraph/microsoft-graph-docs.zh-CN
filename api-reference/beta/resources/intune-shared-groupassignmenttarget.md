---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8ede502c06ffcaef4f3d9be2f133ea6eb591d5de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084280"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="e6ee5-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6ee5-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="e6ee5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6ee5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6ee5-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e6ee5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6ee5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6ee5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6ee5-107">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="e6ee5-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="e6ee5-108">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e6ee5-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e6ee5-109">属性</span><span class="sxs-lookup"><span data-stu-id="e6ee5-109">Properties</span></span>
|<span data-ttu-id="e6ee5-110">属性</span><span class="sxs-lookup"><span data-stu-id="e6ee5-110">Property</span></span>|<span data-ttu-id="e6ee5-111">类型</span><span class="sxs-lookup"><span data-stu-id="e6ee5-111">Type</span></span>|<span data-ttu-id="e6ee5-112">说明</span><span class="sxs-lookup"><span data-stu-id="e6ee5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6ee5-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="e6ee5-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="e6ee5-114">字符串</span><span class="sxs-lookup"><span data-stu-id="e6ee5-114">String</span></span>|<span data-ttu-id="e6ee5-115">目标工作分配的筛选器的 Id。</span><span class="sxs-lookup"><span data-stu-id="e6ee5-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="e6ee5-116">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e6ee5-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="e6ee5-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="e6ee5-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="e6ee5-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="e6ee5-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="e6ee5-119">目标工作分配的筛选器类型，即 Exclude 或 Include。</span><span class="sxs-lookup"><span data-stu-id="e6ee5-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="e6ee5-120">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)。</span><span class="sxs-lookup"><span data-stu-id="e6ee5-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="e6ee5-121">可取值为：`none`、`include`。</span><span class="sxs-lookup"><span data-stu-id="e6ee5-121">Possible values are: `none`, `include`.</span></span>|
|<span data-ttu-id="e6ee5-122">groupId</span><span class="sxs-lookup"><span data-stu-id="e6ee5-122">groupId</span></span>|<span data-ttu-id="e6ee5-123">String</span><span class="sxs-lookup"><span data-stu-id="e6ee5-123">String</span></span>|<span data-ttu-id="e6ee5-124">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="e6ee5-124">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6ee5-125">关系</span><span class="sxs-lookup"><span data-stu-id="e6ee5-125">Relationships</span></span>
<span data-ttu-id="e6ee5-126">无</span><span class="sxs-lookup"><span data-stu-id="e6ee5-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6ee5-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6ee5-127">JSON Representation</span></span>
<span data-ttu-id="e6ee5-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6ee5-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String",
  "groupId": "String"
}
```






