# <a name="operationerror-resource-type"></a><span data-ttu-id="5dbbc-101">operationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="5dbbc-101">operationError resource type</span></span>



<span data-ttu-id="5dbbc-102">介绍[teamsAsyncOperation](teamsasyncoperation.md)中的错误。</span><span class="sxs-lookup"><span data-stu-id="5dbbc-102">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="5dbbc-103">operationError 属性</span><span class="sxs-lookup"><span data-stu-id="5dbbc-103">operationError Properties</span></span>
| <span data-ttu-id="5dbbc-104">属性</span><span class="sxs-lookup"><span data-stu-id="5dbbc-104">Property</span></span>     | <span data-ttu-id="5dbbc-105">类型</span><span class="sxs-lookup"><span data-stu-id="5dbbc-105">Type</span></span>   |<span data-ttu-id="5dbbc-106">说明</span><span class="sxs-lookup"><span data-stu-id="5dbbc-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dbbc-107">code</span><span class="sxs-lookup"><span data-stu-id="5dbbc-107">code</span></span>|<span data-ttu-id="5dbbc-108">字符串 （只读）</span><span class="sxs-lookup"><span data-stu-id="5dbbc-108">string (readonly)</span></span>|<span data-ttu-id="5dbbc-109">操作错误代码。</span><span class="sxs-lookup"><span data-stu-id="5dbbc-109">Operation error code.</span></span>|
|<span data-ttu-id="5dbbc-110">message</span><span class="sxs-lookup"><span data-stu-id="5dbbc-110">message</span></span>|<span data-ttu-id="5dbbc-111">字符串 （只读）</span><span class="sxs-lookup"><span data-stu-id="5dbbc-111">string (readonly)</span></span>|<span data-ttu-id="5dbbc-112">操作错误消息。</span><span class="sxs-lookup"><span data-stu-id="5dbbc-112">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5dbbc-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5dbbc-113">JSON representation</span></span>

<span data-ttu-id="5dbbc-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5dbbc-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
