# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="d4007-101">meetingTimeSuggestion 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4007-101">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="d4007-102">会议时间建议包括会议时间、出席可能性、个人忙/闲状态和可用会议地点等信息。</span><span class="sxs-lookup"><span data-stu-id="d4007-102">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4007-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4007-103">JSON representation</span></span>

<span data-ttu-id="d4007-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4007-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 100.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="d4007-105">属性</span><span class="sxs-lookup"><span data-stu-id="d4007-105">Properties</span></span>
| <span data-ttu-id="d4007-106">属性</span><span class="sxs-lookup"><span data-stu-id="d4007-106">Property</span></span>     | <span data-ttu-id="d4007-107">类型</span><span class="sxs-lookup"><span data-stu-id="d4007-107">Type</span></span>   |<span data-ttu-id="d4007-108">说明</span><span class="sxs-lookup"><span data-stu-id="d4007-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4007-109">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="d4007-109">attendeeAvailability</span></span>|<span data-ttu-id="d4007-110">[attendeeAvailability](attendeeavailability.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4007-110">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="d4007-111">显示此会议时间建议中各个与会者的忙/闲状态的数组。</span><span class="sxs-lookup"><span data-stu-id="d4007-111">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="d4007-112">confidence</span><span class="sxs-lookup"><span data-stu-id="d4007-112">confidence</span></span>|<span data-ttu-id="d4007-113">Double</span><span class="sxs-lookup"><span data-stu-id="d4007-113">Double</span></span>|<span data-ttu-id="d4007-114">表示所有与会者的出席可能性的百分比值。</span><span class="sxs-lookup"><span data-stu-id="d4007-114">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="d4007-115">locations</span><span class="sxs-lookup"><span data-stu-id="d4007-115">locations</span></span>|<span data-ttu-id="d4007-116">[location](location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4007-116">[location](location.md) collection</span></span>|<span data-ttu-id="d4007-117">指定此会议时间建议中各个会议地点的名称和地理位置的数组。</span><span class="sxs-lookup"><span data-stu-id="d4007-117">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="d4007-118">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="d4007-118">meetingTimeSlot</span></span>|[<span data-ttu-id="d4007-119">timeSlot</span><span class="sxs-lookup"><span data-stu-id="d4007-119">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="d4007-120">建议的会议时间段。</span><span class="sxs-lookup"><span data-stu-id="d4007-120">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="d4007-121">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="d4007-121">organizerAvailability</span></span>|<span data-ttu-id="d4007-122">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="d4007-122">FreeBusyStatus</span></span>| <span data-ttu-id="d4007-123">建议会议的会议组织者忙/闲状态。</span><span class="sxs-lookup"><span data-stu-id="d4007-123">Availability of the meeting organizer for this meeting suggestion. Possible values are: , , , , , .</span></span> <span data-ttu-id="d4007-124">可取值为：`free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="d4007-124">The possible values are `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`, , , , , , or .</span></span>|
|<span data-ttu-id="d4007-125">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="d4007-125">suggestionReason</span></span>|<span data-ttu-id="d4007-126">字符串</span><span class="sxs-lookup"><span data-stu-id="d4007-126">String</span></span>|<span data-ttu-id="d4007-127">会议时间建议的理由。</span><span class="sxs-lookup"><span data-stu-id="d4007-127">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->