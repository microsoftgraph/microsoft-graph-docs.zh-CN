---
title: groupAssignmentTarget 资源类型
description: 表示组的赋值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e30bde3c36346fe1938b245174f971bddddebe20
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938623"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="0bc47-103">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="0bc47-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="0bc47-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0bc47-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bc47-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0bc47-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bc47-106">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="0bc47-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="0bc47-107">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="0bc47-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0bc47-108">属性</span><span class="sxs-lookup"><span data-stu-id="0bc47-108">Properties</span></span>
|<span data-ttu-id="0bc47-109">属性</span><span class="sxs-lookup"><span data-stu-id="0bc47-109">Property</span></span>|<span data-ttu-id="0bc47-110">类型</span><span class="sxs-lookup"><span data-stu-id="0bc47-110">Type</span></span>|<span data-ttu-id="0bc47-111">说明</span><span class="sxs-lookup"><span data-stu-id="0bc47-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bc47-112">groupId</span><span class="sxs-lookup"><span data-stu-id="0bc47-112">groupId</span></span>|<span data-ttu-id="0bc47-113">String</span><span class="sxs-lookup"><span data-stu-id="0bc47-113">String</span></span>|<span data-ttu-id="0bc47-114">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="0bc47-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bc47-115">关系</span><span class="sxs-lookup"><span data-stu-id="0bc47-115">Relationships</span></span>
<span data-ttu-id="0bc47-116">无</span><span class="sxs-lookup"><span data-stu-id="0bc47-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bc47-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0bc47-117">JSON Representation</span></span>
<span data-ttu-id="0bc47-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0bc47-118">Here is a JSON representation of the resource.</span></span>
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




