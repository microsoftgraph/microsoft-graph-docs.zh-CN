<span data-ttu-id="f25f3-p102">异步操作类型。其值可以为 *ForceDelete* 或 *Verification*。</span><span class="sxs-lookup"><span data-stu-id="f25f3-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> | 异步操作类型。其值可以为 *ForceDelete* 或 *Verification*。 |
| <span data-ttu-id="f25f3-115">status</span><span class="sxs-lookup"><span data-stu-id="f25f3-115">status</span></span> | <span data-ttu-id="f25f3-116">String</span><span class="sxs-lookup"><span data-stu-id="f25f3-116">String</span></span> | <span data-ttu-id="f25f3-117">操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="f25f3-117">Current status of the operation.</span></span> <br> <span data-ttu-id="f25f3-118">*Scheduled* - 已计划操作但尚未启动。</span><span class="sxs-lookup"><span data-stu-id="f25f3-118">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="f25f3-119">*InProgress* - 任务已启动并且正在进行中。</span><span class="sxs-lookup"><span data-stu-id="f25f3-119">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="f25f3-120">*Failed* - 操作已失败。</span><span class="sxs-lookup"><span data-stu-id="f25f3-120">*Failed* - Operation has failed.</span></span> |

## <span data-ttu-id="f25f3-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f25f3-121">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="f25f3-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f25f3-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->