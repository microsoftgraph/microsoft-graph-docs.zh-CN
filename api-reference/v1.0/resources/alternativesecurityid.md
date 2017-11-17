# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="02b49-101">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="02b49-101">alternativeSecurityId resource type</span></span>

<span data-ttu-id="02b49-p101">包含与设备相关的可选安全 ID。[设备](device.md) 实体的 **AlternativeSecurityIds** 属性是一个 **alternativeSecurityId** 集合。</span><span class="sxs-lookup"><span data-stu-id="02b49-p101">Contains an alternative security ID associated with a device. The **alternativeSecurityIds** property of the [Device](device.md) entity is a collection of **alternativeSecurityId**.</span></span>

## <a name="properties"></a><span data-ttu-id="02b49-104">属性</span><span class="sxs-lookup"><span data-stu-id="02b49-104">Properties</span></span>
| <span data-ttu-id="02b49-105">属性</span><span class="sxs-lookup"><span data-stu-id="02b49-105">Property</span></span>     | <span data-ttu-id="02b49-106">类型</span><span class="sxs-lookup"><span data-stu-id="02b49-106">Type</span></span>   |<span data-ttu-id="02b49-107">说明</span><span class="sxs-lookup"><span data-stu-id="02b49-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02b49-108">identityProvider</span><span class="sxs-lookup"><span data-stu-id="02b49-108">identityProvider</span></span>|<span data-ttu-id="02b49-109">String</span><span class="sxs-lookup"><span data-stu-id="02b49-109">String</span></span>|            |
|<span data-ttu-id="02b49-110">key</span><span class="sxs-lookup"><span data-stu-id="02b49-110">key</span></span>|<span data-ttu-id="02b49-111">二进制</span><span class="sxs-lookup"><span data-stu-id="02b49-111">Binary</span></span>|            |
|<span data-ttu-id="02b49-112">类型</span><span class="sxs-lookup"><span data-stu-id="02b49-112">type</span></span>|<span data-ttu-id="02b49-113">Int32</span><span class="sxs-lookup"><span data-stu-id="02b49-113">Int32</span></span>|            |

## <a name="json-representation"></a><span data-ttu-id="02b49-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02b49-114">JSON representation</span></span>

<span data-ttu-id="02b49-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02b49-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "identityProvider": "string",
  "key": "binary",
  "type": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alternativeSecurityId resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
