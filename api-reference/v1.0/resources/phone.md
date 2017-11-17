# <a name="phone-resource-type"></a><span data-ttu-id="7b301-101">phone 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b301-101">phone resource type</span></span>

<span data-ttu-id="7b301-102">表示一个电话号码。</span><span class="sxs-lookup"><span data-stu-id="7b301-102">Represents a phone number identified in an item.</span></span>


## <a name="properties"></a><span data-ttu-id="7b301-103">属性</span><span class="sxs-lookup"><span data-stu-id="7b301-103">Properties</span></span>
| <span data-ttu-id="7b301-104">属性</span><span class="sxs-lookup"><span data-stu-id="7b301-104">Property</span></span>     | <span data-ttu-id="7b301-105">类型</span><span class="sxs-lookup"><span data-stu-id="7b301-105">Type</span></span>   |<span data-ttu-id="7b301-106">说明</span><span class="sxs-lookup"><span data-stu-id="7b301-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b301-107">number</span><span class="sxs-lookup"><span data-stu-id="7b301-107">number</span></span>|<span data-ttu-id="7b301-108">string</span><span class="sxs-lookup"><span data-stu-id="7b301-108">string</span></span>|<span data-ttu-id="7b301-109">电话号码。</span><span class="sxs-lookup"><span data-stu-id="7b301-109">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="7b301-110">type</span><span class="sxs-lookup"><span data-stu-id="7b301-110">type</span></span>|<span data-ttu-id="7b301-111">String</span><span class="sxs-lookup"><span data-stu-id="7b301-111">String</span></span>|<span data-ttu-id="7b301-p101">电话号码的类型。可能的值是：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="7b301-p101">The type of phone number. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b301-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b301-114">JSON representation</span></span>

<span data-ttu-id="7b301-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b301-115">Here is a JSON representation of the resource.</span></span>

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