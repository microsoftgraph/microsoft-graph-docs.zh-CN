---
title: locationConstraintItem 资源类型
description: 客户端声明的会议地点条件。
ms.openlocfilehash: 4f985a5d37dc3a27866f077b68250b07b4a173f4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010469"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="5017f-103">locationConstraintItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="5017f-103">locationConstraintItem resource type</span></span>

<span data-ttu-id="5017f-104">客户端声明的会议地点条件。</span><span class="sxs-lookup"><span data-stu-id="5017f-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="5017f-105">由 [location](location.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="5017f-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="5017f-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5017f-106">JSON representation</span></span>

<span data-ttu-id="5017f-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5017f-107">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.location",
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```
## <a name="properties"></a><span data-ttu-id="5017f-108">属性</span><span class="sxs-lookup"><span data-stu-id="5017f-108">Properties</span></span>
| <span data-ttu-id="5017f-109">属性</span><span class="sxs-lookup"><span data-stu-id="5017f-109">Property</span></span>     | <span data-ttu-id="5017f-110">类型</span><span class="sxs-lookup"><span data-stu-id="5017f-110">Type</span></span>   |<span data-ttu-id="5017f-111">说明</span><span class="sxs-lookup"><span data-stu-id="5017f-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5017f-112">address</span><span class="sxs-lookup"><span data-stu-id="5017f-112">address</span></span> | [<span data-ttu-id="5017f-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="5017f-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="5017f-114">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="5017f-114">The street address of the location.</span></span> |
| <span data-ttu-id="5017f-115">displayName</span><span class="sxs-lookup"><span data-stu-id="5017f-115">displayName</span></span>  | <span data-ttu-id="5017f-116">String</span><span class="sxs-lookup"><span data-stu-id="5017f-116">String</span></span> | <span data-ttu-id="5017f-117">与地点相关联的名称。</span><span class="sxs-lookup"><span data-stu-id="5017f-117">The name associated with the location.</span></span>                       |
| <span data-ttu-id="5017f-118">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="5017f-118">locationEmailAddress</span></span> | <span data-ttu-id="5017f-119">String</span><span class="sxs-lookup"><span data-stu-id="5017f-119">String</span></span> | <span data-ttu-id="5017f-120">（可选）与地点相关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5017f-120">Optional email address of the location.</span></span> |
| <span data-ttu-id="5017f-121">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="5017f-121">resolveAvailability</span></span> | <span data-ttu-id="5017f-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="5017f-122">Boolean</span></span> | <span data-ttu-id="5017f-p101">如果设为 true，且指定的资源处于忙碌状态，[findMeetingTimes](../api/user-findmeetingtimes.md) 会查找另一空闲资源。如果设为 false，且指定的资源处于忙碌状态，**findMeetingTimes** 会返回用户缓存中排名最靠前的资源，而不会检查其是否空闲。默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="5017f-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->