# <a name="driveitemversion-resource-type"></a><span data-ttu-id="061c8-101">DriveItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="061c8-101">DriveItemVersion resource type</span></span>

<span data-ttu-id="061c8-102">**DriveItemVersion** 资源表示特定版本的 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="061c8-102">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="061c8-103">DriveItemVersion 资源上的任务</span><span class="sxs-lookup"><span data-stu-id="061c8-103">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="061c8-104">下列任务可用于 driveItemVersion 资源。</span><span class="sxs-lookup"><span data-stu-id="061c8-104">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="061c8-105">常见任务</span><span class="sxs-lookup"><span data-stu-id="061c8-105">Common task</span></span>             |         <span data-ttu-id="061c8-106">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="061c8-106">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="061c8-107">[列出版本][version-list]</span><span class="sxs-lookup"><span data-stu-id="061c8-107">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="061c8-108">[获取版本][version-get]</span><span class="sxs-lookup"><span data-stu-id="061c8-108">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="061c8-109">[获取内容][content-get]</span><span class="sxs-lookup"><span data-stu-id="061c8-109">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="061c8-110">[还原版本][version-restore]</span><span class="sxs-lookup"><span data-stu-id="061c8-110">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem_list_versions.md
[version-get]: ../api/driveitemversion_get.md
[content-get]: ../api/driveitemversion_get_contents.md
[version-restore]: ../api/driveitemversion_restore.md

<span data-ttu-id="061c8-111">在上表中，各示例使用的是 `/drive`，但有很多有效的请求。</span><span class="sxs-lookup"><span data-stu-id="061c8-111">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="061c8-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="061c8-112">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "@type.aka": "oneDrive.driveItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" },
  "size": 12356
}
```

## <a name="properties"></a><span data-ttu-id="061c8-113">属性</span><span class="sxs-lookup"><span data-stu-id="061c8-113">Properties</span></span>

|      <span data-ttu-id="061c8-114">属性名称</span><span class="sxs-lookup"><span data-stu-id="061c8-114">Property name</span></span>       |                         <span data-ttu-id="061c8-115">类型</span><span class="sxs-lookup"><span data-stu-id="061c8-115">Type</span></span>                         |                               <span data-ttu-id="061c8-116">说明</span><span class="sxs-lookup"><span data-stu-id="061c8-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="061c8-117">**id**</span><span class="sxs-lookup"><span data-stu-id="061c8-117">**id**</span></span>                   | <span data-ttu-id="061c8-118">字符串</span><span class="sxs-lookup"><span data-stu-id="061c8-118">string</span></span>                                               | <span data-ttu-id="061c8-119">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="061c8-119">The ID of the version.</span></span> <span data-ttu-id="061c8-120">只读。</span><span class="sxs-lookup"><span data-stu-id="061c8-120">Read-only.</span></span>                                       |
| <span data-ttu-id="061c8-121">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="061c8-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="061c8-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="061c8-122">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="061c8-123">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="061c8-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="061c8-124">只读。</span><span class="sxs-lookup"><span data-stu-id="061c8-124">Read-only.</span></span>        |
| <span data-ttu-id="061c8-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="061c8-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="061c8-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="061c8-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="061c8-127">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="061c8-127">Date and time the version was last modified.</span></span> <span data-ttu-id="061c8-128">只读。</span><span class="sxs-lookup"><span data-stu-id="061c8-128">Read-only.</span></span>                 |
| <span data-ttu-id="061c8-129">**publication**</span><span class="sxs-lookup"><span data-stu-id="061c8-129">**publication**</span></span>          | [<span data-ttu-id="061c8-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="061c8-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="061c8-131">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="061c8-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="061c8-132">只读。</span><span class="sxs-lookup"><span data-stu-id="061c8-132">Read-only.</span></span> |
| <span data-ttu-id="061c8-133">**size**</span><span class="sxs-lookup"><span data-stu-id="061c8-133">**size**</span></span>                 | <span data-ttu-id="061c8-134">Int64</span><span class="sxs-lookup"><span data-stu-id="061c8-134">Int64</span></span>                                                | <span data-ttu-id="061c8-135">指示此版本项的内容流大小。</span><span class="sxs-lookup"><span data-stu-id="061c8-135">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="061c8-136">**content**</span><span class="sxs-lookup"><span data-stu-id="061c8-136">**content**</span></span>              | <span data-ttu-id="061c8-137">Stream</span><span class="sxs-lookup"><span data-stu-id="061c8-137">Stream</span></span>                                               | <span data-ttu-id="061c8-138">此版本项的内容流。</span><span class="sxs-lookup"><span data-stu-id="061c8-138">Indicates the size of the content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
