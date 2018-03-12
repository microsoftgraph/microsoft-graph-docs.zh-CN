# <a name="location-resource-type"></a><span data-ttu-id="12c01-101">位置资源类型</span><span class="sxs-lookup"><span data-stu-id="12c01-101">Location resource type</span></span>

<span data-ttu-id="12c01-102">表示事件的位置信息。</span><span class="sxs-lookup"><span data-stu-id="12c01-102">Represents location information of an event.</span></span>


## <a name="properties"></a><span data-ttu-id="12c01-103">属性</span><span class="sxs-lookup"><span data-stu-id="12c01-103">Properties</span></span>
| <span data-ttu-id="12c01-104">属性</span><span class="sxs-lookup"><span data-stu-id="12c01-104">Property</span></span>  | <span data-ttu-id="12c01-105">类型</span><span class="sxs-lookup"><span data-stu-id="12c01-105">Type</span></span>   | <span data-ttu-id="12c01-106">说明</span><span class="sxs-lookup"><span data-stu-id="12c01-106">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="12c01-107">address</span><span class="sxs-lookup"><span data-stu-id="12c01-107">address</span></span> | [<span data-ttu-id="12c01-108">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="12c01-108">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="12c01-109">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="12c01-109">The street address of the location.</span></span> |
| <span data-ttu-id="12c01-110">displayName</span><span class="sxs-lookup"><span data-stu-id="12c01-110">displayName</span></span>  | <span data-ttu-id="12c01-111">String</span><span class="sxs-lookup"><span data-stu-id="12c01-111">String</span></span> | <span data-ttu-id="12c01-112">与地点相关联的名称。</span><span class="sxs-lookup"><span data-stu-id="12c01-112">The name associated with the location.</span></span>                       |
| <span data-ttu-id="12c01-113">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="12c01-113">locationEmailAddress</span></span> | <span data-ttu-id="12c01-114">String</span><span class="sxs-lookup"><span data-stu-id="12c01-114">String</span></span> | <span data-ttu-id="12c01-115">（可选）与地点相关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="12c01-115">Optional email address of the location.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="12c01-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12c01-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```

## <a name="remarks"></a><span data-ttu-id="12c01-117">注解</span><span class="sxs-lookup"><span data-stu-id="12c01-117">Remarks</span></span>

<span data-ttu-id="12c01-118">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="12c01-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
