---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 437d4c8ab11a0cf095e58b56b271aecb9e42729c
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612203"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="6f6e1-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f6e1-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="6f6e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f6e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f6e1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f6e1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f6e1-107">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="6f6e1-108">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="6f6e1-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6f6e1-109">属性</span><span class="sxs-lookup"><span data-stu-id="6f6e1-109">Properties</span></span>
|<span data-ttu-id="6f6e1-110">属性</span><span class="sxs-lookup"><span data-stu-id="6f6e1-110">Property</span></span>|<span data-ttu-id="6f6e1-111">类型</span><span class="sxs-lookup"><span data-stu-id="6f6e1-111">Type</span></span>|<span data-ttu-id="6f6e1-112">Description</span><span class="sxs-lookup"><span data-stu-id="6f6e1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f6e1-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="6f6e1-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="6f6e1-114">String</span><span class="sxs-lookup"><span data-stu-id="6f6e1-114">String</span></span>|<span data-ttu-id="6f6e1-115">目标分配的筛选器 ID。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="6f6e1-116">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="6f6e1-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="6f6e1-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="6f6e1-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="6f6e1-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="6f6e1-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-devices-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="6f6e1-119">目标分配的筛选器类型，即排除或包含。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="6f6e1-120">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="6f6e1-121">可取值为：`none`、`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-121">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="6f6e1-122">groupId</span><span class="sxs-lookup"><span data-stu-id="6f6e1-122">groupId</span></span>|<span data-ttu-id="6f6e1-123">String</span><span class="sxs-lookup"><span data-stu-id="6f6e1-123">String</span></span>|<span data-ttu-id="6f6e1-124">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-124">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f6e1-125">关系</span><span class="sxs-lookup"><span data-stu-id="6f6e1-125">Relationships</span></span>
<span data-ttu-id="6f6e1-126">无</span><span class="sxs-lookup"><span data-stu-id="6f6e1-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f6e1-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f6e1-127">JSON Representation</span></span>
<span data-ttu-id="6f6e1-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-128">Here is a JSON representation of the resource.</span></span>
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




