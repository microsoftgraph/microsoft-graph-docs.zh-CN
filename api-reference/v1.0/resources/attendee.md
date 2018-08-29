# <a name="attendee-resource-type"></a><span data-ttu-id="5a7bc-101">与会者资源类型</span><span class="sxs-lookup"><span data-stu-id="5a7bc-101">attendee resource type</span></span>

<span data-ttu-id="5a7bc-102">会议与会者。</span><span class="sxs-lookup"><span data-stu-id="5a7bc-102">An event attendee.</span></span> <span data-ttu-id="5a7bc-103">这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。</span><span class="sxs-lookup"><span data-stu-id="5a7bc-103">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="5a7bc-104">由 [attendeeBase](attendeebase.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="5a7bc-104">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5a7bc-105">属性</span><span class="sxs-lookup"><span data-stu-id="5a7bc-105">Properties</span></span>
| <span data-ttu-id="5a7bc-106">属性</span><span class="sxs-lookup"><span data-stu-id="5a7bc-106">Property</span></span>     | <span data-ttu-id="5a7bc-107">类型</span><span class="sxs-lookup"><span data-stu-id="5a7bc-107">Type</span></span>   |<span data-ttu-id="5a7bc-108">说明</span><span class="sxs-lookup"><span data-stu-id="5a7bc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a7bc-109">状态</span><span class="sxs-lookup"><span data-stu-id="5a7bc-109">status</span></span>|[<span data-ttu-id="5a7bc-110">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="5a7bc-110">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="5a7bc-111">事件与会者的响应（无、接受、拒绝等）和发送响应的日期时间。</span><span class="sxs-lookup"><span data-stu-id="5a7bc-111">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="5a7bc-112">类型</span><span class="sxs-lookup"><span data-stu-id="5a7bc-112">type</span></span>|<span data-ttu-id="5a7bc-113">String</span><span class="sxs-lookup"><span data-stu-id="5a7bc-113">String</span></span>|<span data-ttu-id="5a7bc-114">与会者类型：`required`、`optional`、`resource`。</span><span class="sxs-lookup"><span data-stu-id="5a7bc-114">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="5a7bc-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5a7bc-115">emailAddress</span></span>|[<span data-ttu-id="5a7bc-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5a7bc-116">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="5a7bc-117">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="5a7bc-117">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a7bc-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a7bc-118">JSON representation</span></span>

<span data-ttu-id="5a7bc-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a7bc-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attendeeBase",
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