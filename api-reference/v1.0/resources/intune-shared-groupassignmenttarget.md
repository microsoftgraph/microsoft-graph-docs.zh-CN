---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7e4b97dd24c053af9aa65739e3c8a6db45044969
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354012"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="19f55-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="19f55-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="19f55-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19f55-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19f55-105">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="19f55-105">Represents an assignment to a group.</span></span>


<span data-ttu-id="19f55-106">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="19f55-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="19f55-107">属性</span><span class="sxs-lookup"><span data-stu-id="19f55-107">Properties</span></span>
|<span data-ttu-id="19f55-108">属性</span><span class="sxs-lookup"><span data-stu-id="19f55-108">Property</span></span>|<span data-ttu-id="19f55-109">类型</span><span class="sxs-lookup"><span data-stu-id="19f55-109">Type</span></span>|<span data-ttu-id="19f55-110">说明</span><span class="sxs-lookup"><span data-stu-id="19f55-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19f55-111">groupId</span><span class="sxs-lookup"><span data-stu-id="19f55-111">groupId</span></span>|<span data-ttu-id="19f55-112">String</span><span class="sxs-lookup"><span data-stu-id="19f55-112">String</span></span>|<span data-ttu-id="19f55-113">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="19f55-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19f55-114">关系</span><span class="sxs-lookup"><span data-stu-id="19f55-114">Relationships</span></span>
<span data-ttu-id="19f55-115">无</span><span class="sxs-lookup"><span data-stu-id="19f55-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19f55-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19f55-116">JSON Representation</span></span>
<span data-ttu-id="19f55-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19f55-117">Here is a JSON representation of the resource.</span></span>
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




