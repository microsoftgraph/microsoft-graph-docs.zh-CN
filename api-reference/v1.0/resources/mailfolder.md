# <a name="mailfolder-resource-type"></a><span data-ttu-id="e7784-101">mailFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7784-101">mailFolder resource type</span></span>

<span data-ttu-id="e7784-102">用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。</span><span class="sxs-lookup"><span data-stu-id="e7784-102">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="e7784-103">邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="e7784-103">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="e7784-104">Outlook 默认情况下会为用户创建某些文件夹。</span><span class="sxs-lookup"><span data-stu-id="e7784-104">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="e7784-105">为方便起见，可以在访问 **mailFolder** 集合中的这些文件夹时使用以下已知的文件夹名称：`ArchiveRoot`、`ConversationHistory`、`DeletedItems`、`Drafts`、`Inbox`、`JunkEmail`、`Outbox` 和 `SentItems` 来替代使用相应的文件夹 **ID** 值。</span><span class="sxs-lookup"><span data-stu-id="e7784-105">Instead of using the corresponding folder **id** value, for convenience, you can use the following well-known folder names when accessing these folders in a **mailFolder** collection: `ArchiveRoot`, `ConversationHistory`, `DeletedItems`, `Drafts`, `Inbox`, `JunkEmail`, `Outbox`, and `SentItems`.</span></span>

<span data-ttu-id="e7784-106">该资源支持通过提供 [delta](../api/mailfolder_delta.md) 函数使用[增量查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="e7784-106">This resource supports using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder_delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="e7784-107">方法</span><span class="sxs-lookup"><span data-stu-id="e7784-107">Methods</span></span>

| <span data-ttu-id="e7784-108">方法</span><span class="sxs-lookup"><span data-stu-id="e7784-108">Method</span></span>       | <span data-ttu-id="e7784-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e7784-109">Return Type</span></span>  |<span data-ttu-id="e7784-110">说明</span><span class="sxs-lookup"><span data-stu-id="e7784-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e7784-111">获取 mailFolder</span><span class="sxs-lookup"><span data-stu-id="e7784-111">Get mailFolder</span></span>](../api/mailfolder_get.md) | [<span data-ttu-id="e7784-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e7784-112">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="e7784-113">读取 mailFolder 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e7784-113">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="e7784-114">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="e7784-114">Create MailFolder</span></span>](../api/mailfolder_post_childfolders.md) |[<span data-ttu-id="e7784-115">MailFolder</span><span class="sxs-lookup"><span data-stu-id="e7784-115">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="e7784-116">通过发布到 childFolder 集合，在当前 mailFolder 下新建 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="e7784-116">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="e7784-117">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="e7784-117">List childFolders</span></span>](../api/mailfolder_list_childfolders.md) |<span data-ttu-id="e7784-118">[MailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7784-118">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="e7784-p103">获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="e7784-p103">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="e7784-121">创建邮件</span><span class="sxs-lookup"><span data-stu-id="e7784-121">Create Message</span></span>](../api/mailfolder_post_messages.md) |[<span data-ttu-id="e7784-122">邮件</span><span class="sxs-lookup"><span data-stu-id="e7784-122">Message</span></span>](message.md)| <span data-ttu-id="e7784-123">通过发布到邮件集合，在当前 mailFolder 中新建邮件。</span><span class="sxs-lookup"><span data-stu-id="e7784-123">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="e7784-124">列出邮件</span><span class="sxs-lookup"><span data-stu-id="e7784-124">List messages</span></span>](../api/mailfolder_list_messages.md) |<span data-ttu-id="e7784-125">[邮件](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7784-125">[Message](message.md) collection</span></span>| <span data-ttu-id="e7784-126">获取已登录用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。</span><span class="sxs-lookup"><span data-stu-id="e7784-126">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="e7784-127">更新</span><span class="sxs-lookup"><span data-stu-id="e7784-127">Update</span></span>](../api/mailfolder_update.md) | [<span data-ttu-id="e7784-128">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e7784-128">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="e7784-129">更新指定的 mailFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="e7784-129">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="e7784-130">删除</span><span class="sxs-lookup"><span data-stu-id="e7784-130">Delete</span></span>](../api/mailfolder_delete.md) | <span data-ttu-id="e7784-131">无</span><span class="sxs-lookup"><span data-stu-id="e7784-131">None</span></span> |<span data-ttu-id="e7784-132">删除指定的 mailFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="e7784-132">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="e7784-133">复制</span><span class="sxs-lookup"><span data-stu-id="e7784-133">copy</span></span>](../api/mailfolder_copy.md)|[<span data-ttu-id="e7784-134">MailFolder</span><span class="sxs-lookup"><span data-stu-id="e7784-134">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="e7784-135">将 mailfolder 及其内容复制到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="e7784-135">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="e7784-136">delta</span><span class="sxs-lookup"><span data-stu-id="e7784-136">delta</span></span>](../api/mailfolder_delta.md)|<span data-ttu-id="e7784-137">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7784-137">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="e7784-138">获取用户邮箱中已添加、删除或移除的邮件文件夹集。</span><span class="sxs-lookup"><span data-stu-id="e7784-138">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="e7784-139">移动</span><span class="sxs-lookup"><span data-stu-id="e7784-139">move</span></span>](../api/mailfolder_move.md)|[<span data-ttu-id="e7784-140">MailFolder</span><span class="sxs-lookup"><span data-stu-id="e7784-140">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="e7784-141">将 mailFolder 及其内容移动到其他 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="e7784-141">Move a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="e7784-142">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="e7784-142">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="e7784-143">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e7784-143">mailFolder</span></span>](mailFolder.md)  |<span data-ttu-id="e7784-144">在新建或现有的 mailFolder 中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e7784-144">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="e7784-145">获取具有单值扩展属性的 mailFolder</span><span class="sxs-lookup"><span data-stu-id="e7784-145">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="e7784-146">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e7784-146">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="e7784-147">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="e7784-147">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="e7784-148">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="e7784-148">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="e7784-149">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e7784-149">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="e7784-150">在新建或现有的 mailFolder 中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e7784-150">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="e7784-151">获取具有多值扩展属性的 mailFolder</span><span class="sxs-lookup"><span data-stu-id="e7784-151">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="e7784-152">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e7784-152">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="e7784-153">使用 `$expand` 获取包含一个多值扩展属性的 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="e7784-153">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="e7784-154">属性</span><span class="sxs-lookup"><span data-stu-id="e7784-154">Properties</span></span>
| <span data-ttu-id="e7784-155">属性</span><span class="sxs-lookup"><span data-stu-id="e7784-155">Property</span></span>     | <span data-ttu-id="e7784-156">类型</span><span class="sxs-lookup"><span data-stu-id="e7784-156">Type</span></span>   |<span data-ttu-id="e7784-157">说明</span><span class="sxs-lookup"><span data-stu-id="e7784-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7784-158">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="e7784-158">childFolderCount</span></span>|<span data-ttu-id="e7784-159">Int32</span><span class="sxs-lookup"><span data-stu-id="e7784-159">Int32</span></span>|<span data-ttu-id="e7784-160">当前 mailFolder 中的直接子 mailFolder 数量。</span><span class="sxs-lookup"><span data-stu-id="e7784-160">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="e7784-161">displayName</span><span class="sxs-lookup"><span data-stu-id="e7784-161">displayName</span></span>|<span data-ttu-id="e7784-162">String</span><span class="sxs-lookup"><span data-stu-id="e7784-162">String</span></span>|<span data-ttu-id="e7784-163">mailFolder 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e7784-163">The mailFolder's display name.</span></span>|
|<span data-ttu-id="e7784-164">id</span><span class="sxs-lookup"><span data-stu-id="e7784-164">id</span></span>|<span data-ttu-id="e7784-165">String</span><span class="sxs-lookup"><span data-stu-id="e7784-165">String</span></span>|<span data-ttu-id="e7784-p104">MailFolder 的唯一标识符。可以使用以下已知名称访问相应的文件夹：收件箱、草稿箱、已发送邮件、已删除邮件。</span><span class="sxs-lookup"><span data-stu-id="e7784-p104">The mailFolder's unique identifier. You can use the following well-known names to access the corresponding folder: Inbox, Drafts, SentItems, DeletedItems.</span></span>|
|<span data-ttu-id="e7784-168">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="e7784-168">parentFolderId</span></span>|<span data-ttu-id="e7784-169">String</span><span class="sxs-lookup"><span data-stu-id="e7784-169">String</span></span>|<span data-ttu-id="e7784-170">MailFolder 的父 mailFolder 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e7784-170">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="e7784-171">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="e7784-171">totalItemCount</span></span>|<span data-ttu-id="e7784-172">Int32</span><span class="sxs-lookup"><span data-stu-id="e7784-172">Int32</span></span>|<span data-ttu-id="e7784-173">邮箱中项的数量</span><span class="sxs-lookup"><span data-stu-id="e7784-173">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="e7784-174">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="e7784-174">unreadItemCount</span></span>|<span data-ttu-id="e7784-175">Int32</span><span class="sxs-lookup"><span data-stu-id="e7784-175">Int32</span></span>|<span data-ttu-id="e7784-176">mailFolder 中标记为未读的项的数量。</span><span class="sxs-lookup"><span data-stu-id="e7784-176">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="e7784-177">**有效的访问项计数**</span><span class="sxs-lookup"><span data-stu-id="e7784-177">**Access item counts efficiently**</span></span>

<span data-ttu-id="e7784-p105">使用文件夹的 TotalItemCount 和 UnreadItemCount 的属性可以方便地计算在文件夹中读取的项数。使你避免进行可产生重大延迟的查询，如下所示：</span><span class="sxs-lookup"><span data-stu-id="e7784-p105">The TotalItemCount and UnreadItemCount properties of a folder allow you to conveniently compute the number of read items in the folder. They let you avoid queries like the following that can incur significant latency:</span></span>
```
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```
<span data-ttu-id="e7784-p106">Outlook 中的 MailFolder 可包含多个类型的项，例如，收件箱可以包含不同于邮件项的会议请求项。无论项目类型如何，TotalItemCount 和 UnreadItemCount 包括 mailFolder 中的项。</span><span class="sxs-lookup"><span data-stu-id="e7784-p106">MailFolders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items. TotalItemCount and UnreadItemCount include items in a mailFolder irrespective of their item types.</span></span>


## <a name="relationships"></a><span data-ttu-id="e7784-182">关系</span><span class="sxs-lookup"><span data-stu-id="e7784-182">Relationships</span></span>
| <span data-ttu-id="e7784-183">关系</span><span class="sxs-lookup"><span data-stu-id="e7784-183">Relationship</span></span> | <span data-ttu-id="e7784-184">类型</span><span class="sxs-lookup"><span data-stu-id="e7784-184">Type</span></span>   |<span data-ttu-id="e7784-185">说明</span><span class="sxs-lookup"><span data-stu-id="e7784-185">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7784-186">childFolders</span><span class="sxs-lookup"><span data-stu-id="e7784-186">childFolders</span></span>|<span data-ttu-id="e7784-187">[MailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7784-187">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="e7784-188">mailFolder 中的子文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="e7784-188">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="e7784-189">邮件</span><span class="sxs-lookup"><span data-stu-id="e7784-189">messages</span></span>|<span data-ttu-id="e7784-190">[邮件](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7784-190">[Message](message.md) collection</span></span>|<span data-ttu-id="e7784-191">mailFolder 中的邮件集合。</span><span class="sxs-lookup"><span data-stu-id="e7784-191">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="e7784-192">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e7784-192">multiValueExtendedProperties</span></span>|<span data-ttu-id="e7784-193">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7784-193">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="e7784-p107">为 mailFolder 定义的多值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e7784-p107">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e7784-197">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e7784-197">singleValueExtendedProperties</span></span>|<span data-ttu-id="e7784-198">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="e7784-198">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="e7784-p108">为 mailFolder 定义的单值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e7784-p108">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7784-202">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7784-202">JSON representation</span></span>

<span data-ttu-id="e7784-203">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7784-203">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="e7784-204">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e7784-204">See also</span></span>

- [<span data-ttu-id="e7784-205">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="e7784-205">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="e7784-206">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="e7784-206">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
