---
title: locationConstraintItem 资源类型
description: 客户端声明的会议地点条件。
localization_priority: Normal
ms.openlocfilehash: 9752b3acec2dd9071e31b743245d662168ecdfd6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508851"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="3d282-103">locationConstraintItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d282-103">locationConstraintItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d282-104">客户端声明的会议地点条件。</span><span class="sxs-lookup"><span data-stu-id="3d282-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="3d282-105">由 [location](location.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="3d282-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d282-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d282-106">JSON representation</span></span>

<span data-ttu-id="3d282-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d282-107">Here is a JSON representation of the resource</span></span>

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
  "locationUri": "string"
}

```
## <a name="properties"></a><span data-ttu-id="3d282-108">属性</span><span class="sxs-lookup"><span data-stu-id="3d282-108">Properties</span></span>
| <span data-ttu-id="3d282-109">属性</span><span class="sxs-lookup"><span data-stu-id="3d282-109">Property</span></span>     | <span data-ttu-id="3d282-110">类型</span><span class="sxs-lookup"><span data-stu-id="3d282-110">Type</span></span>   |<span data-ttu-id="3d282-111">说明</span><span class="sxs-lookup"><span data-stu-id="3d282-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3d282-112">address</span><span class="sxs-lookup"><span data-stu-id="3d282-112">address</span></span> | [<span data-ttu-id="3d282-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="3d282-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="3d282-114">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="3d282-114">The street address of the location.</span></span> |
| <span data-ttu-id="3d282-115">coordinates</span><span class="sxs-lookup"><span data-stu-id="3d282-115">coordinates</span></span> | [<span data-ttu-id="3d282-116">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="3d282-116">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="3d282-117">地理坐标和位置的海拔高度。</span><span class="sxs-lookup"><span data-stu-id="3d282-117">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="3d282-118">displayName</span><span class="sxs-lookup"><span data-stu-id="3d282-118">displayName</span></span>  | <span data-ttu-id="3d282-119">字符串</span><span class="sxs-lookup"><span data-stu-id="3d282-119">String</span></span> | <span data-ttu-id="3d282-120">与地点相关联的名称。</span><span class="sxs-lookup"><span data-stu-id="3d282-120">The name associated with the location.</span></span>                       |
| <span data-ttu-id="3d282-121">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="3d282-121">locationEmailAddress</span></span> | <span data-ttu-id="3d282-122">String</span><span class="sxs-lookup"><span data-stu-id="3d282-122">String</span></span> | <span data-ttu-id="3d282-123">（可选）与位置相关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="3d282-123">Optional email address of the location.</span></span> |
| <span data-ttu-id="3d282-124">locationUri</span><span class="sxs-lookup"><span data-stu-id="3d282-124">locationUri</span></span> | <span data-ttu-id="3d282-125">String</span><span class="sxs-lookup"><span data-stu-id="3d282-125">String</span></span> | <span data-ttu-id="3d282-126">（可选）表示位置的 URI。</span><span class="sxs-lookup"><span data-stu-id="3d282-126">Optional URI representing the location.</span></span> |
| <span data-ttu-id="3d282-127">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="3d282-127">resolveAvailability</span></span> | <span data-ttu-id="3d282-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d282-128">Boolean</span></span> | <span data-ttu-id="3d282-p101">如果设为 true，且指定的资源处于忙碌状态，[findMeetingTimes](../api/user-findmeetingtimes.md) 会查找另一空闲资源。如果设为 false，且指定的资源处于忙碌状态，**findMeetingTimes** 会返回用户缓存中排名最靠前的资源，而不会检查其是否空闲。默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="3d282-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationconstraintitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
