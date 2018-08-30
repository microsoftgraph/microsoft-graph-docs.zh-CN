# <a name="publicationfacet-resource-type"></a><span data-ttu-id="8b0de-101">PublicationFacet 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b0de-101">PublicationFacet resource type</span></span>

<span data-ttu-id="8b0de-102">**publicationFacet** 资源提供有关 [driveItemVersion](driveitemversion.md) 或 [driveItem](driveitem.md) 资源发布状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8b0de-102">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b0de-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b0de-103">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="8b0de-104">属性</span><span class="sxs-lookup"><span data-stu-id="8b0de-104">Properties</span></span>

|   <span data-ttu-id="8b0de-105">属性</span><span class="sxs-lookup"><span data-stu-id="8b0de-105">Property</span></span>    |  <span data-ttu-id="8b0de-106">类型</span><span class="sxs-lookup"><span data-stu-id="8b0de-106">Type</span></span>  | <span data-ttu-id="8b0de-107">说明</span><span class="sxs-lookup"><span data-stu-id="8b0de-107">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="8b0de-108">**level**</span><span class="sxs-lookup"><span data-stu-id="8b0de-108">**level**</span></span>     | <span data-ttu-id="8b0de-109">字符串</span><span class="sxs-lookup"><span data-stu-id="8b0de-109">String</span></span> | <span data-ttu-id="8b0de-110">此文档的发布状态。</span><span class="sxs-lookup"><span data-stu-id="8b0de-110">The state of publication for this document.</span></span> <span data-ttu-id="8b0de-111">或 `checkout`。`published`</span><span class="sxs-lookup"><span data-stu-id="8b0de-111">Either `published` or `checkout`.</span></span> <span data-ttu-id="8b0de-112">只读。</span><span class="sxs-lookup"><span data-stu-id="8b0de-112">Read-only.</span></span>  |
| <span data-ttu-id="8b0de-113">**versionId**</span><span class="sxs-lookup"><span data-stu-id="8b0de-113">**versionId**</span></span> | <span data-ttu-id="8b0de-114">字符串</span><span class="sxs-lookup"><span data-stu-id="8b0de-114">String</span></span> | <span data-ttu-id="8b0de-115">对当前调用方可见的版本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8b0de-115">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="8b0de-116">只读。</span><span class="sxs-lookup"><span data-stu-id="8b0de-116">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->
