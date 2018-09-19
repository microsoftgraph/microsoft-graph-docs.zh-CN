# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="e31db-101">automaticRepliesMailTips 资源类型</span><span class="sxs-lookup"><span data-stu-id="e31db-101">automaticRepliesMailTips resource type</span></span>


<span data-ttu-id="e31db-102">与已在邮箱上设置的任何自动答复有关的[邮件提醒](../resources/mailtips.md) 。</span><span class="sxs-lookup"><span data-stu-id="e31db-102">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="e31db-103">属性</span><span class="sxs-lookup"><span data-stu-id="e31db-103">Properties</span></span>
| <span data-ttu-id="e31db-104">属性</span><span class="sxs-lookup"><span data-stu-id="e31db-104">Property</span></span>     | <span data-ttu-id="e31db-105">类型</span><span class="sxs-lookup"><span data-stu-id="e31db-105">Type</span></span>   |<span data-ttu-id="e31db-106">说明</span><span class="sxs-lookup"><span data-stu-id="e31db-106">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="e31db-107">message</span><span class="sxs-lookup"><span data-stu-id="e31db-107">message</span></span> | <span data-ttu-id="e31db-108">String</span><span class="sxs-lookup"><span data-stu-id="e31db-108">String</span></span> | <span data-ttu-id="e31db-109">自动回复消息。</span><span class="sxs-lookup"><span data-stu-id="e31db-109">The automatic reply message.</span></span> |
| <span data-ttu-id="e31db-110">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="e31db-110">messageLanguage</span></span> | [<span data-ttu-id="e31db-111">localeInfo</span><span class="sxs-lookup"><span data-stu-id="e31db-111">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="e31db-112">自动回复消息所使用的语言。</span><span class="sxs-lookup"><span data-stu-id="e31db-112">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="e31db-113">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="e31db-113">ScheduledEndTime</span></span> | [<span data-ttu-id="e31db-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e31db-114">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="e31db-115">设置自动答复结束的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e31db-115">The date and time that automatic replies are set to end, if Status is set to .</span></span> |
| <span data-ttu-id="e31db-116">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="e31db-116">ScheduledStartTime</span></span> | [<span data-ttu-id="e31db-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e31db-117">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="e31db-118">设置自动答复开始的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e31db-118">The date and time that automatic replies are set to begin, if Status is set to .</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e31db-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e31db-119">JSON representation</span></span>

<span data-ttu-id="e31db-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e31db-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->