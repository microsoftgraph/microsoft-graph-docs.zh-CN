# <a name="directoryobject-resource-type"></a><span data-ttu-id="70b50-101">directoryObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="70b50-101">directoryObject resource type</span></span>

<span data-ttu-id="70b50-p101">表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。</span><span class="sxs-lookup"><span data-stu-id="70b50-p101">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="70b50-104">方法</span><span class="sxs-lookup"><span data-stu-id="70b50-104">Methods</span></span>

| <span data-ttu-id="70b50-105">方法</span><span class="sxs-lookup"><span data-stu-id="70b50-105">Method</span></span>       | <span data-ttu-id="70b50-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="70b50-106">Return Type</span></span>  |<span data-ttu-id="70b50-107">说明</span><span class="sxs-lookup"><span data-stu-id="70b50-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70b50-108">获取 directoryObject</span><span class="sxs-lookup"><span data-stu-id="70b50-108">Get directoryObject</span></span>](../api/directoryobject_get.md) | [<span data-ttu-id="70b50-109">directoryObject</span><span class="sxs-lookup"><span data-stu-id="70b50-109">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="70b50-110">读取目录对象的属性。</span><span class="sxs-lookup"><span data-stu-id="70b50-110">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="70b50-111">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="70b50-111">Delete directoryObject</span></span>](../api/directoryobject_delete.md) | <span data-ttu-id="70b50-112">无</span><span class="sxs-lookup"><span data-stu-id="70b50-112">None</span></span> |<span data-ttu-id="70b50-113">删除目录对象。</span><span class="sxs-lookup"><span data-stu-id="70b50-113">Delete a directory object.</span></span> |
|[<span data-ttu-id="70b50-114">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="70b50-114">checkMemberGroups</span></span>](../api/directoryobject_checkmembergroups.md)|<span data-ttu-id="70b50-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="70b50-115">String collection</span></span>|<span data-ttu-id="70b50-p102">检查组列表中的成员身份。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="70b50-p102">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="70b50-118">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="70b50-118">getMemberGroups</span></span>](../api/directoryobject_getmembergroups.md)|<span data-ttu-id="70b50-119">字符串集合</span><span class="sxs-lookup"><span data-stu-id="70b50-119">String collection</span></span>|<span data-ttu-id="70b50-p103">返回 user、group 或 directory 对象所属的所有组。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="70b50-p103">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="70b50-122">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="70b50-122">getMemberObjects</span></span>](../api/directoryobject_getmemberobjects.md)|<span data-ttu-id="70b50-123">字符串集合</span><span class="sxs-lookup"><span data-stu-id="70b50-123">String collection</span></span>| <span data-ttu-id="70b50-p104">返回 user、group 或 directory 对象所属的所有组和目录角色。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="70b50-p104">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="70b50-126">getByIds</span><span class="sxs-lookup"><span data-stu-id="70b50-126">getByIds</span></span>](../api/directoryobject_getbyids.md) | <span data-ttu-id="70b50-127">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="70b50-127">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="70b50-128">基于提供的 ID 获取目录对象集。</span><span class="sxs-lookup"><span data-stu-id="70b50-128">Get a set of directory objects based on a set of supplied ids.</span></span> |

## <a name="properties"></a><span data-ttu-id="70b50-129">属性</span><span class="sxs-lookup"><span data-stu-id="70b50-129">Properties</span></span>

| <span data-ttu-id="70b50-130">属性</span><span class="sxs-lookup"><span data-stu-id="70b50-130">Property</span></span>   | <span data-ttu-id="70b50-131">类型</span><span class="sxs-lookup"><span data-stu-id="70b50-131">Type</span></span> |<span data-ttu-id="70b50-132">说明</span><span class="sxs-lookup"><span data-stu-id="70b50-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70b50-133">ID</span><span class="sxs-lookup"><span data-stu-id="70b50-133">id</span></span>|<span data-ttu-id="70b50-134">字符串</span><span class="sxs-lookup"><span data-stu-id="70b50-134">String</span></span>|<span data-ttu-id="70b50-p105">用作此对象的唯一标识符的 Guid；例如，12345678-9abc-def0-1234-56789abcde。键。不可为 null。只读。</span><span class="sxs-lookup"><span data-stu-id="70b50-p105">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70b50-139">关系</span><span class="sxs-lookup"><span data-stu-id="70b50-139">Relationships</span></span>

<span data-ttu-id="70b50-140">无</span><span class="sxs-lookup"><span data-stu-id="70b50-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="70b50-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70b50-141">JSON representation</span></span>

<span data-ttu-id="70b50-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70b50-142">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directoryObject",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
