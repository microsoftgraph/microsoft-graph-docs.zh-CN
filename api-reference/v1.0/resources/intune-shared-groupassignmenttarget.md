---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24ac3c4519cc074c3cce423ca5d0745c8a78d865
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250171"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="f2943-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2943-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="f2943-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f2943-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2943-105">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="f2943-105">Represents an assignment to a group.</span></span>


<span data-ttu-id="f2943-106">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="f2943-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f2943-107">属性</span><span class="sxs-lookup"><span data-stu-id="f2943-107">Properties</span></span>
|<span data-ttu-id="f2943-108">属性</span><span class="sxs-lookup"><span data-stu-id="f2943-108">Property</span></span>|<span data-ttu-id="f2943-109">类型</span><span class="sxs-lookup"><span data-stu-id="f2943-109">Type</span></span>|<span data-ttu-id="f2943-110">说明</span><span class="sxs-lookup"><span data-stu-id="f2943-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2943-111">groupId</span><span class="sxs-lookup"><span data-stu-id="f2943-111">groupId</span></span>|<span data-ttu-id="f2943-112">String</span><span class="sxs-lookup"><span data-stu-id="f2943-112">String</span></span>|<span data-ttu-id="f2943-113">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="f2943-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2943-114">关系</span><span class="sxs-lookup"><span data-stu-id="f2943-114">Relationships</span></span>
<span data-ttu-id="f2943-115">无</span><span class="sxs-lookup"><span data-stu-id="f2943-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2943-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2943-116">JSON Representation</span></span>
<span data-ttu-id="f2943-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2943-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```



