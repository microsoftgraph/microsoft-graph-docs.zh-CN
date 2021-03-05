---
title: locationConstraintItem 资源类型
description: 客户端声明的会议地点条件。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 00aa2852744904a57fe3e90303cf562346c478a3
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472042"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="abc9b-103">locationConstraintItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="abc9b-103">locationConstraintItem resource type</span></span>

<span data-ttu-id="abc9b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abc9b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abc9b-105">客户端声明的会议地点条件。</span><span class="sxs-lookup"><span data-stu-id="abc9b-105">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="abc9b-106">由 [location](location.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="abc9b-106">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="abc9b-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="abc9b-107">JSON representation</span></span>

<span data-ttu-id="abc9b-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abc9b-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="abc9b-109">属性</span><span class="sxs-lookup"><span data-stu-id="abc9b-109">Properties</span></span>
| <span data-ttu-id="abc9b-110">属性</span><span class="sxs-lookup"><span data-stu-id="abc9b-110">Property</span></span>     | <span data-ttu-id="abc9b-111">类型</span><span class="sxs-lookup"><span data-stu-id="abc9b-111">Type</span></span>   |<span data-ttu-id="abc9b-112">说明</span><span class="sxs-lookup"><span data-stu-id="abc9b-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="abc9b-113">address</span><span class="sxs-lookup"><span data-stu-id="abc9b-113">address</span></span> | [<span data-ttu-id="abc9b-114">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="abc9b-114">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="abc9b-115">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="abc9b-115">The street address of the location.</span></span> |
| <span data-ttu-id="abc9b-116">coordinates</span><span class="sxs-lookup"><span data-stu-id="abc9b-116">coordinates</span></span> | [<span data-ttu-id="abc9b-117">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="abc9b-117">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="abc9b-118">地理坐标和位置的海拔高度。</span><span class="sxs-lookup"><span data-stu-id="abc9b-118">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="abc9b-119">displayName</span><span class="sxs-lookup"><span data-stu-id="abc9b-119">displayName</span></span>  | <span data-ttu-id="abc9b-120">String</span><span class="sxs-lookup"><span data-stu-id="abc9b-120">String</span></span> | <span data-ttu-id="abc9b-121">与地点相关联的名称。</span><span class="sxs-lookup"><span data-stu-id="abc9b-121">The name associated with the location.</span></span>                       |
| <span data-ttu-id="abc9b-122">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="abc9b-122">locationEmailAddress</span></span> | <span data-ttu-id="abc9b-123">String</span><span class="sxs-lookup"><span data-stu-id="abc9b-123">String</span></span> | <span data-ttu-id="abc9b-124">（可选）与位置相关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="abc9b-124">Optional email address of the location.</span></span> |
| <span data-ttu-id="abc9b-125">locationType</span><span class="sxs-lookup"><span data-stu-id="abc9b-125">locationType</span></span> | <span data-ttu-id="abc9b-126">locationType</span><span class="sxs-lookup"><span data-stu-id="abc9b-126">locationType</span></span> | <span data-ttu-id="abc9b-127">位置的类型。</span><span class="sxs-lookup"><span data-stu-id="abc9b-127">The type of location.</span></span> <span data-ttu-id="abc9b-128">可取值为：`default`、`conferenceRoom`、`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress`。</span><span class="sxs-lookup"><span data-stu-id="abc9b-128">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="abc9b-129">只读。</span><span class="sxs-lookup"><span data-stu-id="abc9b-129">Read-only.</span></span>|
| <span data-ttu-id="abc9b-130">locationUri</span><span class="sxs-lookup"><span data-stu-id="abc9b-130">locationUri</span></span> | <span data-ttu-id="abc9b-131">String</span><span class="sxs-lookup"><span data-stu-id="abc9b-131">String</span></span> | <span data-ttu-id="abc9b-132">（可选）表示位置的 URI。</span><span class="sxs-lookup"><span data-stu-id="abc9b-132">Optional URI representing the location.</span></span> |
| <span data-ttu-id="abc9b-133">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="abc9b-133">resolveAvailability</span></span> | <span data-ttu-id="abc9b-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="abc9b-134">Boolean</span></span> | <span data-ttu-id="abc9b-p102">如果设为 true，且指定的资源处于忙碌状态，[findMeetingTimes](../api/user-findmeetingtimes.md) 会查找另一空闲资源。如果设为 false，且指定的资源处于忙碌状态，**findMeetingTimes** 会返回用户缓存中排名最靠前的资源，而不会检查其是否空闲。默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="abc9b-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |
| <span data-ttu-id="abc9b-138">uniqueId</span><span class="sxs-lookup"><span data-stu-id="abc9b-138">uniqueId</span></span> | <span data-ttu-id="abc9b-139">String</span><span class="sxs-lookup"><span data-stu-id="abc9b-139">String</span></span> | <span data-ttu-id="abc9b-140">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="abc9b-140">For internal use only.</span></span>|
| <span data-ttu-id="abc9b-141">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="abc9b-141">uniqueIdType</span></span> | <span data-ttu-id="abc9b-142">String</span><span class="sxs-lookup"><span data-stu-id="abc9b-142">String</span></span> | <span data-ttu-id="abc9b-143">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="abc9b-143">For internal use only.</span></span> |

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


