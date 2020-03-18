---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d2484d601de3c200cfe300a77245e873502ecc0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42770121"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="92384-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="92384-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="92384-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="92384-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92384-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92384-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92384-106">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="92384-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="92384-107">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="92384-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92384-108">属性</span><span class="sxs-lookup"><span data-stu-id="92384-108">Properties</span></span>
|<span data-ttu-id="92384-109">属性</span><span class="sxs-lookup"><span data-stu-id="92384-109">Property</span></span>|<span data-ttu-id="92384-110">类型</span><span class="sxs-lookup"><span data-stu-id="92384-110">Type</span></span>|<span data-ttu-id="92384-111">说明</span><span class="sxs-lookup"><span data-stu-id="92384-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92384-112">groupId</span><span class="sxs-lookup"><span data-stu-id="92384-112">groupId</span></span>|<span data-ttu-id="92384-113">String</span><span class="sxs-lookup"><span data-stu-id="92384-113">String</span></span>|<span data-ttu-id="92384-114">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="92384-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="92384-115">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="92384-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="92384-116">关系</span><span class="sxs-lookup"><span data-stu-id="92384-116">Relationships</span></span>
<span data-ttu-id="92384-117">无</span><span class="sxs-lookup"><span data-stu-id="92384-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92384-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92384-118">JSON Representation</span></span>
<span data-ttu-id="92384-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92384-119">Here is a JSON representation of the resource.</span></span>
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



