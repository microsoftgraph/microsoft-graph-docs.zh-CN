# <a name="outlookitem-resource-type"></a><span data-ttu-id="baeaf-101">outlookItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="baeaf-101">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="baeaf-102">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="baeaf-102">JSON representation</span></span>

<span data-ttu-id="baeaf-103">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="baeaf-103">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookItem"
}-->

```json
{
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="baeaf-104">属性</span><span class="sxs-lookup"><span data-stu-id="baeaf-104">Properties</span></span>
| <span data-ttu-id="baeaf-105">属性</span><span class="sxs-lookup"><span data-stu-id="baeaf-105">Property</span></span>     | <span data-ttu-id="baeaf-106">类型</span><span class="sxs-lookup"><span data-stu-id="baeaf-106">Type</span></span>   |<span data-ttu-id="baeaf-107">说明</span><span class="sxs-lookup"><span data-stu-id="baeaf-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="baeaf-108">分类</span><span class="sxs-lookup"><span data-stu-id="baeaf-108">categories</span></span>|<span data-ttu-id="baeaf-109">字符串集合</span><span class="sxs-lookup"><span data-stu-id="baeaf-109">String collection</span></span>|<span data-ttu-id="baeaf-110">与项目关联的类别</span><span class="sxs-lookup"><span data-stu-id="baeaf-110">The categories associated with the message.</span></span>|
|<span data-ttu-id="baeaf-111">changeKey</span><span class="sxs-lookup"><span data-stu-id="baeaf-111">changeKey</span></span>|<span data-ttu-id="baeaf-112">字符串</span><span class="sxs-lookup"><span data-stu-id="baeaf-112">String</span></span>|<span data-ttu-id="baeaf-113">标识项目的版本。</span><span class="sxs-lookup"><span data-stu-id="baeaf-113">Identifies the version of the contact.</span></span> <span data-ttu-id="baeaf-114">每次联系人发生变化时，ChangeKey 都会更改。</span><span class="sxs-lookup"><span data-stu-id="baeaf-114">Every time the contact is changed, ChangeKey  changes as well.</span></span> <span data-ttu-id="baeaf-115">它使得 Exchange 能将更改应用于正确版本的对象。</span><span class="sxs-lookup"><span data-stu-id="baeaf-115">Identifies the version of the reminder. Every time the reminder is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="baeaf-116">只读。</span><span class="sxs-lookup"><span data-stu-id="baeaf-116">Read-only.</span></span>|
|<span data-ttu-id="baeaf-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="baeaf-117">createdDateTime</span></span>|<span data-ttu-id="baeaf-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baeaf-118">DateTimeOffset</span></span>|<span data-ttu-id="baeaf-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示： `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="baeaf-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="baeaf-121">id</span><span class="sxs-lookup"><span data-stu-id="baeaf-121">id</span></span>|<span data-ttu-id="baeaf-122">字符串</span><span class="sxs-lookup"><span data-stu-id="baeaf-122">String</span></span>| <span data-ttu-id="baeaf-123">只读。</span><span class="sxs-lookup"><span data-stu-id="baeaf-123">Read-only.</span></span>|
|<span data-ttu-id="baeaf-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="baeaf-124">lastModifiedDateTime</span></span>|<span data-ttu-id="baeaf-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baeaf-125">DateTimeOffset</span></span>|<span data-ttu-id="baeaf-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示： `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="baeaf-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="baeaf-128">关系</span><span class="sxs-lookup"><span data-stu-id="baeaf-128">Relationships</span></span>
<span data-ttu-id="baeaf-129">无</span><span class="sxs-lookup"><span data-stu-id="baeaf-129">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
