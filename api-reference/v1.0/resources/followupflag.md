# <a name="followupflag-resource-type"></a><span data-ttu-id="0844b-101">followupFlag 资源类型</span><span class="sxs-lookup"><span data-stu-id="0844b-101">followupFlag resource type</span></span>


<span data-ttu-id="0844b-102">允许用户跟进更高版本的项目中设置标志。</span><span class="sxs-lookup"><span data-stu-id="0844b-102">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="0844b-103">属性</span><span class="sxs-lookup"><span data-stu-id="0844b-103">Properties</span></span>
| <span data-ttu-id="0844b-104">属性</span><span class="sxs-lookup"><span data-stu-id="0844b-104">Property</span></span>     | <span data-ttu-id="0844b-105">类型</span><span class="sxs-lookup"><span data-stu-id="0844b-105">Type</span></span>   |<span data-ttu-id="0844b-106">说明</span><span class="sxs-lookup"><span data-stu-id="0844b-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0844b-107">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0844b-107">completedDateTime</span></span>|[<span data-ttu-id="0844b-108">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0844b-108">dateTimeTimeZone</span></span>](dateTimeTimeZone.md)|<span data-ttu-id="0844b-109">完成跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0844b-109">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="0844b-110">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="0844b-110">dueDateTime</span></span>|<span data-ttu-id="0844b-111">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0844b-111">**dateTimeTimeZone**</span></span>|<span data-ttu-id="0844b-112">待完成的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0844b-112">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="0844b-113">flagStatus</span><span class="sxs-lookup"><span data-stu-id="0844b-113">flagStatus</span></span>|<span data-ttu-id="0844b-114">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="0844b-114">followupFlagStatus</span></span>|<span data-ttu-id="0844b-115">项目的跟进状态。</span><span class="sxs-lookup"><span data-stu-id="0844b-115">The status for follow-up for an item.</span></span> <span data-ttu-id="0844b-116">可取值为：`notFlagged`、`complete` 和 `flagged`。</span><span class="sxs-lookup"><span data-stu-id="0844b-116">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="0844b-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0844b-117">startDateTime</span></span>|<span data-ttu-id="0844b-118">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0844b-118">**dateTimeTimeZone**</span></span>|<span data-ttu-id="0844b-119">要开始的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0844b-119">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0844b-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0844b-120">JSON representation</span></span>

<span data-ttu-id="0844b-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0844b-121">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
