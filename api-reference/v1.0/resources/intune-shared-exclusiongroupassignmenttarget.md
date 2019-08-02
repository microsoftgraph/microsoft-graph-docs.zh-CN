---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 805f2f1dbcab8751d564fbde3f6747b6e77f6d09
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036923"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="0b65d-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b65d-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="0b65d-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b65d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b65d-105">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="0b65d-105">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="0b65d-106">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="0b65d-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0b65d-107">属性</span><span class="sxs-lookup"><span data-stu-id="0b65d-107">Properties</span></span>
|<span data-ttu-id="0b65d-108">属性</span><span class="sxs-lookup"><span data-stu-id="0b65d-108">Property</span></span>|<span data-ttu-id="0b65d-109">类型</span><span class="sxs-lookup"><span data-stu-id="0b65d-109">Type</span></span>|<span data-ttu-id="0b65d-110">说明</span><span class="sxs-lookup"><span data-stu-id="0b65d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b65d-111">groupId</span><span class="sxs-lookup"><span data-stu-id="0b65d-111">groupId</span></span>|<span data-ttu-id="0b65d-112">String</span><span class="sxs-lookup"><span data-stu-id="0b65d-112">String</span></span>|<span data-ttu-id="0b65d-113">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="0b65d-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="0b65d-114">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="0b65d-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b65d-115">关系</span><span class="sxs-lookup"><span data-stu-id="0b65d-115">Relationships</span></span>
<span data-ttu-id="0b65d-116">无</span><span class="sxs-lookup"><span data-stu-id="0b65d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b65d-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b65d-117">JSON Representation</span></span>
<span data-ttu-id="0b65d-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b65d-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```



