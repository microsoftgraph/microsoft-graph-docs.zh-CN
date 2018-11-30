---
title: locationConstraintItem 资源类型
description: 客户端声明的会议地点条件。
ms.openlocfilehash: f29ff1283d876e726e27473485a183956137f981
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041786"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="76895-103">locationConstraintItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="76895-103">locationConstraintItem resource type</span></span>

> <span data-ttu-id="76895-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="76895-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76895-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="76895-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76895-106">客户端声明的会议地点条件。</span><span class="sxs-lookup"><span data-stu-id="76895-106">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="76895-107">由 [location](location.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="76895-107">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="76895-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76895-108">JSON representation</span></span>

<span data-ttu-id="76895-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76895-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="76895-110">属性</span><span class="sxs-lookup"><span data-stu-id="76895-110">Properties</span></span>
| <span data-ttu-id="76895-111">属性</span><span class="sxs-lookup"><span data-stu-id="76895-111">Property</span></span>     | <span data-ttu-id="76895-112">类型</span><span class="sxs-lookup"><span data-stu-id="76895-112">Type</span></span>   |<span data-ttu-id="76895-113">说明</span><span class="sxs-lookup"><span data-stu-id="76895-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="76895-114">address</span><span class="sxs-lookup"><span data-stu-id="76895-114">address</span></span> | [<span data-ttu-id="76895-115">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="76895-115">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="76895-116">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="76895-116">The street address of the location.</span></span> |
| <span data-ttu-id="76895-117">coordinates</span><span class="sxs-lookup"><span data-stu-id="76895-117">coordinates</span></span> | [<span data-ttu-id="76895-118">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="76895-118">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="76895-119">地理坐标和位置的海拔高度。</span><span class="sxs-lookup"><span data-stu-id="76895-119">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="76895-120">displayName</span><span class="sxs-lookup"><span data-stu-id="76895-120">displayName</span></span>  | <span data-ttu-id="76895-121">String</span><span class="sxs-lookup"><span data-stu-id="76895-121">String</span></span> | <span data-ttu-id="76895-122">与地点相关联的名称。</span><span class="sxs-lookup"><span data-stu-id="76895-122">The name associated with the location.</span></span>                       |
| <span data-ttu-id="76895-123">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="76895-123">locationEmailAddress</span></span> | <span data-ttu-id="76895-124">String</span><span class="sxs-lookup"><span data-stu-id="76895-124">String</span></span> | <span data-ttu-id="76895-125">（可选）与位置相关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="76895-125">Optional email address of the location.</span></span> |
| <span data-ttu-id="76895-126">locationUri</span><span class="sxs-lookup"><span data-stu-id="76895-126">locationUri</span></span> | <span data-ttu-id="76895-127">String</span><span class="sxs-lookup"><span data-stu-id="76895-127">String</span></span> | <span data-ttu-id="76895-128">（可选）表示位置的 URI。</span><span class="sxs-lookup"><span data-stu-id="76895-128">Optional URI representing the location.</span></span> |
| <span data-ttu-id="76895-129">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="76895-129">resolveAvailability</span></span> | <span data-ttu-id="76895-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="76895-130">Boolean</span></span> | <span data-ttu-id="76895-p102">如果设为 true，且指定的资源处于忙碌状态，[findMeetingTimes](../api/user-findmeetingtimes.md) 会查找另一空闲资源。如果设为 false，且指定的资源处于忙碌状态，**findMeetingTimes** 会返回用户缓存中排名最靠前的资源，而不会检查其是否空闲。默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="76895-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->