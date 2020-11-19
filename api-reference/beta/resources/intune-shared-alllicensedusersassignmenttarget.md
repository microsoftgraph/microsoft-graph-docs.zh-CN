---
title: allLicensedUsersAssignmentTarget 资源类型
description: 表示租户中所有许可用户的赋值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c9d799aeb602f1b06c7429e8c69483a238a059ad
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49300876"
---
# <a name="alllicensedusersassignmenttarget-resource-type"></a><span data-ttu-id="e7d60-103">allLicensedUsersAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7d60-103">allLicensedUsersAssignmentTarget resource type</span></span>

<span data-ttu-id="e7d60-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7d60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7d60-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e7d60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7d60-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e7d60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7d60-107">表示租户中所有许可用户的赋值。</span><span class="sxs-lookup"><span data-stu-id="e7d60-107">Represents an assignment to all licensed users in the tenant.</span></span>


<span data-ttu-id="e7d60-108">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e7d60-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e7d60-109">属性</span><span class="sxs-lookup"><span data-stu-id="e7d60-109">Properties</span></span>
|<span data-ttu-id="e7d60-110">属性</span><span class="sxs-lookup"><span data-stu-id="e7d60-110">Property</span></span>|<span data-ttu-id="e7d60-111">类型</span><span class="sxs-lookup"><span data-stu-id="e7d60-111">Type</span></span>|<span data-ttu-id="e7d60-112">Description</span><span class="sxs-lookup"><span data-stu-id="e7d60-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7d60-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="e7d60-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="e7d60-114">字符串</span><span class="sxs-lookup"><span data-stu-id="e7d60-114">String</span></span>|<span data-ttu-id="e7d60-115">目标工作分配的筛选器的 Id。</span><span class="sxs-lookup"><span data-stu-id="e7d60-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="e7d60-116">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e7d60-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="e7d60-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="e7d60-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="e7d60-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="e7d60-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="e7d60-119">目标工作分配的筛选器类型，即 Exclude 或 Include。</span><span class="sxs-lookup"><span data-stu-id="e7d60-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="e7d60-120">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)。</span><span class="sxs-lookup"><span data-stu-id="e7d60-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="e7d60-121">可取值为：`none`、`include`。</span><span class="sxs-lookup"><span data-stu-id="e7d60-121">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7d60-122">关系</span><span class="sxs-lookup"><span data-stu-id="e7d60-122">Relationships</span></span>
<span data-ttu-id="e7d60-123">无</span><span class="sxs-lookup"><span data-stu-id="e7d60-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7d60-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7d60-124">JSON Representation</span></span>
<span data-ttu-id="e7d60-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7d60-125">Here is a JSON representation of the resource.</span></span>
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




