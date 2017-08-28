# <a name="contactfolder-resource-type"></a><span data-ttu-id="cce60-101">contactFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="cce60-101">contactFolder resource type</span></span>

<span data-ttu-id="cce60-102">包含联系人的文件夹。</span><span class="sxs-lookup"><span data-stu-id="cce60-102">A folder that contains contacts.</span></span>

<span data-ttu-id="cce60-103">该资源支持通过提供 [delta](../api/contactfolder_delta.md) 函数使用[增量查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="cce60-103">This resource supports using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="cce60-104">方法</span><span class="sxs-lookup"><span data-stu-id="cce60-104">Methods</span></span>

| <span data-ttu-id="cce60-105">方法</span><span class="sxs-lookup"><span data-stu-id="cce60-105">Method</span></span>       | <span data-ttu-id="cce60-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="cce60-106">Return Type</span></span>  |<span data-ttu-id="cce60-107">说明</span><span class="sxs-lookup"><span data-stu-id="cce60-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cce60-108">获取 contactFolder</span><span class="sxs-lookup"><span data-stu-id="cce60-108">Get contactFolder</span></span>](../api/contactfolder_get.md) | [<span data-ttu-id="cce60-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="cce60-109">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="cce60-110">通过使用联系人文件夹 ID 获取联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="cce60-110">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="cce60-111">更新</span><span class="sxs-lookup"><span data-stu-id="cce60-111">Update</span></span>](../api/contactfolder_update.md) | [<span data-ttu-id="cce60-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="cce60-112">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="cce60-113">更新 contactFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="cce60-113">Update contactFolder object.</span></span> |
|[<span data-ttu-id="cce60-114">删除</span><span class="sxs-lookup"><span data-stu-id="cce60-114">Delete</span></span>](../api/contactfolder_delete.md) | <span data-ttu-id="cce60-115">无</span><span class="sxs-lookup"><span data-stu-id="cce60-115">None</span></span> |<span data-ttu-id="cce60-116">删除 contactFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="cce60-116">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="cce60-117">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="cce60-117">List childFolders</span></span>](../api/contactfolder_list_childfolders.md) |<span data-ttu-id="cce60-118">[ContactFolder](contactfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cce60-118">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="cce60-119">获取指定联系人文件夹下的子文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="cce60-119">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="cce60-120">创建子 ContactFolder</span><span class="sxs-lookup"><span data-stu-id="cce60-120">Create child contactFolder</span></span>](../api/contactfolder_post_childfolders.md) |[<span data-ttu-id="cce60-121">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="cce60-121">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="cce60-122">创建新的 contactFolder 作为指定文件夹的子文件夹。</span><span class="sxs-lookup"><span data-stu-id="cce60-122">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="cce60-123">delta</span><span class="sxs-lookup"><span data-stu-id="cce60-123">delta</span></span>](../api/contact_delta.md)|<span data-ttu-id="cce60-124">[联系人](contact.md)集合</span><span class="sxs-lookup"><span data-stu-id="cce60-124">[contact](contact.md) collection</span></span>| <span data-ttu-id="cce60-125">获取用户邮箱中已添加、删除或移除的联系人文件夹集。</span><span class="sxs-lookup"><span data-stu-id="cce60-125">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="cce60-126">列出文件夹中的联系人</span><span class="sxs-lookup"><span data-stu-id="cce60-126">List contacts in folder</span></span>](../api/contactfolder_list_contacts.md) |<span data-ttu-id="cce60-127">[联系人](contact.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cce60-127">[Contact](contact.md) collection</span></span>| <span data-ttu-id="cce60-128">从已登录用户的默认联系人文件夹 (`.../me/contacts`) 或指定的联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="cce60-128">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="cce60-129">在文件夹中创建联系人</span><span class="sxs-lookup"><span data-stu-id="cce60-129">Create contact in folder</span></span>](../api/contactfolder_post_contacts.md) |[<span data-ttu-id="cce60-130">联系人</span><span class="sxs-lookup"><span data-stu-id="cce60-130">Contact</span></span>](contact.md)| <span data-ttu-id="cce60-131">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 端点中。</span><span class="sxs-lookup"><span data-stu-id="cce60-131">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="cce60-132">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="cce60-132">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="cce60-133">contactFolder</span><span class="sxs-lookup"><span data-stu-id="cce60-133">contactFolder</span></span>](contactFolder.md)  |<span data-ttu-id="cce60-134">在新建或现有的 contactFolder 中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="cce60-134">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="cce60-135">获取包含单值扩展属性的 contactFolder</span><span class="sxs-lookup"><span data-stu-id="cce60-135">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="cce60-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="cce60-136">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="cce60-137">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="cce60-137">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="cce60-138">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="cce60-138">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="cce60-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="cce60-139">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="cce60-140">在新建或现有的 contactFolder 创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="cce60-140">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="cce60-141">获取包含多值扩展属性的 contactFolder</span><span class="sxs-lookup"><span data-stu-id="cce60-141">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="cce60-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="cce60-142">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="cce60-143">使用 `$expand` 获取包含一个多值扩展属性的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="cce60-143">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="cce60-144">属性</span><span class="sxs-lookup"><span data-stu-id="cce60-144">Properties</span></span>
| <span data-ttu-id="cce60-145">属性</span><span class="sxs-lookup"><span data-stu-id="cce60-145">Property</span></span>     | <span data-ttu-id="cce60-146">类型</span><span class="sxs-lookup"><span data-stu-id="cce60-146">Type</span></span>   |<span data-ttu-id="cce60-147">说明</span><span class="sxs-lookup"><span data-stu-id="cce60-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cce60-148">displayName</span><span class="sxs-lookup"><span data-stu-id="cce60-148">displayName</span></span>|<span data-ttu-id="cce60-149">String</span><span class="sxs-lookup"><span data-stu-id="cce60-149">String</span></span>|<span data-ttu-id="cce60-150">文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="cce60-150">The folder's display name.</span></span>|
|<span data-ttu-id="cce60-151">id</span><span class="sxs-lookup"><span data-stu-id="cce60-151">id</span></span>|<span data-ttu-id="cce60-152">String</span><span class="sxs-lookup"><span data-stu-id="cce60-152">String</span></span>|<span data-ttu-id="cce60-p101">联系人文件夹的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="cce60-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="cce60-155">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="cce60-155">parentFolderId</span></span>|<span data-ttu-id="cce60-156">String</span><span class="sxs-lookup"><span data-stu-id="cce60-156">String</span></span>|<span data-ttu-id="cce60-157">文件夹的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="cce60-157">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cce60-158">关系</span><span class="sxs-lookup"><span data-stu-id="cce60-158">Relationships</span></span>
| <span data-ttu-id="cce60-159">关系</span><span class="sxs-lookup"><span data-stu-id="cce60-159">Relationship</span></span> | <span data-ttu-id="cce60-160">类型</span><span class="sxs-lookup"><span data-stu-id="cce60-160">Type</span></span>   |<span data-ttu-id="cce60-161">说明</span><span class="sxs-lookup"><span data-stu-id="cce60-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cce60-162">childFolders</span><span class="sxs-lookup"><span data-stu-id="cce60-162">childFolders</span></span>|<span data-ttu-id="cce60-163">[ContactFolder](contactfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cce60-163">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="cce60-p102">文件夹中的子文件夹集合。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="cce60-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="cce60-168">contacts</span><span class="sxs-lookup"><span data-stu-id="cce60-168">contacts</span></span>|<span data-ttu-id="cce60-169">[联系人](contact.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cce60-169">[Contact](contact.md) collection</span></span>|<span data-ttu-id="cce60-p103">文件夹中的联系人。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="cce60-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="cce60-174">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="cce60-174">multiValueExtendedProperties</span></span>|<span data-ttu-id="cce60-175">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cce60-175">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="cce60-p104">为 contactFolder 定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="cce60-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="cce60-179">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="cce60-179">singleValueExtendedProperties</span></span>|<span data-ttu-id="cce60-180">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cce60-180">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="cce60-p105">为 contactFolder 定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="cce60-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cce60-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cce60-184">JSON representation</span></span>

<span data-ttu-id="cce60-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cce60-185">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="cce60-186">另请参阅</span><span class="sxs-lookup"><span data-stu-id="cce60-186">See also</span></span>

- [<span data-ttu-id="cce60-187">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="cce60-187">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="cce60-188">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="cce60-188">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
