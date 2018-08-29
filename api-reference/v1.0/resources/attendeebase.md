# <a name="attendeebase-resource-type"></a><span data-ttu-id="8cc4f-101">attendeeBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="8cc4f-101">attendeeBase resource type</span></span>

<span data-ttu-id="8cc4f-102">与会者类型。</span><span class="sxs-lookup"><span data-stu-id="8cc4f-102">The type of attendee.</span></span>

<span data-ttu-id="8cc4f-103">由 [recipient](recipient.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="8cc4f-103">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cc4f-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8cc4f-104">JSON representation</span></span>

<span data-ttu-id="8cc4f-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cc4f-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="8cc4f-106">属性</span><span class="sxs-lookup"><span data-stu-id="8cc4f-106">Properties</span></span>
| <span data-ttu-id="8cc4f-107">属性</span><span class="sxs-lookup"><span data-stu-id="8cc4f-107">Property</span></span>     | <span data-ttu-id="8cc4f-108">类型</span><span class="sxs-lookup"><span data-stu-id="8cc4f-108">Type</span></span>   |<span data-ttu-id="8cc4f-109">说明</span><span class="sxs-lookup"><span data-stu-id="8cc4f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cc4f-110">类型</span><span class="sxs-lookup"><span data-stu-id="8cc4f-110">type</span></span>|<span data-ttu-id="8cc4f-111">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="8cc4f-111">AttendeeType</span></span>| <span data-ttu-id="8cc4f-112">与会者类型。</span><span class="sxs-lookup"><span data-stu-id="8cc4f-112">The type of attendee.</span></span> <span data-ttu-id="8cc4f-113">可取值为：`required`、`optional`、`resource`。</span><span class="sxs-lookup"><span data-stu-id="8cc4f-113">The possible values are `required`, `optional`, `resource`, , , , , , , , , or .</span></span> <span data-ttu-id="8cc4f-114">当前如果与会者是一个人，[findMeetingTimes](../api/user_findmeetingtimes.md) 始终认为这个人是 `Required` 类型。</span><span class="sxs-lookup"><span data-stu-id="8cc4f-114">The type of attendee. Possible values are: , , . Currently if the attendee is a person, [findMeetingTimes](../api/user_findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="8cc4f-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8cc4f-115">emailAddress</span></span>|[<span data-ttu-id="8cc4f-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8cc4f-116">emailAddress</span></span>](emailAddress.md)|<span data-ttu-id="8cc4f-117">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="8cc4f-117">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
