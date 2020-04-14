---
title: 位置资源类型
description: 表示事件的位置信息。
localization_priority: Normal
doc_type: resourcePageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: 265dcc7626aaaee1a43997b8c51cea9feb4763c5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442714"
---
# <a name="location-resource-type"></a><span data-ttu-id="a09d9-103">位置资源类型</span><span class="sxs-lookup"><span data-stu-id="a09d9-103">Location resource type</span></span>

<span data-ttu-id="a09d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a09d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a09d9-105">表示[事件](event.md)的位置信息。</span><span class="sxs-lookup"><span data-stu-id="a09d9-105">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="a09d9-106">可采用多种方法在日历中创建事件，例如，通过应用使用 [create event](../api/user-post-events.md) REST API，或者手动使用 Outlook 用户界面。</span><span class="sxs-lookup"><span data-stu-id="a09d9-106">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="a09d9-107">在使用用户界面创建事件时，可以以纯文本格式（例如，“Harry's Bar”）指定位置，或者从 Outlook 提供的会议室列表、[必应自动建议](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/)或[必应本地搜索](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/)中指定位置。</span><span class="sxs-lookup"><span data-stu-id="a09d9-107">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="a09d9-108">根据事件的创建方式，Outlook 应以不同方式设置只读 **locationType** 属性。</span><span class="sxs-lookup"><span data-stu-id="a09d9-108">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="a09d9-109">事件的创建方式</span><span class="sxs-lookup"><span data-stu-id="a09d9-109">How event was created</span></span>  | <span data-ttu-id="a09d9-110">属性</span><span class="sxs-lookup"><span data-stu-id="a09d9-110">Property</span></span>   | <span data-ttu-id="a09d9-111">预期值</span><span class="sxs-lookup"><span data-stu-id="a09d9-111">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="a09d9-112">[create event](../api/user-post-events.md) REST API</span><span class="sxs-lookup"><span data-stu-id="a09d9-112">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="a09d9-113">**locationType**</span><span class="sxs-lookup"><span data-stu-id="a09d9-113">**locationType**</span></span> | `default` |
| <span data-ttu-id="a09d9-114">Outlook 中的用户界面</span><span class="sxs-lookup"><span data-stu-id="a09d9-114">User interface in Outlook</span></span> | <span data-ttu-id="a09d9-115">**locationType**</span><span class="sxs-lookup"><span data-stu-id="a09d9-115">**locationType**</span></span> | <span data-ttu-id="a09d9-116">以下各项之一：</span><span class="sxs-lookup"><span data-stu-id="a09d9-116">One of the following:</span></span> <ul><li><span data-ttu-id="a09d9-117">`default`，以纯文本格式输入的位置。</span><span class="sxs-lookup"><span data-stu-id="a09d9-117">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="a09d9-118">`conferenceRoom`，Outlook 会议室列表提供的会议室。</span><span class="sxs-lookup"><span data-stu-id="a09d9-118">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="a09d9-119">或者，该列表中的任意项：`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress`，必应自动建议或必应本地搜索中的位置。</span><span class="sxs-lookup"><span data-stu-id="a09d9-119">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="a09d9-120">属性</span><span class="sxs-lookup"><span data-stu-id="a09d9-120">Properties</span></span>
| <span data-ttu-id="a09d9-121">属性</span><span class="sxs-lookup"><span data-stu-id="a09d9-121">Property</span></span>  | <span data-ttu-id="a09d9-122">类型</span><span class="sxs-lookup"><span data-stu-id="a09d9-122">Type</span></span>   | <span data-ttu-id="a09d9-123">说明</span><span class="sxs-lookup"><span data-stu-id="a09d9-123">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="a09d9-124">address</span><span class="sxs-lookup"><span data-stu-id="a09d9-124">address</span></span> | [<span data-ttu-id="a09d9-125">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="a09d9-125">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="a09d9-126">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="a09d9-126">The street address of the location.</span></span> |
| <span data-ttu-id="a09d9-127">coordinates</span><span class="sxs-lookup"><span data-stu-id="a09d9-127">coordinates</span></span> | [<span data-ttu-id="a09d9-128">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a09d9-128">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="a09d9-129">地理坐标和位置的海拔高度。</span><span class="sxs-lookup"><span data-stu-id="a09d9-129">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="a09d9-130">displayName</span><span class="sxs-lookup"><span data-stu-id="a09d9-130">displayName</span></span>  | <span data-ttu-id="a09d9-131">String</span><span class="sxs-lookup"><span data-stu-id="a09d9-131">String</span></span> | <span data-ttu-id="a09d9-132">与地点相关联的名称。</span><span class="sxs-lookup"><span data-stu-id="a09d9-132">The name associated with the location.</span></span>                       |
| <span data-ttu-id="a09d9-133">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a09d9-133">locationEmailAddress</span></span> | <span data-ttu-id="a09d9-134">String</span><span class="sxs-lookup"><span data-stu-id="a09d9-134">String</span></span> | <span data-ttu-id="a09d9-135">（可选）与位置相关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a09d9-135">Optional email address of the location.</span></span> |
| <span data-ttu-id="a09d9-136">locationUri</span><span class="sxs-lookup"><span data-stu-id="a09d9-136">locationUri</span></span> | <span data-ttu-id="a09d9-137">String</span><span class="sxs-lookup"><span data-stu-id="a09d9-137">String</span></span> | <span data-ttu-id="a09d9-138">（可选）表示位置的 URI。</span><span class="sxs-lookup"><span data-stu-id="a09d9-138">Optional URI representing the location.</span></span> |
| <span data-ttu-id="a09d9-139">locationType</span><span class="sxs-lookup"><span data-stu-id="a09d9-139">locationType</span></span> | <span data-ttu-id="a09d9-140">locationType</span><span class="sxs-lookup"><span data-stu-id="a09d9-140">locationType</span></span> | <span data-ttu-id="a09d9-141">位置的类型。</span><span class="sxs-lookup"><span data-stu-id="a09d9-141">The type of location.</span></span> <span data-ttu-id="a09d9-142">可取值为：`default`、`conferenceRoom`、`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress`。</span><span class="sxs-lookup"><span data-stu-id="a09d9-142">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="a09d9-143">只读。</span><span class="sxs-lookup"><span data-stu-id="a09d9-143">Read-only.</span></span>|
| <span data-ttu-id="a09d9-144">uniqueId</span><span class="sxs-lookup"><span data-stu-id="a09d9-144">uniqueId</span></span> | <span data-ttu-id="a09d9-145">String</span><span class="sxs-lookup"><span data-stu-id="a09d9-145">String</span></span> | <span data-ttu-id="a09d9-146">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="a09d9-146">For internal use only.</span></span>|
| <span data-ttu-id="a09d9-147">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="a09d9-147">uniqueIdType</span></span> | <span data-ttu-id="a09d9-148">String</span><span class="sxs-lookup"><span data-stu-id="a09d9-148">String</span></span> | <span data-ttu-id="a09d9-149">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="a09d9-149">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a09d9-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a09d9-150">JSON representation</span></span>

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
