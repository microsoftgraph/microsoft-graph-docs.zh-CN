---
title: allDevicesAssignmentTarget 资源类型
description: 表示租户中所有托管设备的赋值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ca3d3b4dbbe534189c66eba09ecbc6e99258936
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612188"
---
# <a name="alldevicesassignmenttarget-resource-type"></a><span data-ttu-id="1b8af-103">allDevicesAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b8af-103">allDevicesAssignmentTarget resource type</span></span>

<span data-ttu-id="1b8af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b8af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b8af-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1b8af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b8af-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b8af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b8af-107">表示租户中所有托管设备的赋值。</span><span class="sxs-lookup"><span data-stu-id="1b8af-107">Represents an assignment to all managed devices in the tenant.</span></span>


<span data-ttu-id="1b8af-108">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="1b8af-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1b8af-109">属性</span><span class="sxs-lookup"><span data-stu-id="1b8af-109">Properties</span></span>
|<span data-ttu-id="1b8af-110">属性</span><span class="sxs-lookup"><span data-stu-id="1b8af-110">Property</span></span>|<span data-ttu-id="1b8af-111">类型</span><span class="sxs-lookup"><span data-stu-id="1b8af-111">Type</span></span>|<span data-ttu-id="1b8af-112">Description</span><span class="sxs-lookup"><span data-stu-id="1b8af-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b8af-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="1b8af-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="1b8af-114">String</span><span class="sxs-lookup"><span data-stu-id="1b8af-114">String</span></span>|<span data-ttu-id="1b8af-115">目标分配的筛选器 ID。</span><span class="sxs-lookup"><span data-stu-id="1b8af-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="1b8af-116">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="1b8af-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="1b8af-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="1b8af-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="1b8af-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="1b8af-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-devices-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="1b8af-119">目标分配的筛选器类型，即排除或包含。</span><span class="sxs-lookup"><span data-stu-id="1b8af-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="1b8af-120">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)。</span><span class="sxs-lookup"><span data-stu-id="1b8af-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="1b8af-121">可取值为：`none`、`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="1b8af-121">Possible values are: `none`, `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b8af-122">关系</span><span class="sxs-lookup"><span data-stu-id="1b8af-122">Relationships</span></span>
<span data-ttu-id="1b8af-123">无</span><span class="sxs-lookup"><span data-stu-id="1b8af-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b8af-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b8af-124">JSON Representation</span></span>
<span data-ttu-id="1b8af-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b8af-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.allDevicesAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String"
}
```




