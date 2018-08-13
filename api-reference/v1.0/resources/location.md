# <a name="location-resource-type"></a><span data-ttu-id="40d30-101">位置资源类型</span><span class="sxs-lookup"><span data-stu-id="40d30-101">Location resource type</span></span>

<span data-ttu-id="40d30-102">表示[事件](event.md)的位置信息。</span><span class="sxs-lookup"><span data-stu-id="40d30-102">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="40d30-103">可采用多种方法在日历中创建事件，例如，通过应用使用 [create event](../api/user_post_events.md) REST API，或者手动使用 Outlook 用户界面。</span><span class="sxs-lookup"><span data-stu-id="40d30-103">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user_post_events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="40d30-104">在使用用户界面创建事件时，可以以纯文本格式（例如，“Harry's Bar”）指定位置，或者从 Outlook 提供的会议室列表、[必应自动建议](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/)或[必应本地搜索](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/)中指定位置。</span><span class="sxs-lookup"><span data-stu-id="40d30-104">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="40d30-105">根据事件的创建方式，Outlook 应以不同方式设置只读 **locationType** 属性。</span><span class="sxs-lookup"><span data-stu-id="40d30-105">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="40d30-106">事件的创建方式</span><span class="sxs-lookup"><span data-stu-id="40d30-106">How event was created</span></span>  | <span data-ttu-id="40d30-107">属性</span><span class="sxs-lookup"><span data-stu-id="40d30-107">Property</span></span>   | <span data-ttu-id="40d30-108">预期值</span><span class="sxs-lookup"><span data-stu-id="40d30-108">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="40d30-109">[create event](../api/user_post_events.md) REST API</span><span class="sxs-lookup"><span data-stu-id="40d30-109">[create event](../api/user_post_events.md) REST API</span></span> | <span data-ttu-id="40d30-110">**locationType**</span><span class="sxs-lookup"><span data-stu-id="40d30-110">**locationType**</span></span> | `default` |
| <span data-ttu-id="40d30-111">Outlook 中的用户界面</span><span class="sxs-lookup"><span data-stu-id="40d30-111">User interface in Outlook</span></span> | <span data-ttu-id="40d30-112">**locationType**</span><span class="sxs-lookup"><span data-stu-id="40d30-112">**locationType**</span></span> | <span data-ttu-id="40d30-113">以下各项之一：</span><span class="sxs-lookup"><span data-stu-id="40d30-113">One of the following:</span></span> <ul><li><span data-ttu-id="40d30-114">`default`，以纯文本格式输入的位置。</span><span class="sxs-lookup"><span data-stu-id="40d30-114">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="40d30-115">`conferenceRoom`，Outlook 会议室列表提供的会议室。</span><span class="sxs-lookup"><span data-stu-id="40d30-115">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="40d30-116">或者，该列表中的任意项：`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress`，必应自动建议或必应本地搜索中的位置。</span><span class="sxs-lookup"><span data-stu-id="40d30-116">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |

## <a name="properties"></a><span data-ttu-id="40d30-117">属性</span><span class="sxs-lookup"><span data-stu-id="40d30-117">Properties</span></span>
| <span data-ttu-id="40d30-118">属性</span><span class="sxs-lookup"><span data-stu-id="40d30-118">Property</span></span>  | <span data-ttu-id="40d30-119">类型</span><span class="sxs-lookup"><span data-stu-id="40d30-119">Type</span></span>   | <span data-ttu-id="40d30-120">说明</span><span class="sxs-lookup"><span data-stu-id="40d30-120">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="40d30-121">address</span><span class="sxs-lookup"><span data-stu-id="40d30-121">address</span></span> | [<span data-ttu-id="40d30-122">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="40d30-122">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="40d30-123">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="40d30-123">The street address of the location.</span></span> |
| <span data-ttu-id="40d30-124">coordinates</span><span class="sxs-lookup"><span data-stu-id="40d30-124">coordinates</span></span> | [<span data-ttu-id="40d30-125">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="40d30-125">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="40d30-126">地理坐标和位置的海拔高度。</span><span class="sxs-lookup"><span data-stu-id="40d30-126">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="40d30-127">displayName</span><span class="sxs-lookup"><span data-stu-id="40d30-127">displayName</span></span>  | <span data-ttu-id="40d30-128">String</span><span class="sxs-lookup"><span data-stu-id="40d30-128">String</span></span> | <span data-ttu-id="40d30-129">与地点相关联的名称。</span><span class="sxs-lookup"><span data-stu-id="40d30-129">The name associated with the location.</span></span>                       |
| <span data-ttu-id="40d30-130">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="40d30-130">locationEmailAddress</span></span> | <span data-ttu-id="40d30-131">String</span><span class="sxs-lookup"><span data-stu-id="40d30-131">String</span></span> | <span data-ttu-id="40d30-132">（可选）与位置相关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="40d30-132">Optional email address of the location.</span></span>              |
| <span data-ttu-id="40d30-133">locationUri</span><span class="sxs-lookup"><span data-stu-id="40d30-133">locationUri</span></span> | <span data-ttu-id="40d30-134">String</span><span class="sxs-lookup"><span data-stu-id="40d30-134">String</span></span> | <span data-ttu-id="40d30-135">（可选）表示位置的 URI。</span><span class="sxs-lookup"><span data-stu-id="40d30-135">Optional URI representing the location.</span></span> |
| <span data-ttu-id="40d30-136">locationType</span><span class="sxs-lookup"><span data-stu-id="40d30-136">locationType</span></span> | <span data-ttu-id="40d30-137">String</span><span class="sxs-lookup"><span data-stu-id="40d30-137">String</span></span> | <span data-ttu-id="40d30-138">位置的类型。</span><span class="sxs-lookup"><span data-stu-id="40d30-138">The type of location.</span></span> <span data-ttu-id="40d30-139">可取值为：`default`、`conferenceRoom`、`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress`。</span><span class="sxs-lookup"><span data-stu-id="40d30-139">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="40d30-140">只读。</span><span class="sxs-lookup"><span data-stu-id="40d30-140">Read-only.</span></span>|
| <span data-ttu-id="40d30-141">uniqueId</span><span class="sxs-lookup"><span data-stu-id="40d30-141">uniqueId</span></span> | <span data-ttu-id="40d30-142">String</span><span class="sxs-lookup"><span data-stu-id="40d30-142">String</span></span> | <span data-ttu-id="40d30-143">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="40d30-143">For internal use only.</span></span>|
| <span data-ttu-id="40d30-144">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="40d30-144">uniqueIdType</span></span> | <span data-ttu-id="40d30-145">String</span><span class="sxs-lookup"><span data-stu-id="40d30-145">String</span></span> | <span data-ttu-id="40d30-146">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="40d30-146">For internal use only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="40d30-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40d30-147">JSON representation</span></span>

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
