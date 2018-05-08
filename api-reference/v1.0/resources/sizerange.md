# <a name="sizerange-resource-type"></a><span data-ttu-id="ff7cf-101">sizeRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff7cf-101">sizeRange resource type</span></span>


<span data-ttu-id="ff7cf-102">指定传入邮件必须具有的最大大小和最小大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="ff7cf-102">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="ff7cf-103">属性</span><span class="sxs-lookup"><span data-stu-id="ff7cf-103">Properties</span></span>
| <span data-ttu-id="ff7cf-104">属性</span><span class="sxs-lookup"><span data-stu-id="ff7cf-104">Property</span></span>     | <span data-ttu-id="ff7cf-105">类型</span><span class="sxs-lookup"><span data-stu-id="ff7cf-105">Type</span></span>   |<span data-ttu-id="ff7cf-106">说明</span><span class="sxs-lookup"><span data-stu-id="ff7cf-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ff7cf-107">maximumSize</span><span class="sxs-lookup"><span data-stu-id="ff7cf-107">maximumSize</span></span> | <span data-ttu-id="ff7cf-108">Int32</span><span class="sxs-lookup"><span data-stu-id="ff7cf-108">Int32</span></span> | <span data-ttu-id="ff7cf-109">传入邮件必须具有的最大大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="ff7cf-109">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="ff7cf-110">minimumSize</span><span class="sxs-lookup"><span data-stu-id="ff7cf-110">minimumSize</span></span> | <span data-ttu-id="ff7cf-111">Int32</span><span class="sxs-lookup"><span data-stu-id="ff7cf-111">Int32</span></span> | <span data-ttu-id="ff7cf-112">传入邮件必须具有的最小大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="ff7cf-112">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="ff7cf-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff7cf-113">JSON representation</span></span>
<span data-ttu-id="ff7cf-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff7cf-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->