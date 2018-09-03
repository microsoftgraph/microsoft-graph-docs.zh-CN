# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="30bf9-101">attendeeAvailability 资源类型</span><span class="sxs-lookup"><span data-stu-id="30bf9-101">attendeeAvailability resource type</span></span>

<span data-ttu-id="30bf9-102">与会者的类型和忙/闲状态。</span><span class="sxs-lookup"><span data-stu-id="30bf9-102">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="30bf9-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30bf9-103">JSON representation</span></span>

<span data-ttu-id="30bf9-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30bf9-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="30bf9-105">属性</span><span class="sxs-lookup"><span data-stu-id="30bf9-105">Properties</span></span>
| <span data-ttu-id="30bf9-106">属性</span><span class="sxs-lookup"><span data-stu-id="30bf9-106">Property</span></span>     | <span data-ttu-id="30bf9-107">类型</span><span class="sxs-lookup"><span data-stu-id="30bf9-107">Type</span></span>   |<span data-ttu-id="30bf9-108">说明</span><span class="sxs-lookup"><span data-stu-id="30bf9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30bf9-109">attendee</span><span class="sxs-lookup"><span data-stu-id="30bf9-109">attendee</span></span>|[<span data-ttu-id="30bf9-110">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="30bf9-110">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="30bf9-111">与会者类型，即是人员还是资源；如果是人员，是必需还是可选。</span><span class="sxs-lookup"><span data-stu-id="30bf9-111">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="30bf9-112">availability</span><span class="sxs-lookup"><span data-stu-id="30bf9-112">availability</span></span>|<span data-ttu-id="30bf9-113">FreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="30bf9-113">FreeBusyStatus</span></span>| <span data-ttu-id="30bf9-114">与会者的忙/闲状态。</span><span class="sxs-lookup"><span data-stu-id="30bf9-114">The availability status of the attendee. Possible values are: , , , , , .</span></span> <span data-ttu-id="30bf9-115">可取值为：`free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="30bf9-115">The possible values are `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`, , , , , , or .</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
