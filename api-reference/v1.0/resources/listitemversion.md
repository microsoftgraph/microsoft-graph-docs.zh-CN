# <a name="listitemversion-resource-type"></a><span data-ttu-id="64ea5-101">ListItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="64ea5-101">ListItemVersion resource type</span></span>

<span data-ttu-id="64ea5-102">**listItemVersion** 资源表示先前版本的 [ListItem](listitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="64ea5-102">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="64ea5-103">ListItemVersion 资源上的任务</span><span class="sxs-lookup"><span data-stu-id="64ea5-103">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="64ea5-104">下列任务可用于 listItemVersion 资源。</span><span class="sxs-lookup"><span data-stu-id="64ea5-104">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="64ea5-105">常见任务</span><span class="sxs-lookup"><span data-stu-id="64ea5-105">Common task</span></span>             |         <span data-ttu-id="64ea5-106">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="64ea5-106">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="64ea5-107">[列出版本][version-list]</span><span class="sxs-lookup"><span data-stu-id="64ea5-107">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="64ea5-108">[获取版本][version-get]</span><span class="sxs-lookup"><span data-stu-id="64ea5-108">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="64ea5-109">[还原版本][version-restore]</span><span class="sxs-lookup"><span data-stu-id="64ea5-109">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem_list_versions.md
[version-get]: ../api/listitemversion_get.md
[version-restore]: ../api/listitemversion_restore.md


## <a name="json-representation"></a><span data-ttu-id="64ea5-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64ea5-110">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.listItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="64ea5-111">属性</span><span class="sxs-lookup"><span data-stu-id="64ea5-111">Properties</span></span>

|      <span data-ttu-id="64ea5-112">属性名称</span><span class="sxs-lookup"><span data-stu-id="64ea5-112">Property name</span></span>       |                         <span data-ttu-id="64ea5-113">类型</span><span class="sxs-lookup"><span data-stu-id="64ea5-113">Type</span></span>                         |                               <span data-ttu-id="64ea5-114">说明</span><span class="sxs-lookup"><span data-stu-id="64ea5-114">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="64ea5-115">**ID**</span><span class="sxs-lookup"><span data-stu-id="64ea5-115">**id**</span></span>                   | <span data-ttu-id="64ea5-116">字符串</span><span class="sxs-lookup"><span data-stu-id="64ea5-116">string</span></span>                                               | <span data-ttu-id="64ea5-117">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="64ea5-117">The ID of the version.</span></span> <span data-ttu-id="64ea5-118">只读。</span><span class="sxs-lookup"><span data-stu-id="64ea5-118">Read-only.</span></span>                                       |
| <span data-ttu-id="64ea5-119">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="64ea5-119">**lastModifiedBy**</span></span>       | [<span data-ttu-id="64ea5-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="64ea5-120">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="64ea5-121">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="64ea5-121">Identity of the user which last modified the version.</span></span> <span data-ttu-id="64ea5-122">只读。</span><span class="sxs-lookup"><span data-stu-id="64ea5-122">Read-only.</span></span>        |
| <span data-ttu-id="64ea5-123">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="64ea5-123">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="64ea5-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64ea5-124">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="64ea5-125">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="64ea5-125">Date and time the version was last modified.</span></span> <span data-ttu-id="64ea5-126">只读。</span><span class="sxs-lookup"><span data-stu-id="64ea5-126">Read-only.</span></span>                 |
| <span data-ttu-id="64ea5-127">**published**</span><span class="sxs-lookup"><span data-stu-id="64ea5-127">**published**</span></span>            | [<span data-ttu-id="64ea5-128">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="64ea5-128">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="64ea5-129">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="64ea5-129">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="64ea5-130">只读。</span><span class="sxs-lookup"><span data-stu-id="64ea5-130">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="64ea5-131">关系</span><span class="sxs-lookup"><span data-stu-id="64ea5-131">Relationships</span></span>

<span data-ttu-id="64ea5-132">下表定义了 **driveItemVersion** 资源与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="64ea5-132">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="64ea5-133">关系名称</span><span class="sxs-lookup"><span data-stu-id="64ea5-133">Relationship name</span></span> |                      <span data-ttu-id="64ea5-134">类型</span><span class="sxs-lookup"><span data-stu-id="64ea5-134">Type</span></span>                      |                               <span data-ttu-id="64ea5-135">说明</span><span class="sxs-lookup"><span data-stu-id="64ea5-135">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="64ea5-136">**字段**</span><span class="sxs-lookup"><span data-stu-id="64ea5-136">**fields**</span></span>        | [<span data-ttu-id="64ea5-137">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="64ea5-137">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="64ea5-138">此版本列表项的字段和值集合。</span><span class="sxs-lookup"><span data-stu-id="64ea5-138">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
