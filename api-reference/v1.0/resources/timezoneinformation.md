# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="00edf-101">timeZoneInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="00edf-101">timeZoneInformation resource type</span></span>


<span data-ttu-id="00edf-102">表示时区。</span><span class="sxs-lookup"><span data-stu-id="00edf-102">Represents a time zone.</span></span> <span data-ttu-id="00edf-103">支持的格式为 Windows，如果修复了当前已知问题，还支持 [Internet 编号分配机构 (IANA) 时区](https://www.iana.org/time-zones)（也称为 Olson 时区）格式。</span><span class="sxs-lookup"><span data-stu-id="00edf-103">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="00edf-104">属性</span><span class="sxs-lookup"><span data-stu-id="00edf-104">Properties</span></span>
| <span data-ttu-id="00edf-105">属性</span><span class="sxs-lookup"><span data-stu-id="00edf-105">Property</span></span>     | <span data-ttu-id="00edf-106">类型</span><span class="sxs-lookup"><span data-stu-id="00edf-106">Type</span></span>   |<span data-ttu-id="00edf-107">说明</span><span class="sxs-lookup"><span data-stu-id="00edf-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00edf-108">alias</span><span class="sxs-lookup"><span data-stu-id="00edf-108">alias</span></span>|<span data-ttu-id="00edf-109">string</span><span class="sxs-lookup"><span data-stu-id="00edf-109">string</span></span>|<span data-ttu-id="00edf-110">时区标识符。</span><span class="sxs-lookup"><span data-stu-id="00edf-110">An identifier for the time zone.</span></span>|
|<span data-ttu-id="00edf-111">displayName</span><span class="sxs-lookup"><span data-stu-id="00edf-111">displayName</span></span>|<span data-ttu-id="00edf-112">string</span><span class="sxs-lookup"><span data-stu-id="00edf-112">string</span></span>|<span data-ttu-id="00edf-113">表示时区的显示字符串。</span><span class="sxs-lookup"><span data-stu-id="00edf-113">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00edf-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00edf-114">JSON representation</span></span>

<span data-ttu-id="00edf-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00edf-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->