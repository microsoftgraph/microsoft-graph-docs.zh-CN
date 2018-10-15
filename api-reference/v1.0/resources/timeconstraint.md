# <a name="timeconstraint-resource-type"></a><span data-ttu-id="aad5d-101">timeConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="aad5d-101">timeConstraint resource type</span></span>

<span data-ttu-id="aad5d-102">根据活动的特定性质和开放时间段，将会议时间建议限制为某周的几个小时或几天。</span><span class="sxs-lookup"><span data-stu-id="aad5d-102">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aad5d-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aad5d-103">JSON representation</span></span>

<span data-ttu-id="aad5d-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aad5d-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="aad5d-105">属性</span><span class="sxs-lookup"><span data-stu-id="aad5d-105">Properties</span></span>
| <span data-ttu-id="aad5d-106">属性</span><span class="sxs-lookup"><span data-stu-id="aad5d-106">Property</span></span>     | <span data-ttu-id="aad5d-107">类型</span><span class="sxs-lookup"><span data-stu-id="aad5d-107">Type</span></span>   |<span data-ttu-id="aad5d-108">说明</span><span class="sxs-lookup"><span data-stu-id="aad5d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aad5d-109">activityDomain</span><span class="sxs-lookup"><span data-stu-id="aad5d-109">activityDomain</span></span>|<span data-ttu-id="aad5d-110">activityDomain</span><span class="sxs-lookup"><span data-stu-id="aad5d-110">activityDomain</span></span>|<span data-ttu-id="aad5d-111">活动的性质，可选。</span><span class="sxs-lookup"><span data-stu-id="aad5d-111">The nature of the activity, optional. Possible values are: , , , or .</span></span> <span data-ttu-id="aad5d-112">可取值为：`work`、`personal`、`unrestricted` 或 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="aad5d-112">The possible values are `work`, `personal`, `unrestricted`, , , , , , , , , or `unknown`.</span></span>|
|<span data-ttu-id="aad5d-113">timeslots</span><span class="sxs-lookup"><span data-stu-id="aad5d-113">timeslots</span></span>|<span data-ttu-id="aad5d-114">[timeSlot](timeslot.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aad5d-114">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="aad5d-115">一组时间段。</span><span class="sxs-lookup"><span data-stu-id="aad5d-115">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
