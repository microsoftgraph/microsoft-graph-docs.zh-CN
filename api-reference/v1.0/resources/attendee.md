# <a name="attendee-resource-type"></a><span data-ttu-id="3194b-101">与会者资源类型</span><span class="sxs-lookup"><span data-stu-id="3194b-101">attendee resource type</span></span>

<span data-ttu-id="3194b-102">会议与会者。</span><span class="sxs-lookup"><span data-stu-id="3194b-102">An event attendee.</span></span>

<span data-ttu-id="3194b-103">由 [attendeeBase](attendeebase.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="3194b-103">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3194b-104">属性</span><span class="sxs-lookup"><span data-stu-id="3194b-104">Properties</span></span>
| <span data-ttu-id="3194b-105">属性</span><span class="sxs-lookup"><span data-stu-id="3194b-105">Property</span></span>     | <span data-ttu-id="3194b-106">类型</span><span class="sxs-lookup"><span data-stu-id="3194b-106">Type</span></span>   |<span data-ttu-id="3194b-107">说明</span><span class="sxs-lookup"><span data-stu-id="3194b-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3194b-108">状态</span><span class="sxs-lookup"><span data-stu-id="3194b-108">status</span></span>|[<span data-ttu-id="3194b-109">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="3194b-109">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="3194b-110">事件与会者的响应（无、接受、拒绝等）和发送响应的日期时间。</span><span class="sxs-lookup"><span data-stu-id="3194b-110">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="3194b-111">类型</span><span class="sxs-lookup"><span data-stu-id="3194b-111">type</span></span>|<span data-ttu-id="3194b-112">String</span><span class="sxs-lookup"><span data-stu-id="3194b-112">String</span></span>|<span data-ttu-id="3194b-113">与会者类型：`Required`、`Optional`、`Resource`。</span><span class="sxs-lookup"><span data-stu-id="3194b-113">The attendee type: `Required`, `Optional`, `Resource`.</span></span>|
|<span data-ttu-id="3194b-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3194b-114">emailAddress</span></span>|[<span data-ttu-id="3194b-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3194b-115">emailAddress</span></span>](emailAddress.md)|<span data-ttu-id="3194b-116">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="3194b-116">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3194b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3194b-117">JSON representation</span></span>

<span data-ttu-id="3194b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3194b-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->