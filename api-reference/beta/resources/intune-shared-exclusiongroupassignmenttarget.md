---
title: exclusionGroupAssignmentTarget 资源类型
description: 表示应从赋值中排除的组。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6d8973a8974c15c9243d901d65a3d5dd9dbe1a54
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010467"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="9fbb5-103">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="9fbb5-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="9fbb5-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9fbb5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fbb5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9fbb5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fbb5-106">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="9fbb5-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="9fbb5-107">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="9fbb5-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9fbb5-108">属性</span><span class="sxs-lookup"><span data-stu-id="9fbb5-108">Properties</span></span>
|<span data-ttu-id="9fbb5-109">属性</span><span class="sxs-lookup"><span data-stu-id="9fbb5-109">Property</span></span>|<span data-ttu-id="9fbb5-110">类型</span><span class="sxs-lookup"><span data-stu-id="9fbb5-110">Type</span></span>|<span data-ttu-id="9fbb5-111">说明</span><span class="sxs-lookup"><span data-stu-id="9fbb5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fbb5-112">groupId</span><span class="sxs-lookup"><span data-stu-id="9fbb5-112">groupId</span></span>|<span data-ttu-id="9fbb5-113">String</span><span class="sxs-lookup"><span data-stu-id="9fbb5-113">String</span></span>|<span data-ttu-id="9fbb5-114">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="9fbb5-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="9fbb5-115">继承自 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="9fbb5-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fbb5-116">关系</span><span class="sxs-lookup"><span data-stu-id="9fbb5-116">Relationships</span></span>
<span data-ttu-id="9fbb5-117">无</span><span class="sxs-lookup"><span data-stu-id="9fbb5-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fbb5-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9fbb5-118">JSON Representation</span></span>
<span data-ttu-id="9fbb5-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fbb5-119">Here is a JSON representation of the resource.</span></span>
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





