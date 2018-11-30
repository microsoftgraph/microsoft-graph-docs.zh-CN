---
title: 位置资源类型
description: 表示事件的位置信息。
ms.openlocfilehash: fec075d37bfb2d7eca80f5007db53801dda96ed8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041568"
---
# <a name="location-resource-type"></a><span data-ttu-id="5531d-103">位置资源类型</span><span class="sxs-lookup"><span data-stu-id="5531d-103">Location resource type</span></span>

> <span data-ttu-id="5531d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5531d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5531d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5531d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5531d-106">表示[事件](event.md)的位置信息。</span><span class="sxs-lookup"><span data-stu-id="5531d-106">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="5531d-107">可采用多种方法在日历中创建事件，例如，通过应用使用 [create event](../api/user-post-events.md) REST API，或者手动使用 Outlook 用户界面。</span><span class="sxs-lookup"><span data-stu-id="5531d-107">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="5531d-108">在使用用户界面创建事件时，可以以纯文本格式（例如，“Harry's Bar”）指定位置，或者从 Outlook 提供的会议室列表、[必应自动建议](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/)或[必应本地搜索](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/)中指定位置。</span><span class="sxs-lookup"><span data-stu-id="5531d-108">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="5531d-109">根据事件的创建方式，Outlook 应以不同方式设置只读 **locationType** 属性。</span><span class="sxs-lookup"><span data-stu-id="5531d-109">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="5531d-110">事件的创建方式</span><span class="sxs-lookup"><span data-stu-id="5531d-110">How event was created</span></span>  | <span data-ttu-id="5531d-111">属性</span><span class="sxs-lookup"><span data-stu-id="5531d-111">Property</span></span>   | <span data-ttu-id="5531d-112">预期值</span><span class="sxs-lookup"><span data-stu-id="5531d-112">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="5531d-113">[create event](../api/user-post-events.md) REST API</span><span class="sxs-lookup"><span data-stu-id="5531d-113">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="5531d-114">**locationType**</span><span class="sxs-lookup"><span data-stu-id="5531d-114">**locationType**</span></span> | `default` |
| <span data-ttu-id="5531d-115">Outlook 中的用户界面</span><span class="sxs-lookup"><span data-stu-id="5531d-115">User interface in Outlook</span></span> | <span data-ttu-id="5531d-116">**locationType**</span><span class="sxs-lookup"><span data-stu-id="5531d-116">**locationType**</span></span> | <span data-ttu-id="5531d-117">以下各项之一：</span><span class="sxs-lookup"><span data-stu-id="5531d-117">One of the following:</span></span> <ul><li><span data-ttu-id="5531d-118">`default`，以纯文本格式输入的位置。</span><span class="sxs-lookup"><span data-stu-id="5531d-118">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="5531d-119">`conferenceRoom`，Outlook 会议室列表提供的会议室。</span><span class="sxs-lookup"><span data-stu-id="5531d-119">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="5531d-120">或者，该列表中的任意项：`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress`，必应自动建议或必应本地搜索中的位置。</span><span class="sxs-lookup"><span data-stu-id="5531d-120">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="5531d-121">属性</span><span class="sxs-lookup"><span data-stu-id="5531d-121">Properties</span></span>
| <span data-ttu-id="5531d-122">属性</span><span class="sxs-lookup"><span data-stu-id="5531d-122">Property</span></span>  | <span data-ttu-id="5531d-123">类型</span><span class="sxs-lookup"><span data-stu-id="5531d-123">Type</span></span>   | <span data-ttu-id="5531d-124">说明</span><span class="sxs-lookup"><span data-stu-id="5531d-124">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="5531d-125">address</span><span class="sxs-lookup"><span data-stu-id="5531d-125">address</span></span> | [<span data-ttu-id="5531d-126">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="5531d-126">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="5531d-127">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="5531d-127">The street address of the location.</span></span> |
| <span data-ttu-id="5531d-128">coordinates</span><span class="sxs-lookup"><span data-stu-id="5531d-128">coordinates</span></span> | [<span data-ttu-id="5531d-129">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="5531d-129">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="5531d-130">地理坐标和位置的海拔高度。</span><span class="sxs-lookup"><span data-stu-id="5531d-130">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="5531d-131">displayName</span><span class="sxs-lookup"><span data-stu-id="5531d-131">displayName</span></span>  | <span data-ttu-id="5531d-132">String</span><span class="sxs-lookup"><span data-stu-id="5531d-132">String</span></span> | <span data-ttu-id="5531d-133">与地点相关联的名称。</span><span class="sxs-lookup"><span data-stu-id="5531d-133">The name associated with the location.</span></span>                       |
| <span data-ttu-id="5531d-134">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="5531d-134">locationEmailAddress</span></span> | <span data-ttu-id="5531d-135">String</span><span class="sxs-lookup"><span data-stu-id="5531d-135">String</span></span> | <span data-ttu-id="5531d-136">（可选）与位置相关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5531d-136">Optional email address of the location.</span></span> |
| <span data-ttu-id="5531d-137">locationUri</span><span class="sxs-lookup"><span data-stu-id="5531d-137">locationUri</span></span> | <span data-ttu-id="5531d-138">String</span><span class="sxs-lookup"><span data-stu-id="5531d-138">String</span></span> | <span data-ttu-id="5531d-139">（可选）表示位置的 URI。</span><span class="sxs-lookup"><span data-stu-id="5531d-139">Optional URI representing the location.</span></span> |
| <span data-ttu-id="5531d-140">locationType</span><span class="sxs-lookup"><span data-stu-id="5531d-140">locationType</span></span> | <span data-ttu-id="5531d-141">String</span><span class="sxs-lookup"><span data-stu-id="5531d-141">String</span></span> | <span data-ttu-id="5531d-142">位置的类型。</span><span class="sxs-lookup"><span data-stu-id="5531d-142">The type of location.</span></span> <span data-ttu-id="5531d-143">可取值为：`default`、`conferenceRoom`、`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress`。</span><span class="sxs-lookup"><span data-stu-id="5531d-143">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="5531d-144">只读。</span><span class="sxs-lookup"><span data-stu-id="5531d-144">Read-only.</span></span>|
| <span data-ttu-id="5531d-145">uniqueId</span><span class="sxs-lookup"><span data-stu-id="5531d-145">uniqueId</span></span> | <span data-ttu-id="5531d-146">String</span><span class="sxs-lookup"><span data-stu-id="5531d-146">String</span></span> | <span data-ttu-id="5531d-147">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="5531d-147">For internal use only.</span></span>|
| <span data-ttu-id="5531d-148">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="5531d-148">uniqueIdType</span></span> | <span data-ttu-id="5531d-149">String</span><span class="sxs-lookup"><span data-stu-id="5531d-149">String</span></span> | <span data-ttu-id="5531d-150">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="5531d-150">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="5531d-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5531d-151">JSON representation</span></span>

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
  "locationUri": "string",
  "locationType": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
