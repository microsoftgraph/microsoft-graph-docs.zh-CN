# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="251f3-101">mailboxSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="251f3-101">mailboxSettings resource type</span></span>

<span data-ttu-id="251f3-102">已登录用户的主邮箱的设置。</span><span class="sxs-lookup"><span data-stu-id="251f3-102">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="251f3-103">属性</span><span class="sxs-lookup"><span data-stu-id="251f3-103">Properties</span></span>
| <span data-ttu-id="251f3-104">属性</span><span class="sxs-lookup"><span data-stu-id="251f3-104">Property</span></span>     | <span data-ttu-id="251f3-105">类型</span><span class="sxs-lookup"><span data-stu-id="251f3-105">Type</span></span>   |<span data-ttu-id="251f3-106">说明</span><span class="sxs-lookup"><span data-stu-id="251f3-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="251f3-107">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="251f3-107">archiveFolder</span></span>|<span data-ttu-id="251f3-108">string</span><span class="sxs-lookup"><span data-stu-id="251f3-108">string</span></span>|<span data-ttu-id="251f3-109">用户存档文件夹的文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="251f3-109">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="251f3-110">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="251f3-110">automaticRepliesSetting</span></span>|[<span data-ttu-id="251f3-111">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="251f3-111">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="251f3-112">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="251f3-112">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="251f3-113">语言</span><span class="sxs-lookup"><span data-stu-id="251f3-113">language</span></span>|[<span data-ttu-id="251f3-114">localeInfo</span><span class="sxs-lookup"><span data-stu-id="251f3-114">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="251f3-115">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="251f3-115">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="251f3-116">timeZone</span><span class="sxs-lookup"><span data-stu-id="251f3-116">timeZone</span></span>|<span data-ttu-id="251f3-117">string</span><span class="sxs-lookup"><span data-stu-id="251f3-117">string</span></span>|<span data-ttu-id="251f3-118">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="251f3-118">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="251f3-119">workingHours</span><span class="sxs-lookup"><span data-stu-id="251f3-119">workingHours</span></span>|[<span data-ttu-id="251f3-120">workingHours</span><span class="sxs-lookup"><span data-stu-id="251f3-120">workingHours</span></span>](workinghours.md)|<span data-ttu-id="251f3-121">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="251f3-121">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="251f3-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="251f3-122">JSON representation</span></span>

<span data-ttu-id="251f3-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="251f3-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "archiveFolder"
  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "archiveFolder": "string",
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->