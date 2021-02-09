---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0dda74257a3596ad72470806cdcc4f169fd935d9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157510"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="a1079-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1079-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="a1079-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1079-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1079-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1079-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1079-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1079-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1079-107">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="a1079-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="a1079-108">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="a1079-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a1079-109">属性</span><span class="sxs-lookup"><span data-stu-id="a1079-109">Properties</span></span>
|<span data-ttu-id="a1079-110">属性</span><span class="sxs-lookup"><span data-stu-id="a1079-110">Property</span></span>|<span data-ttu-id="a1079-111">类型</span><span class="sxs-lookup"><span data-stu-id="a1079-111">Type</span></span>|<span data-ttu-id="a1079-112">说明</span><span class="sxs-lookup"><span data-stu-id="a1079-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1079-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="a1079-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="a1079-114">String</span><span class="sxs-lookup"><span data-stu-id="a1079-114">String</span></span>|<span data-ttu-id="a1079-115">目标分配的筛选器的 ID。</span><span class="sxs-lookup"><span data-stu-id="a1079-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="a1079-116">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="a1079-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="a1079-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="a1079-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="a1079-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="a1079-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="a1079-119">目标分配的筛选器类型，即排除或包含。</span><span class="sxs-lookup"><span data-stu-id="a1079-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="a1079-120">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)。</span><span class="sxs-lookup"><span data-stu-id="a1079-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="a1079-121">可取值为：`none`、`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="a1079-121">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="a1079-122">groupId</span><span class="sxs-lookup"><span data-stu-id="a1079-122">groupId</span></span>|<span data-ttu-id="a1079-123">String</span><span class="sxs-lookup"><span data-stu-id="a1079-123">String</span></span>|<span data-ttu-id="a1079-124">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="a1079-124">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1079-125">关系</span><span class="sxs-lookup"><span data-stu-id="a1079-125">Relationships</span></span>
<span data-ttu-id="a1079-126">无</span><span class="sxs-lookup"><span data-stu-id="a1079-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1079-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1079-127">JSON Representation</span></span>
<span data-ttu-id="a1079-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1079-128">Here is a JSON representation of the resource.</span></span>
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




