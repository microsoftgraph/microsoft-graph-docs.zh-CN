# <a name="baseitemversion-resource-type"></a><span data-ttu-id="640a3-101">BaseItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="640a3-101">BaseItemVersion resource type</span></span>

<span data-ttu-id="640a3-102">**baseItemVersion** 资源表示项或实体的以前版本。</span><span class="sxs-lookup"><span data-stu-id="640a3-102">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="640a3-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="640a3-103">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="640a3-104">属性</span><span class="sxs-lookup"><span data-stu-id="640a3-104">Properties</span></span>

|      <span data-ttu-id="640a3-105">属性名称</span><span class="sxs-lookup"><span data-stu-id="640a3-105">Property name</span></span>       |                         <span data-ttu-id="640a3-106">类型</span><span class="sxs-lookup"><span data-stu-id="640a3-106">Type</span></span>                         |                               <span data-ttu-id="640a3-107">说明</span><span class="sxs-lookup"><span data-stu-id="640a3-107">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="640a3-108">**id**</span><span class="sxs-lookup"><span data-stu-id="640a3-108">**id**</span></span>                   | <span data-ttu-id="640a3-109">字符串</span><span class="sxs-lookup"><span data-stu-id="640a3-109">string</span></span>                                               | <span data-ttu-id="640a3-110">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="640a3-110">The ID of the version.</span></span> <span data-ttu-id="640a3-111">只读。</span><span class="sxs-lookup"><span data-stu-id="640a3-111">Read-only.</span></span>                                       |
| <span data-ttu-id="640a3-112">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="640a3-112">**lastModifiedBy**</span></span>       | [<span data-ttu-id="640a3-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="640a3-113">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="640a3-114">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="640a3-114">Identity of the user which last modified the version.</span></span> <span data-ttu-id="640a3-115">只读。</span><span class="sxs-lookup"><span data-stu-id="640a3-115">Read-only.</span></span>        |
| <span data-ttu-id="640a3-116">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="640a3-116">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="640a3-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="640a3-117">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="640a3-118">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="640a3-118">Date and time the version was last modified.</span></span> <span data-ttu-id="640a3-119">只读。</span><span class="sxs-lookup"><span data-stu-id="640a3-119">Read-only.</span></span>                 |
| <span data-ttu-id="640a3-120">**publication**</span><span class="sxs-lookup"><span data-stu-id="640a3-120">**publication**</span></span>          | [<span data-ttu-id="640a3-121">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="640a3-121">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="640a3-122">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="640a3-122">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="640a3-123">只读。</span><span class="sxs-lookup"><span data-stu-id="640a3-123">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
