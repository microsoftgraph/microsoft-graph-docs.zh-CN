---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 00e3fecab48e0c34e500dd7b3d9e7c114de0c8d8
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612204"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="6e761-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="6e761-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="6e761-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e761-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e761-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6e761-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e761-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e761-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e761-107">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="6e761-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="6e761-108">继承自 [groupAssignmentTarget](../resources/intune-devices-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="6e761-108">Inherits from [groupAssignmentTarget](../resources/intune-devices-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6e761-109">属性</span><span class="sxs-lookup"><span data-stu-id="6e761-109">Properties</span></span>
|<span data-ttu-id="6e761-110">属性</span><span class="sxs-lookup"><span data-stu-id="6e761-110">Property</span></span>|<span data-ttu-id="6e761-111">类型</span><span class="sxs-lookup"><span data-stu-id="6e761-111">Type</span></span>|<span data-ttu-id="6e761-112">Description</span><span class="sxs-lookup"><span data-stu-id="6e761-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e761-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="6e761-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="6e761-114">String</span><span class="sxs-lookup"><span data-stu-id="6e761-114">String</span></span>|<span data-ttu-id="6e761-115">目标分配的筛选器 ID。</span><span class="sxs-lookup"><span data-stu-id="6e761-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="6e761-116">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="6e761-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="6e761-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="6e761-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="6e761-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="6e761-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-devices-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="6e761-119">目标分配的筛选器类型，即排除或包含。</span><span class="sxs-lookup"><span data-stu-id="6e761-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="6e761-120">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)。</span><span class="sxs-lookup"><span data-stu-id="6e761-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="6e761-121">可取值为：`none`、`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="6e761-121">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="6e761-122">groupId</span><span class="sxs-lookup"><span data-stu-id="6e761-122">groupId</span></span>|<span data-ttu-id="6e761-123">String</span><span class="sxs-lookup"><span data-stu-id="6e761-123">String</span></span>|<span data-ttu-id="6e761-124">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="6e761-124">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="6e761-125">继承自 [groupAssignmentTarget](../resources/intune-devices-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="6e761-125">Inherited from [groupAssignmentTarget](../resources/intune-devices-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e761-126">关系</span><span class="sxs-lookup"><span data-stu-id="6e761-126">Relationships</span></span>
<span data-ttu-id="6e761-127">无</span><span class="sxs-lookup"><span data-stu-id="6e761-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e761-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6e761-128">JSON Representation</span></span>
<span data-ttu-id="6e761-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e761-129">Here is a JSON representation of the resource.</span></span>
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




