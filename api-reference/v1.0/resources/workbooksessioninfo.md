# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="64450-101">workbookSessionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="64450-101">workbookSessionInfo resource type</span></span>

<span data-ttu-id="64450-102">提供有关工作簿会话的信息。</span><span class="sxs-lookup"><span data-stu-id="64450-102">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="64450-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64450-103">JSON representation</span></span>

<span data-ttu-id="64450-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64450-104">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="64450-105">属性</span><span class="sxs-lookup"><span data-stu-id="64450-105">Properties</span></span>

| <span data-ttu-id="64450-106">属性</span><span class="sxs-lookup"><span data-stu-id="64450-106">Property</span></span> | <span data-ttu-id="64450-107">类型</span><span class="sxs-lookup"><span data-stu-id="64450-107">Type</span></span>  | <span data-ttu-id="64450-108">说明</span><span class="sxs-lookup"><span data-stu-id="64450-108">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="64450-109">id</span><span class="sxs-lookup"><span data-stu-id="64450-109">id</span></span>  | <span data-ttu-id="64450-110">string</span><span class="sxs-lookup"><span data-stu-id="64450-110">string</span></span> | <span data-ttu-id="64450-111">工作簿会话 的 ID。</span><span class="sxs-lookup"><span data-stu-id="64450-111">Id of the workbook session.</span></span> |
| <span data-ttu-id="64450-112">persistChanges</span><span class="sxs-lookup"><span data-stu-id="64450-112">persistChanges</span></span> | <span data-ttu-id="64450-113">string</span><span class="sxs-lookup"><span data-stu-id="64450-113">string</span></span> |  <span data-ttu-id="64450-114">对于持续会话，值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="64450-114">`true` for persistent session.</span></span> <span data-ttu-id="64450-115">对于非持续会话（视图模式），值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="64450-115">`false` for non-persistent session (view mode)</span></span> |

