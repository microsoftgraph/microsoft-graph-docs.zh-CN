# <a name="timezonebase-resource-type"></a><span data-ttu-id="64ddb-101">timeZoneBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="64ddb-101">timeZoneBase resource type</span></span>

<span data-ttu-id="64ddb-102">时区的基本表示形式。</span><span class="sxs-lookup"><span data-stu-id="64ddb-102">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="64ddb-103">属性</span><span class="sxs-lookup"><span data-stu-id="64ddb-103">Properties</span></span>
| <span data-ttu-id="64ddb-104">属性</span><span class="sxs-lookup"><span data-stu-id="64ddb-104">Property</span></span>     | <span data-ttu-id="64ddb-105">类型</span><span class="sxs-lookup"><span data-stu-id="64ddb-105">Type</span></span>   |<span data-ttu-id="64ddb-106">说明</span><span class="sxs-lookup"><span data-stu-id="64ddb-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="64ddb-107">name</span><span class="sxs-lookup"><span data-stu-id="64ddb-107">name</span></span> | <span data-ttu-id="64ddb-108">string</span><span class="sxs-lookup"><span data-stu-id="64ddb-108">string</span></span> | <span data-ttu-id="64ddb-109">时区的名称。</span><span class="sxs-lookup"><span data-stu-id="64ddb-109">The name of a time zone.</span></span> <span data-ttu-id="64ddb-110">它可以是一个标准时区名称，例如“夏威夷-阿留申标准时间”，或自定义时区的“自定义时区”。</span><span class="sxs-lookup"><span data-stu-id="64ddb-110">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="64ddb-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64ddb-111">JSON representation</span></span>

<span data-ttu-id="64ddb-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64ddb-112">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->