# <a name="mailfolder-resource-type"></a><span data-ttu-id="88f34-101">mailFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="88f34-101">mailFolder resource type</span></span>

<span data-ttu-id="88f34-102">用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。</span><span class="sxs-lookup"><span data-stu-id="88f34-102">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="88f34-103">邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-103">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="88f34-104">该资源支持通过提供 [delta](../api/mailfolder_delta.md) 函数使用[增量查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="88f34-104">This resource supports using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder_delta.md) function.</span></span>

<span data-ttu-id="88f34-105">**已知文件夹名**</span><span class="sxs-lookup"><span data-stu-id="88f34-105">**Well-known folder names**</span></span>

<span data-ttu-id="88f34-106">Outlook 默认情况下会为用户创建某些文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-106">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="88f34-107">访问这些文件夹时，为方便起见，你可以使用下表中的已知文件夹名而不必使用的相应文件夹 **ID** 值。</span><span class="sxs-lookup"><span data-stu-id="88f34-107">Instead of using the corresponding folder id value, for convenience, you can use the following well-known folder names when accessing these folders in a mailFolder collection: , , , , , , , and .</span></span> <span data-ttu-id="88f34-108">例如，你可以通过以下查询使用其已知名称来获取草稿箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-108">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="88f34-109">已知名称不分用户邮箱的区域设置一律奏效，所以上述查询将不顾文件夹的命名方式而始终返回用户的草稿箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-109">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="88f34-110">已知文件夹名</span><span class="sxs-lookup"><span data-stu-id="88f34-110">Well-known folder name</span></span> | <span data-ttu-id="88f34-111">说明</span><span class="sxs-lookup"><span data-stu-id="88f34-111">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="88f34-112">存档</span><span class="sxs-lookup"><span data-stu-id="88f34-112">Archive</span></span> | <span data-ttu-id="88f34-113">在支持的 Outlook 客户端使用“One_Click 存档”功能时，就可发送存档文件夹邮件。</span><span class="sxs-lookup"><span data-stu-id="88f34-113">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="88f34-114">**注意：** 这个与 Exchange online 的“存档邮箱”功能不一样。</span><span class="sxs-lookup"><span data-stu-id="88f34-114">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="88f34-115">混乱邮件</span><span class="sxs-lookup"><span data-stu-id="88f34-115">Clutter</span></span> | <span data-ttu-id="88f34-116">在使用“混乱邮件”功能时，就可移动混乱文件夹低优先级邮件了。</span><span class="sxs-lookup"><span data-stu-id="88f34-116">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="88f34-117">冲突</span><span class="sxs-lookup"><span data-stu-id="88f34-117">Conflicts</span></span> | <span data-ttu-id="88f34-118">邮箱中包含冲突项目的文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-118">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="88f34-119">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="88f34-119">conversationhistory</span></span> | <span data-ttu-id="88f34-120">Skype 保存 IM 对话（如果 Skype 配置这样做）的文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-120">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="88f34-121">deleteditems</span><span class="sxs-lookup"><span data-stu-id="88f34-121">deleteditems</span></span> | <span data-ttu-id="88f34-122">删除文件夹项目时，就可移动文件夹项目了。</span><span class="sxs-lookup"><span data-stu-id="88f34-122">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="88f34-123">草稿</span><span class="sxs-lookup"><span data-stu-id="88f34-123">drafts</span></span> | <span data-ttu-id="88f34-124">包含未发送邮件的文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-124">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="88f34-125">收件箱</span><span class="sxs-lookup"><span data-stu-id="88f34-125">Inbox</span></span> | <span data-ttu-id="88f34-126">收件箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-126">The Inbox folder.</span></span> |
| <span data-ttu-id="88f34-127">junkemail</span><span class="sxs-lookup"><span data-stu-id="88f34-127">junkemail</span></span> | <span data-ttu-id="88f34-128">垃圾邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-128">The Junk E-Mail folder.</span></span> |
| <span data-ttu-id="88f34-129">localfailures</span><span class="sxs-lookup"><span data-stu-id="88f34-129">localfailures</span></span> | <span data-ttu-id="88f34-130">包含存在于本地客户端上，但无法上传到服务器的项目的文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-130">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="88f34-131">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="88f34-131">msgfolderroot</span></span> | <span data-ttu-id="88f34-132">“Information Store 顶端”文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-132">The "Top of Information Store" folder.</span></span> <span data-ttu-id="88f34-133">这个文件夹是普通邮件客户端中显示的如收件箱之类文件夹的父文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-133">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="88f34-134">发件箱</span><span class="sxs-lookup"><span data-stu-id="88f34-134">Outbox</span></span> | <span data-ttu-id="88f34-135">发件箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-135">The Outbox folder.</span></span> |
| <span data-ttu-id="88f34-136">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="88f34-136">recoverableitemsdeletions</span></span> | <span data-ttu-id="88f34-137">包含软删除项目的文件夹：从“已删除邮件”文件夹中删除的，或在 Outlook 中通过按 shift+delete 删除的。</span><span class="sxs-lookup"><span data-stu-id="88f34-137">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="88f34-138">这个文件夹在任何 Outlook 电子邮件客户端中都不可见，但是最终用户可以通过 Outlook 中或 Outlook 网页版上的**从服务器恢复已删除邮件**功能与其进行交互。</span><span class="sxs-lookup"><span data-stu-id="88f34-138">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="88f34-139">已计划</span><span class="sxs-lookup"><span data-stu-id="88f34-139">scheduled</span></span> | <span data-ttu-id="88f34-140">包含使用 Outlook for iOS 中的日程安排功能计划重新显示在收件箱中的邮件的文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-140">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="88f34-141">searchfolders</span><span class="sxs-lookup"><span data-stu-id="88f34-141">searchfolders</span></span> | <span data-ttu-id="88f34-142">在用户的邮箱中定义的所有搜索文件夹的父文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-142">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="88f34-143">sentitems</span><span class="sxs-lookup"><span data-stu-id="88f34-143">sentitems</span></span> | <span data-ttu-id="88f34-144">已发送邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-144">sent items folder</span></span> |
| <span data-ttu-id="88f34-145">serverfailures</span><span class="sxs-lookup"><span data-stu-id="88f34-145">serverfailures</span></span> | <span data-ttu-id="88f34-146">包含存在于服务器上，但无法同步到本地客户端的项目的文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-146">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="88f34-147">syncissues</span><span class="sxs-lookup"><span data-stu-id="88f34-147">syncissues</span></span> | <span data-ttu-id="88f34-148">包含由 Outlook 创建的同步日志的文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-148">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="88f34-149">方法</span><span class="sxs-lookup"><span data-stu-id="88f34-149">Methods</span></span>

| <span data-ttu-id="88f34-150">方法</span><span class="sxs-lookup"><span data-stu-id="88f34-150">Method</span></span> | <span data-ttu-id="88f34-151">返回类型</span><span class="sxs-lookup"><span data-stu-id="88f34-151">Return Type</span></span> | <span data-ttu-id="88f34-152">说明</span><span class="sxs-lookup"><span data-stu-id="88f34-152">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="88f34-153">获取 mailFolder</span><span class="sxs-lookup"><span data-stu-id="88f34-153">Get mailFolder</span></span>](../api/mailfolder_get.md) | [<span data-ttu-id="88f34-154">mailFolder</span><span class="sxs-lookup"><span data-stu-id="88f34-154">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="88f34-155">读取 mailFolder 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88f34-155">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="88f34-156">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="88f34-156">Create MailFolder</span></span>](../api/mailfolder_post_childfolders.md) |[<span data-ttu-id="88f34-157">MailFolder</span><span class="sxs-lookup"><span data-stu-id="88f34-157">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="88f34-158">通过发布到 childFolder 集合，在当前 mailFolder 下新建 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="88f34-158">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="88f34-159">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="88f34-159">List childFolders</span></span>](../api/mailfolder_list_childfolders.md) |<span data-ttu-id="88f34-160">[MailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88f34-160">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="88f34-p106">获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="88f34-p106">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="88f34-163">创建邮件</span><span class="sxs-lookup"><span data-stu-id="88f34-163">Create Message</span></span>](../api/mailfolder_post_messages.md) |[<span data-ttu-id="88f34-164">邮件</span><span class="sxs-lookup"><span data-stu-id="88f34-164">Message</span></span>](message.md)| <span data-ttu-id="88f34-165">通过发布到邮件集合，在当前 mailFolder 中新建邮件。</span><span class="sxs-lookup"><span data-stu-id="88f34-165">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="88f34-166">列出邮件</span><span class="sxs-lookup"><span data-stu-id="88f34-166">List messages</span></span>](../api/mailfolder_list_messages.md) |<span data-ttu-id="88f34-167">[邮件](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88f34-167">[Message](message.md) collection</span></span>| <span data-ttu-id="88f34-168">获取已登录用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。</span><span class="sxs-lookup"><span data-stu-id="88f34-168">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="88f34-169">更新</span><span class="sxs-lookup"><span data-stu-id="88f34-169">Update</span></span>](../api/mailfolder_update.md) | [<span data-ttu-id="88f34-170">mailFolder</span><span class="sxs-lookup"><span data-stu-id="88f34-170">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="88f34-171">更新指定的 mailFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="88f34-171">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="88f34-172">删除</span><span class="sxs-lookup"><span data-stu-id="88f34-172">Delete</span></span>](../api/mailfolder_delete.md) | <span data-ttu-id="88f34-173">无</span><span class="sxs-lookup"><span data-stu-id="88f34-173">None</span></span> |<span data-ttu-id="88f34-174">删除指定的 mailFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="88f34-174">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="88f34-175">复制</span><span class="sxs-lookup"><span data-stu-id="88f34-175">copy</span></span>](../api/mailfolder_copy.md)|[<span data-ttu-id="88f34-176">MailFolder</span><span class="sxs-lookup"><span data-stu-id="88f34-176">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="88f34-177">将 mailfolder 及其内容复制到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="88f34-177">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="88f34-178">delta</span><span class="sxs-lookup"><span data-stu-id="88f34-178">delta</span></span>](../api/mailfolder_delta.md)|<span data-ttu-id="88f34-179">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88f34-179">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="88f34-180">获取用户邮箱中已添加、删除或移除的邮件文件夹集。</span><span class="sxs-lookup"><span data-stu-id="88f34-180">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="88f34-181">移动</span><span class="sxs-lookup"><span data-stu-id="88f34-181">move</span></span>](../api/mailfolder_move.md)|[<span data-ttu-id="88f34-182">MailFolder</span><span class="sxs-lookup"><span data-stu-id="88f34-182">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="88f34-183">将 mailFolder 及其内容移动到其他 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="88f34-183">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="88f34-184">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="88f34-184">**Extended properties**</span></span>| | |
|[<span data-ttu-id="88f34-185">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="88f34-185">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="88f34-186">mailFolder</span><span class="sxs-lookup"><span data-stu-id="88f34-186">mailFolder</span></span>](mailFolder.md)  |<span data-ttu-id="88f34-187">在新建或现有的 mailFolder 中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="88f34-187">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="88f34-188">获取具有单值扩展属性的 mailFolder</span><span class="sxs-lookup"><span data-stu-id="88f34-188">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="88f34-189">mailFolder</span><span class="sxs-lookup"><span data-stu-id="88f34-189">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="88f34-190">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="88f34-190">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="88f34-191">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="88f34-191">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="88f34-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="88f34-192">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="88f34-193">在新建或现有的 mailFolder 中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="88f34-193">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="88f34-194">获取具有多值扩展属性的 mailFolder</span><span class="sxs-lookup"><span data-stu-id="88f34-194">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="88f34-195">mailFolder</span><span class="sxs-lookup"><span data-stu-id="88f34-195">mailFolder</span></span>](mailFolder.md) | <span data-ttu-id="88f34-196">使用 `$expand` 获取包含一个多值扩展属性的 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="88f34-196">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="88f34-197">属性</span><span class="sxs-lookup"><span data-stu-id="88f34-197">Properties</span></span>

| <span data-ttu-id="88f34-198">属性</span><span class="sxs-lookup"><span data-stu-id="88f34-198">Property</span></span> | <span data-ttu-id="88f34-199">类型</span><span class="sxs-lookup"><span data-stu-id="88f34-199">Type</span></span> | <span data-ttu-id="88f34-200">说明</span><span class="sxs-lookup"><span data-stu-id="88f34-200">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="88f34-201">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="88f34-201">childFolderCount</span></span>|<span data-ttu-id="88f34-202">Int32</span><span class="sxs-lookup"><span data-stu-id="88f34-202">Int32</span></span>|<span data-ttu-id="88f34-203">当前 mailFolder 中的直接子 mailFolder 数量。</span><span class="sxs-lookup"><span data-stu-id="88f34-203">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="88f34-204">displayName</span><span class="sxs-lookup"><span data-stu-id="88f34-204">displayName</span></span>|<span data-ttu-id="88f34-205">字符串</span><span class="sxs-lookup"><span data-stu-id="88f34-205">String</span></span>|<span data-ttu-id="88f34-206">mailFolder 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="88f34-206">The mailFolder's display name.</span></span>|
|<span data-ttu-id="88f34-207">ID</span><span class="sxs-lookup"><span data-stu-id="88f34-207">id</span></span>|<span data-ttu-id="88f34-208">字符串</span><span class="sxs-lookup"><span data-stu-id="88f34-208">String</span></span>|<span data-ttu-id="88f34-209">mailFolder 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="88f34-209">The folder's unique identifier.</span></span>|
|<span data-ttu-id="88f34-210">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="88f34-210">parentFolderId</span></span>|<span data-ttu-id="88f34-211">字符串</span><span class="sxs-lookup"><span data-stu-id="88f34-211">String</span></span>|<span data-ttu-id="88f34-212">MailFolder 的父 mailFolder 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="88f34-212">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="88f34-213">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="88f34-213">totalItemCount</span></span>|<span data-ttu-id="88f34-214">Int32</span><span class="sxs-lookup"><span data-stu-id="88f34-214">Int32</span></span>|<span data-ttu-id="88f34-215">邮箱中项的数量</span><span class="sxs-lookup"><span data-stu-id="88f34-215">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="88f34-216">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="88f34-216">unreadItemCount</span></span>|<span data-ttu-id="88f34-217">Int32</span><span class="sxs-lookup"><span data-stu-id="88f34-217">Int32</span></span>|<span data-ttu-id="88f34-218">mailFolder 中标记为未读的项的数量。</span><span class="sxs-lookup"><span data-stu-id="88f34-218">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="88f34-219">**有效的访问项计数**</span><span class="sxs-lookup"><span data-stu-id="88f34-219">**Access item counts efficiently**</span></span>

<span data-ttu-id="88f34-220">文件夹的 `TotalItemCount` 和 `UnreadItemCount` 属性允许您方便地计算文件夹中读取项目的数量。</span><span class="sxs-lookup"><span data-stu-id="88f34-220">The TotalItemCount and UnreadItemCount properties of a folder allow you to conveniently compute the number of read items in the folder. They let you avoid queries like the following that can incur significant latency:</span></span>
<span data-ttu-id="88f34-221">它们让你避免像下面这样会引起严重延迟的查询：</span><span class="sxs-lookup"><span data-stu-id="88f34-221">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="88f34-222">Outlook 中的邮件文件夹可以包含多个类型的项，例如，收件箱可以包含不同于邮件项的会议请求项。</span><span class="sxs-lookup"><span data-stu-id="88f34-222">MailFolders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items. TotalItemCount and UnreadItemCount include items in a mailFolder irrespective of their item types.</span></span> <span data-ttu-id="88f34-223">`TotalItemCount` 和 `UnreadItemCount` 会计入文件夹中的项目，而无论项目的类型如何。</span><span class="sxs-lookup"><span data-stu-id="88f34-223">`TotalItemCount` and `UnreadItemCount` include items in a folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="88f34-224">关系</span><span class="sxs-lookup"><span data-stu-id="88f34-224">Relationships</span></span>

| <span data-ttu-id="88f34-225">关系</span><span class="sxs-lookup"><span data-stu-id="88f34-225">Relationship</span></span> | <span data-ttu-id="88f34-226">类型</span><span class="sxs-lookup"><span data-stu-id="88f34-226">Type</span></span> | <span data-ttu-id="88f34-227">说明</span><span class="sxs-lookup"><span data-stu-id="88f34-227">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="88f34-228">childFolders</span><span class="sxs-lookup"><span data-stu-id="88f34-228">childFolders</span></span>|<span data-ttu-id="88f34-229">[MailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88f34-229">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="88f34-230">mailFolder 中的子文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="88f34-230">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="88f34-231">messageRules</span><span class="sxs-lookup"><span data-stu-id="88f34-231">messageRules</span></span> | <span data-ttu-id="88f34-232">[messageRule](messagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88f34-232">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="88f34-233">适用于用户“收件箱”文件夹的规则集合。</span><span class="sxs-lookup"><span data-stu-id="88f34-233">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="88f34-234">消息</span><span class="sxs-lookup"><span data-stu-id="88f34-234">messages</span></span>|<span data-ttu-id="88f34-235">[邮件](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88f34-235">[Message](message.md) collection</span></span>|<span data-ttu-id="88f34-236">mailFolder 中的邮件集合。</span><span class="sxs-lookup"><span data-stu-id="88f34-236">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="88f34-237">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="88f34-237">multiValueExtendedProperties</span></span>|<span data-ttu-id="88f34-238">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88f34-238">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="88f34-p109">为 mailFolder 定义的多值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="88f34-p109">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="88f34-242">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="88f34-242">singleValueExtendedProperties</span></span>|<span data-ttu-id="88f34-243">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88f34-243">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="88f34-p110">为 mailFolder 定义的单值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="88f34-p110">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88f34-247">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88f34-247">JSON representation</span></span>

<span data-ttu-id="88f34-248">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88f34-248">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mailFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "changeTracking": false,
        "navigability": "single",
        "searchable": false
      }
    },
    {
      "property": "messageRules",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single"
      }
    }
  ]
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
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a><span data-ttu-id="88f34-249">另请参阅</span><span class="sxs-lookup"><span data-stu-id="88f34-249">See also</span></span>

- [<span data-ttu-id="88f34-250">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="88f34-250">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="88f34-251">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="88f34-251">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
