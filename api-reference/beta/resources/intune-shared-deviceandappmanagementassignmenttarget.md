---
title: deviceAndAppManagementAssignmentTarget 资源类型
description: 赋值目标的基类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3a4e45685acffb6523bfc7dc77cebbff4796530
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707582"
---
# <a name="deviceandappmanagementassignmenttarget-resource-type"></a><span data-ttu-id="9cea7-103">deviceAndAppManagementAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="9cea7-103">deviceAndAppManagementAssignmentTarget resource type</span></span>

<span data-ttu-id="9cea7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cea7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9cea7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9cea7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cea7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9cea7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cea7-107">赋值目标的基类型。</span><span class="sxs-lookup"><span data-stu-id="9cea7-107">Base type for assignment targets.</span></span>

## <a name="properties"></a><span data-ttu-id="9cea7-108">属性</span><span class="sxs-lookup"><span data-stu-id="9cea7-108">Properties</span></span>
|<span data-ttu-id="9cea7-109">属性</span><span class="sxs-lookup"><span data-stu-id="9cea7-109">Property</span></span>|<span data-ttu-id="9cea7-110">类型</span><span class="sxs-lookup"><span data-stu-id="9cea7-110">Type</span></span>|<span data-ttu-id="9cea7-111">说明</span><span class="sxs-lookup"><span data-stu-id="9cea7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cea7-112">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="9cea7-112">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="9cea7-113">String</span><span class="sxs-lookup"><span data-stu-id="9cea7-113">String</span></span>|<span data-ttu-id="9cea7-114">目标工作分配的筛选器的 Id。</span><span class="sxs-lookup"><span data-stu-id="9cea7-114">The Id of the filter for the target assignment.</span></span>|
|<span data-ttu-id="9cea7-115">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="9cea7-115">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="9cea7-116">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="9cea7-116">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="9cea7-117">目标工作分配的筛选器类型，即 Exclude 或 Include。</span><span class="sxs-lookup"><span data-stu-id="9cea7-117">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="9cea7-118">可取值为：`none`、`include`。</span><span class="sxs-lookup"><span data-stu-id="9cea7-118">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cea7-119">关系</span><span class="sxs-lookup"><span data-stu-id="9cea7-119">Relationships</span></span>
<span data-ttu-id="9cea7-120">无</span><span class="sxs-lookup"><span data-stu-id="9cea7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9cea7-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9cea7-121">JSON Representation</span></span>
<span data-ttu-id="9cea7-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9cea7-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String"
}
```





