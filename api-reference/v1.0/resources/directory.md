# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="50d07-101">目录资源类型（已删除的项目）</span><span class="sxs-lookup"><span data-stu-id="50d07-101">directory resource type (deleted items)</span></span>

<span data-ttu-id="50d07-102">表示目录中已删除的项目。</span><span class="sxs-lookup"><span data-stu-id="50d07-102">Represents a deleted item in the directory.</span></span> <span data-ttu-id="50d07-103">删除某个项目后，它会被添加到已删除项目“容器”中。</span><span class="sxs-lookup"><span data-stu-id="50d07-103">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="50d07-104">已删除的项目将保留最多 30 天的还原时间。</span><span class="sxs-lookup"><span data-stu-id="50d07-104">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="50d07-105">30 天后，这些项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="50d07-105">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="50d07-106">目前，已删除的项目功能仅支持用于 Office 365 [groups](group.md) 和 [users](users.md)。</span><span class="sxs-lookup"><span data-stu-id="50d07-106">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="50d07-107">方法</span><span class="sxs-lookup"><span data-stu-id="50d07-107">Methods</span></span>

| <span data-ttu-id="50d07-108">方法</span><span class="sxs-lookup"><span data-stu-id="50d07-108">Method</span></span>         | <span data-ttu-id="50d07-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="50d07-109">Return Type</span></span> | <span data-ttu-id="50d07-110">说明</span><span class="sxs-lookup"><span data-stu-id="50d07-110">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="50d07-111">Get deleted item</span><span class="sxs-lookup"><span data-stu-id="50d07-111">Get deleted item</span></span>](../api/directory_deleteditems_get.md) | [<span data-ttu-id="50d07-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="50d07-112">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="50d07-113">获取已删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="50d07-113">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="50d07-114">Restore deleted item</span><span class="sxs-lookup"><span data-stu-id="50d07-114">Restore deleted item</span></span>](../api/directory_deleteditems_restore.md) |[<span data-ttu-id="50d07-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="50d07-115">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="50d07-116">还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="50d07-116">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="50d07-117">List deleted items</span><span class="sxs-lookup"><span data-stu-id="50d07-117">List deleted items</span></span>](../api/directory_deleteditems_list.md) |<span data-ttu-id="50d07-118">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50d07-118">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="50d07-119">获取最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="50d07-119">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="50d07-120">Permanently delete an item</span><span class="sxs-lookup"><span data-stu-id="50d07-120">Permanently delete an item</span></span>](../api/directory_deleteditems_delete.md) | <span data-ttu-id="50d07-121">无</span><span class="sxs-lookup"><span data-stu-id="50d07-121">None</span></span> | <span data-ttu-id="50d07-122">永久删除项目。</span><span class="sxs-lookup"><span data-stu-id="50d07-122">Permanently deletes an item.</span></span> |

## <a name="properties"></a><span data-ttu-id="50d07-123">属性</span><span class="sxs-lookup"><span data-stu-id="50d07-123">Properties</span></span>
| <span data-ttu-id="50d07-124">属性</span><span class="sxs-lookup"><span data-stu-id="50d07-124">Property</span></span>   | <span data-ttu-id="50d07-125">类型</span><span class="sxs-lookup"><span data-stu-id="50d07-125">Type</span></span> |<span data-ttu-id="50d07-126">说明</span><span class="sxs-lookup"><span data-stu-id="50d07-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50d07-127">id</span><span class="sxs-lookup"><span data-stu-id="50d07-127">id</span></span>|<span data-ttu-id="50d07-128">String</span><span class="sxs-lookup"><span data-stu-id="50d07-128">String</span></span>| <span data-ttu-id="50d07-129">对象的唯一标识符；例如，12345678-9abc-def0-1234-56789abcde。</span><span class="sxs-lookup"><span data-stu-id="50d07-129">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span> <span data-ttu-id="50d07-130">键。</span><span class="sxs-lookup"><span data-stu-id="50d07-130">Key</span></span> <span data-ttu-id="50d07-131">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="50d07-131">Not nullable.</span></span> <span data-ttu-id="50d07-132">只读。</span><span class="sxs-lookup"><span data-stu-id="50d07-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50d07-133">关系</span><span class="sxs-lookup"><span data-stu-id="50d07-133">Relationships</span></span>
| <span data-ttu-id="50d07-134">关系</span><span class="sxs-lookup"><span data-stu-id="50d07-134">Relationship</span></span> | <span data-ttu-id="50d07-135">类型</span><span class="sxs-lookup"><span data-stu-id="50d07-135">Type</span></span>   |<span data-ttu-id="50d07-136">说明</span><span class="sxs-lookup"><span data-stu-id="50d07-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50d07-137">DeletedItems</span><span class="sxs-lookup"><span data-stu-id="50d07-137">deleteditems</span></span>|<span data-ttu-id="50d07-138">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50d07-138">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="50d07-139">最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="50d07-139">Recently deleted items.</span></span> <span data-ttu-id="50d07-140">只读。</span><span class="sxs-lookup"><span data-stu-id="50d07-140">Read-only.</span></span> <span data-ttu-id="50d07-141">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="50d07-141">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50d07-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50d07-142">JSON representation</span></span>
<span data-ttu-id="50d07-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50d07-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "id": "String (identifier)"
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