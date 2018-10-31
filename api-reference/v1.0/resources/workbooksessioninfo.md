# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="23671-101">workbookSessionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="23671-101">workbookSessionInfo resource type</span></span>

<span data-ttu-id="23671-102">提供有关工作簿会话的信息。</span><span class="sxs-lookup"><span data-stu-id="23671-102">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="23671-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23671-103">JSON representation</span></span>

<span data-ttu-id="23671-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23671-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a><span data-ttu-id="23671-105">属性</span><span class="sxs-lookup"><span data-stu-id="23671-105">Properties</span></span>

| <span data-ttu-id="23671-106">属性</span><span class="sxs-lookup"><span data-stu-id="23671-106">Property</span></span> | <span data-ttu-id="23671-107">类型</span><span class="sxs-lookup"><span data-stu-id="23671-107">Type</span></span>  | <span data-ttu-id="23671-108">说明</span><span class="sxs-lookup"><span data-stu-id="23671-108">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="23671-109">id</span><span class="sxs-lookup"><span data-stu-id="23671-109">id</span></span>  | <span data-ttu-id="23671-110">字符串</span><span class="sxs-lookup"><span data-stu-id="23671-110">string</span></span> | <span data-ttu-id="23671-111">工作簿会话 的 ID。</span><span class="sxs-lookup"><span data-stu-id="23671-111">Id of the workbook session.</span></span> |
| <span data-ttu-id="23671-112">persistChanges</span><span class="sxs-lookup"><span data-stu-id="23671-112">persistChanges</span></span> | <span data-ttu-id="23671-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="23671-113">boolean</span></span> |  <span data-ttu-id="23671-114">`true` 对于持续会话，值为 。</span><span class="sxs-lookup"><span data-stu-id="23671-114">`true` for persistent session.</span></span> <span data-ttu-id="23671-115">`false` 对于非持续会话（视图模式），值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="23671-115">`false` for non-persistent session (view mode)</span></span> |

