---
title: locationConstraintItem 资源类型
description: 客户端声明的会议地点条件。
localization_priority: Normal
ms.openlocfilehash: d9124377172c7598d45b0be9b9f3f9799bd3e1f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874317"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="3bd33-103">locationConstraintItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="3bd33-103">locationConstraintItem resource type</span></span>

<span data-ttu-id="3bd33-104">客户端声明的会议地点条件。</span><span class="sxs-lookup"><span data-stu-id="3bd33-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="3bd33-105">由 [location](location.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="3bd33-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bd33-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3bd33-106">JSON representation</span></span>

<span data-ttu-id="3bd33-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3bd33-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="3bd33-108">属性</span><span class="sxs-lookup"><span data-stu-id="3bd33-108">Properties</span></span>
| <span data-ttu-id="3bd33-109">属性</span><span class="sxs-lookup"><span data-stu-id="3bd33-109">Property</span></span>     | <span data-ttu-id="3bd33-110">类型</span><span class="sxs-lookup"><span data-stu-id="3bd33-110">Type</span></span>   |<span data-ttu-id="3bd33-111">说明</span><span class="sxs-lookup"><span data-stu-id="3bd33-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3bd33-112">address</span><span class="sxs-lookup"><span data-stu-id="3bd33-112">address</span></span> | [<span data-ttu-id="3bd33-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="3bd33-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="3bd33-114">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="3bd33-114">The street address of the location.</span></span> |
| <span data-ttu-id="3bd33-115">displayName</span><span class="sxs-lookup"><span data-stu-id="3bd33-115">displayName</span></span>  | <span data-ttu-id="3bd33-116">String</span><span class="sxs-lookup"><span data-stu-id="3bd33-116">String</span></span> | <span data-ttu-id="3bd33-117">与地点相关联的名称。</span><span class="sxs-lookup"><span data-stu-id="3bd33-117">The name associated with the location.</span></span>                       |
| <span data-ttu-id="3bd33-118">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="3bd33-118">locationEmailAddress</span></span> | <span data-ttu-id="3bd33-119">String</span><span class="sxs-lookup"><span data-stu-id="3bd33-119">String</span></span> | <span data-ttu-id="3bd33-120">（可选）与地点相关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="3bd33-120">Optional email address of the location.</span></span> |
| <span data-ttu-id="3bd33-121">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="3bd33-121">resolveAvailability</span></span> | <span data-ttu-id="3bd33-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bd33-122">Boolean</span></span> | <span data-ttu-id="3bd33-p101">如果设为 true，且指定的资源处于忙碌状态，[findMeetingTimes](../api/user-findmeetingtimes.md) 会查找另一空闲资源。如果设为 false，且指定的资源处于忙碌状态，**findMeetingTimes** 会返回用户缓存中排名最靠前的资源，而不会检查其是否空闲。默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="3bd33-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
