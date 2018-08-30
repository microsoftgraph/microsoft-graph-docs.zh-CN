# <a name="mailtipserror-resource-type"></a><span data-ttu-id="7b03b-101">mailTipsError 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b03b-101">mailTipsError resource type</span></span>

<span data-ttu-id="7b03b-102">操作过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="7b03b-102">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="7b03b-103">属性</span><span class="sxs-lookup"><span data-stu-id="7b03b-103">Properties</span></span>
| <span data-ttu-id="7b03b-104">属性</span><span class="sxs-lookup"><span data-stu-id="7b03b-104">Property</span></span>     | <span data-ttu-id="7b03b-105">类型</span><span class="sxs-lookup"><span data-stu-id="7b03b-105">Type</span></span>   |<span data-ttu-id="7b03b-106">说明</span><span class="sxs-lookup"><span data-stu-id="7b03b-106">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="7b03b-107">消息</span><span class="sxs-lookup"><span data-stu-id="7b03b-107">message</span></span> | <span data-ttu-id="7b03b-108">字符串</span><span class="sxs-lookup"><span data-stu-id="7b03b-108">String</span></span> | <span data-ttu-id="7b03b-109">错误消息。</span><span class="sxs-lookup"><span data-stu-id="7b03b-109">The error message.</span></span> |
| <span data-ttu-id="7b03b-110">code</span><span class="sxs-lookup"><span data-stu-id="7b03b-110">code</span></span> | <span data-ttu-id="7b03b-111">字符串</span><span class="sxs-lookup"><span data-stu-id="7b03b-111">String</span></span> | <span data-ttu-id="7b03b-112">错误代码。</span><span class="sxs-lookup"><span data-stu-id="7b03b-112">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7b03b-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b03b-113">JSON representation</span></span>

<span data-ttu-id="7b03b-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b03b-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->