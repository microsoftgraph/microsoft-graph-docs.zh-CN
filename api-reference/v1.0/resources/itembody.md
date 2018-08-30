# <a name="itembody-resource-type"></a><span data-ttu-id="bcb33-101">itemBody 资源类型</span><span class="sxs-lookup"><span data-stu-id="bcb33-101">itemBody resource type</span></span>

<span data-ttu-id="bcb33-102">表示项目正文的属性，例如邮件、事件或组帖子。</span><span class="sxs-lookup"><span data-stu-id="bcb33-102">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="bcb33-103">属性</span><span class="sxs-lookup"><span data-stu-id="bcb33-103">Properties</span></span>
| <span data-ttu-id="bcb33-104">属性</span><span class="sxs-lookup"><span data-stu-id="bcb33-104">Property</span></span>     | <span data-ttu-id="bcb33-105">类型</span><span class="sxs-lookup"><span data-stu-id="bcb33-105">Type</span></span>   |<span data-ttu-id="bcb33-106">说明</span><span class="sxs-lookup"><span data-stu-id="bcb33-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcb33-107">内容</span><span class="sxs-lookup"><span data-stu-id="bcb33-107">content</span></span>|<span data-ttu-id="bcb33-108">字符串</span><span class="sxs-lookup"><span data-stu-id="bcb33-108">String</span></span>|<span data-ttu-id="bcb33-109">项目的内容。</span><span class="sxs-lookup"><span data-stu-id="bcb33-109">The content of the item.</span></span>|
|<span data-ttu-id="bcb33-110">contentType</span><span class="sxs-lookup"><span data-stu-id="bcb33-110">contentType</span></span>|<span data-ttu-id="bcb33-111">BodyType</span><span class="sxs-lookup"><span data-stu-id="bcb33-111">BodyType</span></span>|<span data-ttu-id="bcb33-p101">内容的类型。可能的值为 `Text` 和 `HTML`。</span><span class="sxs-lookup"><span data-stu-id="bcb33-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bcb33-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bcb33-114">JSON representation</span></span>

<span data-ttu-id="bcb33-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bcb33-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
