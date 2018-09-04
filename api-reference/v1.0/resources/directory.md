# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="821fc-101">目录资源类型（已删除的项目）</span><span class="sxs-lookup"><span data-stu-id="821fc-101">directory resource type (deleted items)</span></span>

<span data-ttu-id="821fc-102">表示目录中已删除的项目。</span><span class="sxs-lookup"><span data-stu-id="821fc-102">Represents a deleted item in the directory.</span></span> <span data-ttu-id="821fc-103">删除某个项目后，它会被添加到已删除项目“容器”中。</span><span class="sxs-lookup"><span data-stu-id="821fc-103">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="821fc-104">已删除的项目将保留最多 30 天的还原时间。</span><span class="sxs-lookup"><span data-stu-id="821fc-104">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="821fc-105">30 天后，这些项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="821fc-105">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="821fc-106">目前，已删除的项目功能仅支持用于 Office 365 [groups](group.md) 和 [users](users.md)。</span><span class="sxs-lookup"><span data-stu-id="821fc-106">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="821fc-107">方法</span><span class="sxs-lookup"><span data-stu-id="821fc-107">Methods</span></span>

| <span data-ttu-id="821fc-108">方法</span><span class="sxs-lookup"><span data-stu-id="821fc-108">Method</span></span>         | <span data-ttu-id="821fc-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="821fc-109">Return Type</span></span> | <span data-ttu-id="821fc-110">说明</span><span class="sxs-lookup"><span data-stu-id="821fc-110">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="821fc-111">获取已删除项目</span><span class="sxs-lookup"><span data-stu-id="821fc-111">Get deleted item</span></span>](../api/directory_deleteditems_get.md) | [<span data-ttu-id="821fc-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="821fc-112">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="821fc-113">获取已删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="821fc-113">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="821fc-114">还原已删除项目</span><span class="sxs-lookup"><span data-stu-id="821fc-114">Restore deleted item</span></span>](../api/directory_deleteditems_restore.md) |[<span data-ttu-id="821fc-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="821fc-115">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="821fc-116">还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="821fc-116">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="821fc-117">列出已删除项目</span><span class="sxs-lookup"><span data-stu-id="821fc-117">List deleted items</span></span>](../api/directory_deleteditems_list.md) |<span data-ttu-id="821fc-118">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="821fc-118">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="821fc-119">获取最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="821fc-119">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="821fc-120">永久删除项目</span><span class="sxs-lookup"><span data-stu-id="821fc-120">Permanently delete an item</span></span>](../api/directory_deleteditems_delete.md) | <span data-ttu-id="821fc-121">无</span><span class="sxs-lookup"><span data-stu-id="821fc-121">None</span></span> | <span data-ttu-id="821fc-122">永久删除项目。</span><span class="sxs-lookup"><span data-stu-id="821fc-122">Permanently deletes an item.</span></span> |
|<span data-ttu-id="821fc-123">[列出由用户拥有的已删除项目](../api/directory_deleteditems_user_owned.md)</span><span class="sxs-lookup"><span data-stu-id="821fc-123">Added [List deleted items owned by a user](../api/directory_deleteditems_user_owned.md) action to directory (deleted items) resource</span></span> | <span data-ttu-id="821fc-124">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="821fc-124">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="821fc-125">列出了由用户拥有的目录项。</span><span class="sxs-lookup"><span data-stu-id="821fc-125">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="821fc-126">关系</span><span class="sxs-lookup"><span data-stu-id="821fc-126">Relationships</span></span>
| <span data-ttu-id="821fc-127">关系</span><span class="sxs-lookup"><span data-stu-id="821fc-127">Relationship</span></span> | <span data-ttu-id="821fc-128">类型</span><span class="sxs-lookup"><span data-stu-id="821fc-128">Type</span></span>   |<span data-ttu-id="821fc-129">说明</span><span class="sxs-lookup"><span data-stu-id="821fc-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="821fc-130">DeletedItems</span><span class="sxs-lookup"><span data-stu-id="821fc-130">deleteditems</span></span>|<span data-ttu-id="821fc-131">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="821fc-131">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="821fc-132">最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="821fc-132">Recently deleted items.</span></span> <span data-ttu-id="821fc-133">只读。</span><span class="sxs-lookup"><span data-stu-id="821fc-133">Read-only.</span></span> <span data-ttu-id="821fc-134">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="821fc-134">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="821fc-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="821fc-135">JSON representation</span></span>
<span data-ttu-id="821fc-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="821fc-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="821fc-137">示例</span><span class="sxs-lookup"><span data-stu-id="821fc-137">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/directory
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.directory"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->