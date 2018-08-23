# <a name="operation-resource-type"></a><span data-ttu-id="270ad-101">操作资源类型</span><span class="sxs-lookup"><span data-stu-id="270ad-101">operation resource type</span></span>

<span data-ttu-id="270ad-102">长时间运行操作的状态。</span><span class="sxs-lookup"><span data-stu-id="270ad-102">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="270ad-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="270ad-103">JSON representation</span></span>

<span data-ttu-id="270ad-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="270ad-104">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}

```
## <a name="properties"></a><span data-ttu-id="270ad-105">属性</span><span class="sxs-lookup"><span data-stu-id="270ad-105">Properties</span></span>
| <span data-ttu-id="270ad-106">属性</span><span class="sxs-lookup"><span data-stu-id="270ad-106">Property</span></span>     | <span data-ttu-id="270ad-107">类型</span><span class="sxs-lookup"><span data-stu-id="270ad-107">Type</span></span>   |<span data-ttu-id="270ad-108">说明</span><span class="sxs-lookup"><span data-stu-id="270ad-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="270ad-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="270ad-109">createdDateTime</span></span>| <span data-ttu-id="270ad-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="270ad-110">DateTimeOffset</span></span> |<span data-ttu-id="270ad-111">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="270ad-111">The start time of the operation.</span></span>|
|<span data-ttu-id="270ad-112">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="270ad-112">lastActionDateTime</span></span>| <span data-ttu-id="270ad-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="270ad-113">DateTimeOffset</span></span> |<span data-ttu-id="270ad-114">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="270ad-114">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="270ad-115">status</span><span class="sxs-lookup"><span data-stu-id="270ad-115">status</span></span>|<span data-ttu-id="270ad-116">operationStatus</span><span class="sxs-lookup"><span data-stu-id="270ad-116">operationStatus</span></span>|<span data-ttu-id="270ad-117">操作的当前状态：`notStarted`、`running`、`completed`。 `failed`</span><span class="sxs-lookup"><span data-stu-id="270ad-117">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
