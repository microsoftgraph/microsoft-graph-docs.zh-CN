---
title: deviceAndAppManagementAssignmentTarget 资源类型
description: 赋值目标的基类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ec96f18f16a40182bccfc00efbe70c84568fae33
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158091"
---
# <a name="deviceandappmanagementassignmenttarget-resource-type"></a><span data-ttu-id="3df32-103">deviceAndAppManagementAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="3df32-103">deviceAndAppManagementAssignmentTarget resource type</span></span>

<span data-ttu-id="3df32-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3df32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3df32-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3df32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3df32-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3df32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3df32-107">赋值目标的基类型。</span><span class="sxs-lookup"><span data-stu-id="3df32-107">Base type for assignment targets.</span></span>

## <a name="properties"></a><span data-ttu-id="3df32-108">属性</span><span class="sxs-lookup"><span data-stu-id="3df32-108">Properties</span></span>
|<span data-ttu-id="3df32-109">属性</span><span class="sxs-lookup"><span data-stu-id="3df32-109">Property</span></span>|<span data-ttu-id="3df32-110">类型</span><span class="sxs-lookup"><span data-stu-id="3df32-110">Type</span></span>|<span data-ttu-id="3df32-111">说明</span><span class="sxs-lookup"><span data-stu-id="3df32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3df32-112">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="3df32-112">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="3df32-113">String</span><span class="sxs-lookup"><span data-stu-id="3df32-113">String</span></span>|<span data-ttu-id="3df32-114">目标分配的筛选器的 ID。</span><span class="sxs-lookup"><span data-stu-id="3df32-114">The Id of the filter for the target assignment.</span></span>|
|<span data-ttu-id="3df32-115">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="3df32-115">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="3df32-116">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="3df32-116">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="3df32-117">目标分配的筛选器类型，即排除或包含。</span><span class="sxs-lookup"><span data-stu-id="3df32-117">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="3df32-118">可取值为：`none`、`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="3df32-118">Possible values are: `none`, `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3df32-119">关系</span><span class="sxs-lookup"><span data-stu-id="3df32-119">Relationships</span></span>
<span data-ttu-id="3df32-120">无</span><span class="sxs-lookup"><span data-stu-id="3df32-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3df32-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3df32-121">JSON Representation</span></span>
<span data-ttu-id="3df32-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3df32-122">Here is a JSON representation of the resource.</span></span>
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




