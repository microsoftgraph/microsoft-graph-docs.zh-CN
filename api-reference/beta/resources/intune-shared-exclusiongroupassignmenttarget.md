---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6c92cbad6b9c09de3dc8e468ddcec9d2035cb254
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408050"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="fb29e-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb29e-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="fb29e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb29e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb29e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fb29e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb29e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb29e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb29e-107">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="fb29e-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="fb29e-108">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="fb29e-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fb29e-109">属性</span><span class="sxs-lookup"><span data-stu-id="fb29e-109">Properties</span></span>
|<span data-ttu-id="fb29e-110">属性</span><span class="sxs-lookup"><span data-stu-id="fb29e-110">Property</span></span>|<span data-ttu-id="fb29e-111">类型</span><span class="sxs-lookup"><span data-stu-id="fb29e-111">Type</span></span>|<span data-ttu-id="fb29e-112">说明</span><span class="sxs-lookup"><span data-stu-id="fb29e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb29e-113">groupId</span><span class="sxs-lookup"><span data-stu-id="fb29e-113">groupId</span></span>|<span data-ttu-id="fb29e-114">String</span><span class="sxs-lookup"><span data-stu-id="fb29e-114">String</span></span>|<span data-ttu-id="fb29e-115">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="fb29e-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="fb29e-116">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="fb29e-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb29e-117">关系</span><span class="sxs-lookup"><span data-stu-id="fb29e-117">Relationships</span></span>
<span data-ttu-id="fb29e-118">无</span><span class="sxs-lookup"><span data-stu-id="fb29e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb29e-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb29e-119">JSON Representation</span></span>
<span data-ttu-id="fb29e-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb29e-120">Here is a JSON representation of the resource.</span></span>
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



