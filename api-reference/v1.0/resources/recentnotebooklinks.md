# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="864c8-101">recentNotebookLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="864c8-101">recentNotebookLinks resource type</span></span>

<span data-ttu-id="864c8-102">用于打开 OneNote 笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="864c8-102">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="864c8-103">此资源类型以 [recentNotebook](recentnotebook.md) 资源属性的形式存在。</span><span class="sxs-lookup"><span data-stu-id="864c8-103">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="864c8-104">属性</span><span class="sxs-lookup"><span data-stu-id="864c8-104">Properties</span></span>
| <span data-ttu-id="864c8-105">属性</span><span class="sxs-lookup"><span data-stu-id="864c8-105">Property</span></span>     | <span data-ttu-id="864c8-106">类型</span><span class="sxs-lookup"><span data-stu-id="864c8-106">Type</span></span>   |<span data-ttu-id="864c8-107">说明</span><span class="sxs-lookup"><span data-stu-id="864c8-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="864c8-108">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="864c8-108">oneNoteClientUrl</span></span>|[<span data-ttu-id="864c8-109">externalLink</span><span class="sxs-lookup"><span data-stu-id="864c8-109">externalLink</span></span>](externallink.md)|<span data-ttu-id="864c8-110">如果安装了 OneNote 本机客户端，则在其中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="864c8-110">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="864c8-111">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="864c8-111">oneNoteWebUrl</span></span>|[<span data-ttu-id="864c8-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="864c8-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="864c8-113">在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="864c8-113">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="864c8-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="864c8-114">JSON representation</span></span>

<span data-ttu-id="864c8-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="864c8-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
