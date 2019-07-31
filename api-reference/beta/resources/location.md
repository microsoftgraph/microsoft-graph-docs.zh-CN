---
title: 位置资源类型
description: 表示事件的位置信息。
localization_priority: Normal
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b96dfb725c6a4e82c61f4d2eac3ebb3602c5d738
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009949"
---
# <a name="location-resource-type"></a><span data-ttu-id="09d85-103">位置资源类型</span><span class="sxs-lookup"><span data-stu-id="09d85-103">Location resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09d85-104">表示[事件](event.md)的位置信息。</span><span class="sxs-lookup"><span data-stu-id="09d85-104">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="09d85-105">可采用多种方法在日历中创建事件，例如，通过应用使用 [create event](../api/user-post-events.md) REST API，或者手动使用 Outlook 用户界面。</span><span class="sxs-lookup"><span data-stu-id="09d85-105">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="09d85-106">在使用用户界面创建事件时，可以以纯文本格式（例如，“Harry's Bar”）指定位置，或者从 Outlook 提供的会议室列表、[必应自动建议](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/)或[必应本地搜索](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/)中指定位置。</span><span class="sxs-lookup"><span data-stu-id="09d85-106">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="09d85-107">根据事件的创建方式，Outlook 应以不同方式设置只读 **locationType** 属性。</span><span class="sxs-lookup"><span data-stu-id="09d85-107">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="09d85-108">事件的创建方式</span><span class="sxs-lookup"><span data-stu-id="09d85-108">How event was created</span></span>  | <span data-ttu-id="09d85-109">属性</span><span class="sxs-lookup"><span data-stu-id="09d85-109">Property</span></span>   | <span data-ttu-id="09d85-110">预期值</span><span class="sxs-lookup"><span data-stu-id="09d85-110">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="09d85-111">[create event](../api/user-post-events.md) REST API</span><span class="sxs-lookup"><span data-stu-id="09d85-111">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="09d85-112">**locationType**</span><span class="sxs-lookup"><span data-stu-id="09d85-112">**locationType**</span></span> | `default` |
| <span data-ttu-id="09d85-113">Outlook 中的用户界面</span><span class="sxs-lookup"><span data-stu-id="09d85-113">User interface in Outlook</span></span> | <span data-ttu-id="09d85-114">**locationType**</span><span class="sxs-lookup"><span data-stu-id="09d85-114">**locationType**</span></span> | <span data-ttu-id="09d85-115">以下各项之一：</span><span class="sxs-lookup"><span data-stu-id="09d85-115">One of the following:</span></span> <ul><li><span data-ttu-id="09d85-116">`default`，以纯文本格式输入的位置。</span><span class="sxs-lookup"><span data-stu-id="09d85-116">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="09d85-117">`conferenceRoom`，Outlook 会议室列表提供的会议室。</span><span class="sxs-lookup"><span data-stu-id="09d85-117">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="09d85-118">或者，该列表中的任意项：`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress`，必应自动建议或必应本地搜索中的位置。</span><span class="sxs-lookup"><span data-stu-id="09d85-118">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="09d85-119">属性</span><span class="sxs-lookup"><span data-stu-id="09d85-119">Properties</span></span>
| <span data-ttu-id="09d85-120">属性</span><span class="sxs-lookup"><span data-stu-id="09d85-120">Property</span></span>  | <span data-ttu-id="09d85-121">类型</span><span class="sxs-lookup"><span data-stu-id="09d85-121">Type</span></span>   | <span data-ttu-id="09d85-122">说明</span><span class="sxs-lookup"><span data-stu-id="09d85-122">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="09d85-123">address</span><span class="sxs-lookup"><span data-stu-id="09d85-123">address</span></span> | [<span data-ttu-id="09d85-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="09d85-124">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="09d85-125">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="09d85-125">The street address of the location.</span></span> |
| <span data-ttu-id="09d85-126">coordinates</span><span class="sxs-lookup"><span data-stu-id="09d85-126">coordinates</span></span> | [<span data-ttu-id="09d85-127">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="09d85-127">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="09d85-128">地理坐标和位置的海拔高度。</span><span class="sxs-lookup"><span data-stu-id="09d85-128">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="09d85-129">displayName</span><span class="sxs-lookup"><span data-stu-id="09d85-129">displayName</span></span>  | <span data-ttu-id="09d85-130">String</span><span class="sxs-lookup"><span data-stu-id="09d85-130">String</span></span> | <span data-ttu-id="09d85-131">与地点相关联的名称。</span><span class="sxs-lookup"><span data-stu-id="09d85-131">The name associated with the location.</span></span>                       |
| <span data-ttu-id="09d85-132">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="09d85-132">locationEmailAddress</span></span> | <span data-ttu-id="09d85-133">String</span><span class="sxs-lookup"><span data-stu-id="09d85-133">String</span></span> | <span data-ttu-id="09d85-134">（可选）与位置相关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="09d85-134">Optional email address of the location.</span></span> |
| <span data-ttu-id="09d85-135">locationUri</span><span class="sxs-lookup"><span data-stu-id="09d85-135">locationUri</span></span> | <span data-ttu-id="09d85-136">String</span><span class="sxs-lookup"><span data-stu-id="09d85-136">String</span></span> | <span data-ttu-id="09d85-137">（可选）表示位置的 URI。</span><span class="sxs-lookup"><span data-stu-id="09d85-137">Optional URI representing the location.</span></span> |
| <span data-ttu-id="09d85-138">locationType</span><span class="sxs-lookup"><span data-stu-id="09d85-138">locationType</span></span> | <span data-ttu-id="09d85-139">locationType</span><span class="sxs-lookup"><span data-stu-id="09d85-139">locationType</span></span> | <span data-ttu-id="09d85-140">位置的类型。</span><span class="sxs-lookup"><span data-stu-id="09d85-140">The type of location.</span></span> <span data-ttu-id="09d85-141">可取值为：`default`、`conferenceRoom`、`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress`。</span><span class="sxs-lookup"><span data-stu-id="09d85-141">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="09d85-142">只读。</span><span class="sxs-lookup"><span data-stu-id="09d85-142">Read-only.</span></span>|
| <span data-ttu-id="09d85-143">uniqueId</span><span class="sxs-lookup"><span data-stu-id="09d85-143">uniqueId</span></span> | <span data-ttu-id="09d85-144">String</span><span class="sxs-lookup"><span data-stu-id="09d85-144">String</span></span> | <span data-ttu-id="09d85-145">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="09d85-145">For internal use only.</span></span>|
| <span data-ttu-id="09d85-146">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="09d85-146">uniqueIdType</span></span> | <span data-ttu-id="09d85-147">String</span><span class="sxs-lookup"><span data-stu-id="09d85-147">String</span></span> | <span data-ttu-id="09d85-148">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="09d85-148">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="09d85-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09d85-149">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
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



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
