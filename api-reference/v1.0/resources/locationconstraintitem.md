---
title: locationConstraintItem 资源类型
description: 客户端声明的会议地点条件。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 404b0fd380c1161a827fe4610f744d0b9872c92b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447526"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="dc5b0-103">locationConstraintItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc5b0-103">locationConstraintItem resource type</span></span>

<span data-ttu-id="dc5b0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dc5b0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dc5b0-105">客户端声明的会议地点条件。</span><span class="sxs-lookup"><span data-stu-id="dc5b0-105">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="dc5b0-106">由 [location](location.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="dc5b0-106">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc5b0-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc5b0-107">JSON representation</span></span>

<span data-ttu-id="dc5b0-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc5b0-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="dc5b0-109">属性</span><span class="sxs-lookup"><span data-stu-id="dc5b0-109">Properties</span></span>
| <span data-ttu-id="dc5b0-110">属性</span><span class="sxs-lookup"><span data-stu-id="dc5b0-110">Property</span></span>     | <span data-ttu-id="dc5b0-111">类型</span><span class="sxs-lookup"><span data-stu-id="dc5b0-111">Type</span></span>   |<span data-ttu-id="dc5b0-112">说明</span><span class="sxs-lookup"><span data-stu-id="dc5b0-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dc5b0-113">address</span><span class="sxs-lookup"><span data-stu-id="dc5b0-113">address</span></span> | [<span data-ttu-id="dc5b0-114">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="dc5b0-114">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="dc5b0-115">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="dc5b0-115">The street address of the location.</span></span> |
| <span data-ttu-id="dc5b0-116">displayName</span><span class="sxs-lookup"><span data-stu-id="dc5b0-116">displayName</span></span>  | <span data-ttu-id="dc5b0-117">String</span><span class="sxs-lookup"><span data-stu-id="dc5b0-117">String</span></span> | <span data-ttu-id="dc5b0-118">与地点相关联的名称。</span><span class="sxs-lookup"><span data-stu-id="dc5b0-118">The name associated with the location.</span></span>                       |
| <span data-ttu-id="dc5b0-119">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="dc5b0-119">locationEmailAddress</span></span> | <span data-ttu-id="dc5b0-120">String</span><span class="sxs-lookup"><span data-stu-id="dc5b0-120">String</span></span> | <span data-ttu-id="dc5b0-121">（可选）与地点相关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="dc5b0-121">Optional email address of the location.</span></span> |
| <span data-ttu-id="dc5b0-122">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="dc5b0-122">resolveAvailability</span></span> | <span data-ttu-id="dc5b0-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc5b0-123">Boolean</span></span> | <span data-ttu-id="dc5b0-p101">如果设为 true，且指定的资源处于忙碌状态，[findMeetingTimes](../api/user-findmeetingtimes.md) 会查找另一空闲资源。如果设为 false，且指定的资源处于忙碌状态，**findMeetingTimes** 会返回用户缓存中排名最靠前的资源，而不会检查其是否空闲。默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="dc5b0-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
