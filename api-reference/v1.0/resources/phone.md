# <a name="phone-resource-type"></a><span data-ttu-id="16449-101">phone 资源类型</span><span class="sxs-lookup"><span data-stu-id="16449-101">phone resource type</span></span>

<span data-ttu-id="16449-102">表示一个电话号码。</span><span class="sxs-lookup"><span data-stu-id="16449-102">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="16449-103">属性</span><span class="sxs-lookup"><span data-stu-id="16449-103">Properties</span></span>
| <span data-ttu-id="16449-104">属性</span><span class="sxs-lookup"><span data-stu-id="16449-104">Property</span></span>     | <span data-ttu-id="16449-105">类型</span><span class="sxs-lookup"><span data-stu-id="16449-105">Type</span></span>   |<span data-ttu-id="16449-106">说明</span><span class="sxs-lookup"><span data-stu-id="16449-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16449-107">number</span><span class="sxs-lookup"><span data-stu-id="16449-107">number</span></span>|<span data-ttu-id="16449-108">string</span><span class="sxs-lookup"><span data-stu-id="16449-108">string</span></span>|<span data-ttu-id="16449-109">电话号码。</span><span class="sxs-lookup"><span data-stu-id="16449-109">The phone number.</span></span>|
|<span data-ttu-id="16449-110">type</span><span class="sxs-lookup"><span data-stu-id="16449-110">type</span></span>|<span data-ttu-id="16449-111">phoneType</span><span class="sxs-lookup"><span data-stu-id="16449-111">phoneType values</span></span>|<span data-ttu-id="16449-112">电话号码的类型。</span><span class="sxs-lookup"><span data-stu-id="16449-112">The type of phone number.</span></span> <span data-ttu-id="16449-113">可取值为：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="16449-113">The possible values are `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`, , or .</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16449-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16449-114">JSON representation</span></span>

<span data-ttu-id="16449-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16449-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
