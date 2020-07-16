---
title: allLicensedUsersAssignmentTarget 资源类型
description: 表示租户中所有许可用户的赋值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4388710e079366193f2a2ca7bd842a2d7b5763cf
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793596"
---
# <a name="alllicensedusersassignmenttarget-resource-type"></a><span data-ttu-id="e2582-103">allLicensedUsersAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2582-103">allLicensedUsersAssignmentTarget resource type</span></span>

<span data-ttu-id="e2582-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2582-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2582-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e2582-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2582-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2582-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2582-107">表示租户中所有许可用户的赋值。</span><span class="sxs-lookup"><span data-stu-id="e2582-107">Represents an assignment to all licensed users in the tenant.</span></span>


<span data-ttu-id="e2582-108">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e2582-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e2582-109">属性</span><span class="sxs-lookup"><span data-stu-id="e2582-109">Properties</span></span>
|<span data-ttu-id="e2582-110">属性</span><span class="sxs-lookup"><span data-stu-id="e2582-110">Property</span></span>|<span data-ttu-id="e2582-111">类型</span><span class="sxs-lookup"><span data-stu-id="e2582-111">Type</span></span>|<span data-ttu-id="e2582-112">说明</span><span class="sxs-lookup"><span data-stu-id="e2582-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2582-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="e2582-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="e2582-114">String</span><span class="sxs-lookup"><span data-stu-id="e2582-114">String</span></span>|<span data-ttu-id="e2582-115">目标工作分配的筛选器的 Id。</span><span class="sxs-lookup"><span data-stu-id="e2582-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="e2582-116">继承自[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e2582-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="e2582-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="e2582-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="e2582-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="e2582-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="e2582-119">目标工作分配的筛选器类型，即 Exclude 或 Include。</span><span class="sxs-lookup"><span data-stu-id="e2582-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="e2582-120">继承自[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)。</span><span class="sxs-lookup"><span data-stu-id="e2582-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="e2582-121">可取值为：`none`、`include`。</span><span class="sxs-lookup"><span data-stu-id="e2582-121">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2582-122">关系</span><span class="sxs-lookup"><span data-stu-id="e2582-122">Relationships</span></span>
<span data-ttu-id="e2582-123">无</span><span class="sxs-lookup"><span data-stu-id="e2582-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2582-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2582-124">JSON Representation</span></span>
<span data-ttu-id="e2582-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2582-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.allLicensedUsersAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String"
}
```



