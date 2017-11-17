# <a name="mailfolder-resource-type"></a><span data-ttu-id="67122-101">mailFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="67122-101">mailFolder resource type</span></span>

<span data-ttu-id="67122-p101">用户邮箱中的 mailFolder，例如收件箱、草稿箱和已发送邮件。MailFolders 可包含邮件和子 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="67122-p101">A mailFolder in a user's mailbox, such as Inbox, Drafts, and Sent Items. MailFolders can contain messages and child mailFolders.</span></span>

<span data-ttu-id="67122-104">该资源支持通过提供 [delta](../api/mailfolder_delta.md) 函数使用[增量查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="67122-104">This resource supports using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder_delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="67122-105">方法</span><span class="sxs-lookup"><span data-stu-id="67122-105">Methods</span></span>

| <span data-ttu-id="67122-106">方法</span><span class="sxs-lookup"><span data-stu-id="67122-106">Method</span></span>       | <span data-ttu-id="67122-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="67122-107">Return Type</span></span>  |<span data-ttu-id="67122-108">说明</span><span class="sxs-lookup"><span data-stu-id="67122-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="67122-109">获取 mailFolder</span><span class="sxs-lookup"><span data-stu-id="67122-109">Get mailFolder</span></span>](../api/mailfolder_get.md) | [<span data-ttu-id="67122-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="67122-110">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="67122-111">读取 mailFolder 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="67122-111">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="67122-112">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="67122-112">Create MailFolder</span></span>](../api/mailfolder_post_childfolders.md) |[<span data-ttu-id="67122-113">MailFolder</span><span class="sxs-lookup"><span data-stu-id="67122-113">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="67122-114">通过发布到 childFolder 集合，在当前 mailFolder 下新建 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="67122-114">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="67122-115">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="67122-115">List childFolders</span></span>](../api/mailfolder_list_childfolders.md) |<span data-ttu-id="67122-116">[MailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67122-116">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="67122-p102">获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="67122-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="67122-119">创建邮件</span><span class="sxs-lookup"><span data-stu-id="67122-119">Create Message</span></span>](../api/mailfolder_post_messages.md) |[<span data-ttu-id="67122-120">邮件</span><span class="sxs-lookup"><span data-stu-id="67122-120">Message</span></span>](message.md)| <span data-ttu-id="67122-121">通过发布到邮件集合，在当前 mailFolder 中新建邮件。</span><span class="sxs-lookup"><span data-stu-id="67122-121">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="67122-122">列出邮件</span><span class="sxs-lookup"><span data-stu-id="67122-122">List messages</span></span>](../api/mailfolder_list_messages.md) |<span data-ttu-id="67122-123">[邮件](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67122-123">[Message](message.md) collection</span></span>| <span data-ttu-id="67122-124">获取已登录用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。</span><span class="sxs-lookup"><span data-stu-id="67122-124">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="67122-125">更新</span><span class="sxs-lookup"><span data-stu-id="67122-125">Update</span></span>](../api/mailfolder_update.md) | [<span data-ttu-id="67122-126">mailFolder</span><span class="sxs-lookup"><span data-stu-id="67122-126">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="67122-127">更新指定的 mailFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="67122-127">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="67122-128">删除</span><span class="sxs-lookup"><span data-stu-id="67122-128">Delete</span></span>](../api/mailfolder_delete.md) | <span data-ttu-id="67122-129">无</span><span class="sxs-lookup"><span data-stu-id="67122-129">None</span></span> |<span data-ttu-id="67122-130">删除指定的 mailFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="67122-130">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="67122-131">复制</span><span class="sxs-lookup"><span data-stu-id="67122-131">copy</span></span>](../api/mailfolder_copy.md)|[<span data-ttu-id="67122-132">MailFolder</span><span class="sxs-lookup"><span data-stu-id="67122-132">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="67122-133">将 mailfolder 及其内容复制到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="67122-133">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="67122-134">delta</span><span class="sxs-lookup"><span data-stu-id="67122-134">delta</span></span>](../api/mailfolder_delta.md)|<span data-ttu-id="67122-135">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67122-135">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="67122-136">获取用户邮箱中已添加、删除或移除的邮件文件夹集。</span><span class="sxs-lookup"><span data-stu-id="67122-136">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="67122-137">移动</span><span class="sxs-lookup"><span data-stu-id="67122-137">move</span></span>](../api/mailfolder_move.md)|[<span data-ttu-id="67122-138">MailFolder</span><span class="sxs-lookup"><span data-stu-id="67122-138">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="67122-139">将 mailFolder 及其内容移动到其他 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="67122-139">Move a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="67122-140">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="67122-140">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="67122-141">mailFolder</span><span class="sxs-lookup"><span data-stu-id="67122-141">mailFolder</span></span>](mailFolder.md)  |<span data-ttu-id="67122-142">在新建或现有的 mailFolder 中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="67122-142">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="67122-143">获取具有单值扩展属性的 mailFolder</span><span class="sxs-lookup"><span data-stu-id="67122-143">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="67122-144">mailFolder</span><span class="sxs-lookup"><span data-stu-id="67122-144">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="67122-145">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="67122-145">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="67122-146">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="67122-146">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="67122-147">mailFolder</span><span class="sxs-lookup"><span data-stu-id="67122-147">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="67122-148">在新建或现有的 mailFolder 中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="67122-148">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="67122-149">获取具有多值扩展属性的 mailFolder</span><span class="sxs-lookup"><span data-stu-id="67122-149">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="67122-150">mailFolder</span><span class="sxs-lookup"><span data-stu-id="67122-150">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="67122-151">使用 `$expand` 获取包含一个多值扩展属性的 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="67122-151">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="67122-152">属性</span><span class="sxs-lookup"><span data-stu-id="67122-152">Properties</span></span>
| <span data-ttu-id="67122-153">属性</span><span class="sxs-lookup"><span data-stu-id="67122-153">Property</span></span>     | <span data-ttu-id="67122-154">类型</span><span class="sxs-lookup"><span data-stu-id="67122-154">Type</span></span>   |<span data-ttu-id="67122-155">说明</span><span class="sxs-lookup"><span data-stu-id="67122-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67122-156">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="67122-156">childFolderCount</span></span>|<span data-ttu-id="67122-157">Int32</span><span class="sxs-lookup"><span data-stu-id="67122-157">Int32</span></span>|<span data-ttu-id="67122-158">当前 mailFolder 中的直接子 mailFolder 数量。</span><span class="sxs-lookup"><span data-stu-id="67122-158">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="67122-159">displayName</span><span class="sxs-lookup"><span data-stu-id="67122-159">displayName</span></span>|<span data-ttu-id="67122-160">String</span><span class="sxs-lookup"><span data-stu-id="67122-160">String</span></span>|<span data-ttu-id="67122-161">mailFolder 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="67122-161">The mailFolder's display name.</span></span>|
|<span data-ttu-id="67122-162">id</span><span class="sxs-lookup"><span data-stu-id="67122-162">id</span></span>|<span data-ttu-id="67122-163">String</span><span class="sxs-lookup"><span data-stu-id="67122-163">String</span></span>|<span data-ttu-id="67122-p103">MailFolder 的唯一标识符。可以使用以下已知名称访问相应的文件夹：收件箱、草稿箱、已发送邮件、已删除邮件。</span><span class="sxs-lookup"><span data-stu-id="67122-p103">The mailFolder's unique identifier. You can use the following well-known names to access the corresponding folder: Inbox, Drafts, SentItems, DeletedItems.</span></span>|
|<span data-ttu-id="67122-166">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="67122-166">parentFolderId</span></span>|<span data-ttu-id="67122-167">String</span><span class="sxs-lookup"><span data-stu-id="67122-167">String</span></span>|<span data-ttu-id="67122-168">MailFolder 的父 mailFolder 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="67122-168">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="67122-169">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="67122-169">totalItemCount</span></span>|<span data-ttu-id="67122-170">Int32</span><span class="sxs-lookup"><span data-stu-id="67122-170">Int32</span></span>|<span data-ttu-id="67122-171">邮箱中项的数量</span><span class="sxs-lookup"><span data-stu-id="67122-171">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="67122-172">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="67122-172">unreadItemCount</span></span>|<span data-ttu-id="67122-173">Int32</span><span class="sxs-lookup"><span data-stu-id="67122-173">Int32</span></span>|<span data-ttu-id="67122-174">mailFolder 中标记为未读的项的数量。</span><span class="sxs-lookup"><span data-stu-id="67122-174">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="67122-175">**有效的访问项计数**</span><span class="sxs-lookup"><span data-stu-id="67122-175">**Access item counts efficiently**</span></span>

<span data-ttu-id="67122-p104">使用文件夹的 TotalItemCount 和 UnreadItemCount 的属性可以方便地计算在文件夹中读取的项数。使你避免进行可产生重大延迟的查询，如下所示：</span><span class="sxs-lookup"><span data-stu-id="67122-p104">The TotalItemCount and UnreadItemCount properties of a folder allow you to conveniently compute the number of read items in the folder. They let you avoid queries like the following that can incur significant latency:</span></span>
```
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```
<span data-ttu-id="67122-p105">Outlook 中的 MailFolder 可包含多个类型的项，例如，收件箱可以包含不同于邮件项的会议请求项。无论项目类型如何，TotalItemCount 和 UnreadItemCount 包括 mailFolder 中的项。</span><span class="sxs-lookup"><span data-stu-id="67122-p105">MailFolders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items. TotalItemCount and UnreadItemCount include items in a mailFolder irrespective of their item types.</span></span>


## <a name="relationships"></a><span data-ttu-id="67122-180">关系</span><span class="sxs-lookup"><span data-stu-id="67122-180">Relationships</span></span>
| <span data-ttu-id="67122-181">关系</span><span class="sxs-lookup"><span data-stu-id="67122-181">Relationship</span></span> | <span data-ttu-id="67122-182">类型</span><span class="sxs-lookup"><span data-stu-id="67122-182">Type</span></span>   |<span data-ttu-id="67122-183">说明</span><span class="sxs-lookup"><span data-stu-id="67122-183">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67122-184">childFolders</span><span class="sxs-lookup"><span data-stu-id="67122-184">childFolders</span></span>|<span data-ttu-id="67122-185">[MailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67122-185">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="67122-186">mailFolder 中的子文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="67122-186">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="67122-187">邮件</span><span class="sxs-lookup"><span data-stu-id="67122-187">messages</span></span>|<span data-ttu-id="67122-188">[邮件](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67122-188">[Message](message.md) collection</span></span>|<span data-ttu-id="67122-189">mailFolder 中的邮件集合。</span><span class="sxs-lookup"><span data-stu-id="67122-189">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="67122-190">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="67122-190">multiValueExtendedProperties</span></span>|<span data-ttu-id="67122-191">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67122-191">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="67122-p106">为 mailFolder 定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="67122-p106">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="67122-195">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="67122-195">singleValueExtendedProperties</span></span>|<span data-ttu-id="67122-196">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67122-196">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="67122-p107">为 mailFolder 定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="67122-p107">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67122-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67122-200">JSON representation</span></span>

<span data-ttu-id="67122-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67122-201">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder"
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,

  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}

```

## <a name="see-also"></a><span data-ttu-id="67122-202">另请参阅</span><span class="sxs-lookup"><span data-stu-id="67122-202">See also</span></span>

- [<span data-ttu-id="67122-203">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="67122-203">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="67122-204">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="67122-204">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
