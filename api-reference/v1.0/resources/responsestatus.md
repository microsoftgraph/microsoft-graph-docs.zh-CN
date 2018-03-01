# <a name="responsestatus-resource-type"></a><span data-ttu-id="0e13e-101">responseStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e13e-101">responseStatus resource type</span></span>

<span data-ttu-id="0e13e-102">会议请求的响应状态。</span><span class="sxs-lookup"><span data-stu-id="0e13e-102">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="0e13e-103">属性</span><span class="sxs-lookup"><span data-stu-id="0e13e-103">Properties</span></span>

| <span data-ttu-id="0e13e-104">属性</span><span class="sxs-lookup"><span data-stu-id="0e13e-104">Property</span></span> | <span data-ttu-id="0e13e-105">类型</span><span class="sxs-lookup"><span data-stu-id="0e13e-105">Type</span></span>           | <span data-ttu-id="0e13e-106">说明</span><span class="sxs-lookup"><span data-stu-id="0e13e-106">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="0e13e-107">响应</span><span class="sxs-lookup"><span data-stu-id="0e13e-107">response</span></span> | <span data-ttu-id="0e13e-108">String</span><span class="sxs-lookup"><span data-stu-id="0e13e-108">String</span></span>         | <span data-ttu-id="0e13e-109">响应类型。</span><span class="sxs-lookup"><span data-stu-id="0e13e-109">The response type.</span></span> <span data-ttu-id="0e13e-110">可取值为：`None`、`Organizer`、`TentativelyAccepted`、`Accepted`、`Declined`、`NotResponded`。</span><span class="sxs-lookup"><span data-stu-id="0e13e-110">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="0e13e-111">时间</span><span class="sxs-lookup"><span data-stu-id="0e13e-111">time</span></span>     | <span data-ttu-id="0e13e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e13e-112">DateTimeOffset</span></span> | <span data-ttu-id="0e13e-113">响应返回的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0e13e-113">The date and time that the response was returned.</span></span> <span data-ttu-id="0e13e-114">它使用 ISO 8601 格式，并始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0e13e-114">It uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0e13e-115">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0e13e-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'` Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e13e-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e13e-116">JSON representation</span></span>

<span data-ttu-id="0e13e-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e13e-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
