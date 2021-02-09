---
title: allLicensedUsersAssignmentTarget 资源类型
description: 表示租户中所有许可用户的赋值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f4e05236b0782d74547204bab30d7957aeb52ca
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158413"
---
# <a name="alllicensedusersassignmenttarget-resource-type"></a><span data-ttu-id="5988c-103">allLicensedUsersAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="5988c-103">allLicensedUsersAssignmentTarget resource type</span></span>

<span data-ttu-id="5988c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5988c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5988c-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5988c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5988c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5988c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5988c-107">表示租户中所有许可用户的赋值。</span><span class="sxs-lookup"><span data-stu-id="5988c-107">Represents an assignment to all licensed users in the tenant.</span></span>


<span data-ttu-id="5988c-108">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="5988c-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5988c-109">属性</span><span class="sxs-lookup"><span data-stu-id="5988c-109">Properties</span></span>
|<span data-ttu-id="5988c-110">属性</span><span class="sxs-lookup"><span data-stu-id="5988c-110">Property</span></span>|<span data-ttu-id="5988c-111">类型</span><span class="sxs-lookup"><span data-stu-id="5988c-111">Type</span></span>|<span data-ttu-id="5988c-112">说明</span><span class="sxs-lookup"><span data-stu-id="5988c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5988c-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="5988c-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="5988c-114">String</span><span class="sxs-lookup"><span data-stu-id="5988c-114">String</span></span>|<span data-ttu-id="5988c-115">目标分配的筛选器的 ID。</span><span class="sxs-lookup"><span data-stu-id="5988c-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="5988c-116">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="5988c-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="5988c-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="5988c-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="5988c-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="5988c-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="5988c-119">目标分配的筛选器类型，即排除或包含。</span><span class="sxs-lookup"><span data-stu-id="5988c-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="5988c-120">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)。</span><span class="sxs-lookup"><span data-stu-id="5988c-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="5988c-121">可取值为：`none`、`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="5988c-121">Possible values are: `none`, `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5988c-122">关系</span><span class="sxs-lookup"><span data-stu-id="5988c-122">Relationships</span></span>
<span data-ttu-id="5988c-123">无</span><span class="sxs-lookup"><span data-stu-id="5988c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5988c-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5988c-124">JSON Representation</span></span>
<span data-ttu-id="5988c-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5988c-125">Here is a JSON representation of the resource.</span></span>
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




