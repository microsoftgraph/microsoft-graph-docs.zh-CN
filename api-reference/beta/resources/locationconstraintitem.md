---
title: locationConstraintItem 资源类型
description: 客户端声明的会议地点条件。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ecc29f65cf8296250c3daceddc8b7b5ca1a88381
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345223"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="e2b32-103">locationConstraintItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2b32-103">locationConstraintItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2b32-104">客户端声明的会议地点条件。</span><span class="sxs-lookup"><span data-stu-id="e2b32-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="e2b32-105">由 [location](location.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="e2b32-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2b32-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2b32-106">JSON representation</span></span>

<span data-ttu-id="e2b32-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2b32-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  
  ],
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationType": "string",
  "locationUri": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```
## <a name="properties"></a><span data-ttu-id="e2b32-108">属性</span><span class="sxs-lookup"><span data-stu-id="e2b32-108">Properties</span></span>
| <span data-ttu-id="e2b32-109">属性</span><span class="sxs-lookup"><span data-stu-id="e2b32-109">Property</span></span>     | <span data-ttu-id="e2b32-110">类型</span><span class="sxs-lookup"><span data-stu-id="e2b32-110">Type</span></span>   |<span data-ttu-id="e2b32-111">说明</span><span class="sxs-lookup"><span data-stu-id="e2b32-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2b32-112">address</span><span class="sxs-lookup"><span data-stu-id="e2b32-112">address</span></span> | [<span data-ttu-id="e2b32-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="e2b32-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="e2b32-114">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="e2b32-114">The street address of the location.</span></span> |
| <span data-ttu-id="e2b32-115">coordinates</span><span class="sxs-lookup"><span data-stu-id="e2b32-115">coordinates</span></span> | [<span data-ttu-id="e2b32-116">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="e2b32-116">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="e2b32-117">地理坐标和位置的海拔高度。</span><span class="sxs-lookup"><span data-stu-id="e2b32-117">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="e2b32-118">displayName</span><span class="sxs-lookup"><span data-stu-id="e2b32-118">displayName</span></span>  | <span data-ttu-id="e2b32-119">String</span><span class="sxs-lookup"><span data-stu-id="e2b32-119">String</span></span> | <span data-ttu-id="e2b32-120">与地点相关联的名称。</span><span class="sxs-lookup"><span data-stu-id="e2b32-120">The name associated with the location.</span></span>                       |
| <span data-ttu-id="e2b32-121">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e2b32-121">locationEmailAddress</span></span> | <span data-ttu-id="e2b32-122">String</span><span class="sxs-lookup"><span data-stu-id="e2b32-122">String</span></span> | <span data-ttu-id="e2b32-123">（可选）与位置相关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="e2b32-123">Optional email address of the location.</span></span> |
| <span data-ttu-id="e2b32-124">locationType</span><span class="sxs-lookup"><span data-stu-id="e2b32-124">locationType</span></span> | <span data-ttu-id="e2b32-125">locationType</span><span class="sxs-lookup"><span data-stu-id="e2b32-125">locationType</span></span> | <span data-ttu-id="e2b32-126">位置的类型。</span><span class="sxs-lookup"><span data-stu-id="e2b32-126">The type of location.</span></span> <span data-ttu-id="e2b32-127">可取值为：`default`、`conferenceRoom`、`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress`。</span><span class="sxs-lookup"><span data-stu-id="e2b32-127">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="e2b32-128">只读。</span><span class="sxs-lookup"><span data-stu-id="e2b32-128">Read-only.</span></span>|
| <span data-ttu-id="e2b32-129">locationUri</span><span class="sxs-lookup"><span data-stu-id="e2b32-129">locationUri</span></span> | <span data-ttu-id="e2b32-130">String</span><span class="sxs-lookup"><span data-stu-id="e2b32-130">String</span></span> | <span data-ttu-id="e2b32-131">（可选）表示位置的 URI。</span><span class="sxs-lookup"><span data-stu-id="e2b32-131">Optional URI representing the location.</span></span> |
| <span data-ttu-id="e2b32-132">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="e2b32-132">resolveAvailability</span></span> | <span data-ttu-id="e2b32-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b32-133">Boolean</span></span> | <span data-ttu-id="e2b32-p102">如果设为 true，且指定的资源处于忙碌状态，[findMeetingTimes](../api/user-findmeetingtimes.md) 会查找另一空闲资源。如果设为 false，且指定的资源处于忙碌状态，**findMeetingTimes** 会返回用户缓存中排名最靠前的资源，而不会检查其是否空闲。默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="e2b32-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |
| <span data-ttu-id="e2b32-137">uniqueId</span><span class="sxs-lookup"><span data-stu-id="e2b32-137">uniqueId</span></span> | <span data-ttu-id="e2b32-138">String</span><span class="sxs-lookup"><span data-stu-id="e2b32-138">String</span></span> | <span data-ttu-id="e2b32-139">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="e2b32-139">For internal use only.</span></span>|
| <span data-ttu-id="e2b32-140">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="e2b32-140">uniqueIdType</span></span> | <span data-ttu-id="e2b32-141">String</span><span class="sxs-lookup"><span data-stu-id="e2b32-141">String</span></span> | <span data-ttu-id="e2b32-142">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="e2b32-142">For internal use only.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
