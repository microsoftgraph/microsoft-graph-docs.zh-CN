---
title: mailFolder 资源类型
description: 用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。 邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0de32560e154eaa732e596040525025ad0676926
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448016"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="b6303-104">mailFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6303-104">mailFolder resource type</span></span>

<span data-ttu-id="b6303-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6303-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6303-106">用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。</span><span class="sxs-lookup"><span data-stu-id="b6303-106">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="b6303-107">邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-107">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="b6303-108">该资源支持通过提供 [delta](../api/mailfolder-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="b6303-108">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="b6303-109">**已知文件夹名称**</span><span class="sxs-lookup"><span data-stu-id="b6303-109">**Well-known folder names**</span></span>

<span data-ttu-id="b6303-110">Outlook 默认情况下会为用户创建某些文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-110">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="b6303-111">为方便起见，可以在访问这些文件夹时使用已知的文件夹名称来替代使用相应的文件夹 **id** 值。</span><span class="sxs-lookup"><span data-stu-id="b6303-111">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="b6303-112">例如，你可以使用其已知名称和以下查询来获取“草稿”文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-112">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="b6303-113">无论用户邮箱的区域设置如何，已知名称都可以工作，因此无论命名方式如何，上述查询都将始终返回用户的“草稿”文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-113">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="b6303-114">已知文件夹名称</span><span class="sxs-lookup"><span data-stu-id="b6303-114">Well-known folder name</span></span> | <span data-ttu-id="b6303-115">说明</span><span class="sxs-lookup"><span data-stu-id="b6303-115">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="b6303-116">archive</span><span class="sxs-lookup"><span data-stu-id="b6303-116">archive</span></span> | <span data-ttu-id="b6303-117">在支持它的 Outlook 客户端中使用 One_Click 存档功能时，将发送存档文件夹邮件。</span><span class="sxs-lookup"><span data-stu-id="b6303-117">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="b6303-118">**注意：** 这与 Exchange Online 的存档邮箱功能并不相同。</span><span class="sxs-lookup"><span data-stu-id="b6303-118">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="b6303-119">clutter</span><span class="sxs-lookup"><span data-stu-id="b6303-119">clutter</span></span> | <span data-ttu-id="b6303-120">使用待筛选邮件功能时，待筛选文件夹低优先级邮件将被移动到这里。</span><span class="sxs-lookup"><span data-stu-id="b6303-120">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="b6303-121">conflicts</span><span class="sxs-lookup"><span data-stu-id="b6303-121">conflicts</span></span> | <span data-ttu-id="b6303-122">包含邮箱中冲突项的文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-122">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="b6303-123">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="b6303-123">conversationhistory</span></span> | <span data-ttu-id="b6303-124">Skype 保存 IM 对话的文件夹（如果 Skype 配置为这样做）。</span><span class="sxs-lookup"><span data-stu-id="b6303-124">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="b6303-125">deleteditems</span><span class="sxs-lookup"><span data-stu-id="b6303-125">deleteditems</span></span> | <span data-ttu-id="b6303-126">文件夹项被删除时，将被移动到这里。</span><span class="sxs-lookup"><span data-stu-id="b6303-126">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="b6303-127">drafts</span><span class="sxs-lookup"><span data-stu-id="b6303-127">drafts</span></span> | <span data-ttu-id="b6303-128">包含未发送邮件的文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-128">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="b6303-129">inbox</span><span class="sxs-lookup"><span data-stu-id="b6303-129">inbox</span></span> | <span data-ttu-id="b6303-130">收件箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-130">The inbox folder.</span></span> |
| <span data-ttu-id="b6303-131">junkemail</span><span class="sxs-lookup"><span data-stu-id="b6303-131">junkemail</span></span> | <span data-ttu-id="b6303-132">“垃圾邮件”文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-132">The junk email folder.</span></span> |
| <span data-ttu-id="b6303-133">localfailures</span><span class="sxs-lookup"><span data-stu-id="b6303-133">localfailures</span></span> | <span data-ttu-id="b6303-134">包含本地客户端上存在但无法上载到服务器的项的文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-134">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="b6303-135">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="b6303-135">msgfolderroot</span></span> | <span data-ttu-id="b6303-136">“最上层的信息文件”文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-136">The "Top of Information Store" folder.</span></span> <span data-ttu-id="b6303-137">此文件夹是在普通邮件客户端（如收件箱）中显示的文件夹的父文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-137">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="b6303-138">outbox</span><span class="sxs-lookup"><span data-stu-id="b6303-138">outbox</span></span> | <span data-ttu-id="b6303-139">“发件箱”文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-139">The outbox folder.</span></span> |
| <span data-ttu-id="b6303-140">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="b6303-140">recoverableitemsdeletions</span></span> | <span data-ttu-id="b6303-141">包含软删除项的文件夹：从“已删除邮件”文件夹中删除，或者在 Outlook 中按 shift+delete 删除。</span><span class="sxs-lookup"><span data-stu-id="b6303-141">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="b6303-142">此文件夹在任何 Outlook 电子邮件客户端中都不可见，但最终用户可以通过 Outlook 中的“**从服务器恢复已删除邮件**”功能或 Web 上的 Outlook 与其进行交互。</span><span class="sxs-lookup"><span data-stu-id="b6303-142">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="b6303-143">scheduled</span><span class="sxs-lookup"><span data-stu-id="b6303-143">scheduled</span></span> | <span data-ttu-id="b6303-144">包含计划使用 Outlook for iOS 中的“计划”功能重新出现在收件箱中的邮件的文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-144">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="b6303-145">searchfolders</span><span class="sxs-lookup"><span data-stu-id="b6303-145">searchfolders</span></span> | <span data-ttu-id="b6303-146">用户邮箱中定义的所有搜索文件夹的父文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-146">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="b6303-147">sentitems</span><span class="sxs-lookup"><span data-stu-id="b6303-147">sentitems</span></span> | <span data-ttu-id="b6303-148">已发送项的文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-148">The sent items folder.</span></span> |
| <span data-ttu-id="b6303-149">serverfailures</span><span class="sxs-lookup"><span data-stu-id="b6303-149">serverfailures</span></span> | <span data-ttu-id="b6303-150">包含服务器上存在但无法同步到本地客户端的项的文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-150">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="b6303-151">syncissues</span><span class="sxs-lookup"><span data-stu-id="b6303-151">syncissues</span></span> | <span data-ttu-id="b6303-152">包含 Outlook 创建的同步日志的文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-152">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="b6303-153">方法</span><span class="sxs-lookup"><span data-stu-id="b6303-153">Methods</span></span>

| <span data-ttu-id="b6303-154">方法</span><span class="sxs-lookup"><span data-stu-id="b6303-154">Method</span></span> | <span data-ttu-id="b6303-155">返回类型</span><span class="sxs-lookup"><span data-stu-id="b6303-155">Return Type</span></span> | <span data-ttu-id="b6303-156">说明</span><span class="sxs-lookup"><span data-stu-id="b6303-156">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="b6303-157">获取 mailFolder</span><span class="sxs-lookup"><span data-stu-id="b6303-157">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="b6303-158">mailFolder</span><span class="sxs-lookup"><span data-stu-id="b6303-158">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="b6303-159">读取 mailFolder 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b6303-159">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="b6303-160">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="b6303-160">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="b6303-161">MailFolder</span><span class="sxs-lookup"><span data-stu-id="b6303-161">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="b6303-162">通过发布到 childFolder 集合，在当前 mailFolder 下新建 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="b6303-162">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="b6303-163">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="b6303-163">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="b6303-164">[MailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b6303-164">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="b6303-p107">获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6303-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="b6303-167">创建邮件</span><span class="sxs-lookup"><span data-stu-id="b6303-167">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="b6303-168">邮件</span><span class="sxs-lookup"><span data-stu-id="b6303-168">Message</span></span>](message.md)| <span data-ttu-id="b6303-169">通过发布到邮件集合，在当前 mailFolder 中新建邮件。</span><span class="sxs-lookup"><span data-stu-id="b6303-169">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="b6303-170">列出邮件</span><span class="sxs-lookup"><span data-stu-id="b6303-170">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="b6303-171">[邮件](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b6303-171">[Message](message.md) collection</span></span>| <span data-ttu-id="b6303-172">获取已登录用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。</span><span class="sxs-lookup"><span data-stu-id="b6303-172">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="b6303-173">更新</span><span class="sxs-lookup"><span data-stu-id="b6303-173">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="b6303-174">mailFolder</span><span class="sxs-lookup"><span data-stu-id="b6303-174">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="b6303-175">更新指定的 mailFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="b6303-175">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="b6303-176">删除</span><span class="sxs-lookup"><span data-stu-id="b6303-176">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="b6303-177">无</span><span class="sxs-lookup"><span data-stu-id="b6303-177">None</span></span> |<span data-ttu-id="b6303-178">删除指定的 mailFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="b6303-178">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="b6303-179">复制</span><span class="sxs-lookup"><span data-stu-id="b6303-179">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="b6303-180">MailFolder</span><span class="sxs-lookup"><span data-stu-id="b6303-180">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="b6303-181">将 mailfolder 及其内容复制到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="b6303-181">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="b6303-182">delta</span><span class="sxs-lookup"><span data-stu-id="b6303-182">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="b6303-183">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b6303-183">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="b6303-184">获取用户邮箱中已添加、删除或移除的邮件文件夹集。</span><span class="sxs-lookup"><span data-stu-id="b6303-184">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="b6303-185">移动</span><span class="sxs-lookup"><span data-stu-id="b6303-185">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="b6303-186">MailFolder</span><span class="sxs-lookup"><span data-stu-id="b6303-186">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="b6303-187">将 mailFolder 及其内容移动到其他 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="b6303-187">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="b6303-188">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="b6303-188">**Extended properties**</span></span>| | |
|[<span data-ttu-id="b6303-189">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="b6303-189">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="b6303-190">mailFolder</span><span class="sxs-lookup"><span data-stu-id="b6303-190">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="b6303-191">在新建或现有的 mailFolder 中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b6303-191">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="b6303-192">获取具有单值扩展属性的 mailFolder</span><span class="sxs-lookup"><span data-stu-id="b6303-192">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="b6303-193">mailFolder</span><span class="sxs-lookup"><span data-stu-id="b6303-193">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="b6303-194">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="b6303-194">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="b6303-195">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="b6303-195">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="b6303-196">mailFolder</span><span class="sxs-lookup"><span data-stu-id="b6303-196">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="b6303-197">在新建或现有的 mailFolder 中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b6303-197">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="b6303-198">获取具有多值扩展属性的 mailFolder</span><span class="sxs-lookup"><span data-stu-id="b6303-198">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="b6303-199">mailFolder</span><span class="sxs-lookup"><span data-stu-id="b6303-199">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="b6303-200">使用 `$expand` 获取包含一个多值扩展属性的 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="b6303-200">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="b6303-201">属性</span><span class="sxs-lookup"><span data-stu-id="b6303-201">Properties</span></span>

| <span data-ttu-id="b6303-202">属性</span><span class="sxs-lookup"><span data-stu-id="b6303-202">Property</span></span> | <span data-ttu-id="b6303-203">类型</span><span class="sxs-lookup"><span data-stu-id="b6303-203">Type</span></span> | <span data-ttu-id="b6303-204">说明</span><span class="sxs-lookup"><span data-stu-id="b6303-204">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="b6303-205">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="b6303-205">childFolderCount</span></span>|<span data-ttu-id="b6303-206">Int32</span><span class="sxs-lookup"><span data-stu-id="b6303-206">Int32</span></span>|<span data-ttu-id="b6303-207">当前 mailFolder 中的直接子 mailFolder 数量。</span><span class="sxs-lookup"><span data-stu-id="b6303-207">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="b6303-208">displayName</span><span class="sxs-lookup"><span data-stu-id="b6303-208">displayName</span></span>|<span data-ttu-id="b6303-209">String</span><span class="sxs-lookup"><span data-stu-id="b6303-209">String</span></span>|<span data-ttu-id="b6303-210">mailFolder 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b6303-210">The mailFolder's display name.</span></span>|
|<span data-ttu-id="b6303-211">id</span><span class="sxs-lookup"><span data-stu-id="b6303-211">id</span></span>|<span data-ttu-id="b6303-212">String</span><span class="sxs-lookup"><span data-stu-id="b6303-212">String</span></span>|<span data-ttu-id="b6303-213">MailFolder 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b6303-213">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="b6303-214">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="b6303-214">parentFolderId</span></span>|<span data-ttu-id="b6303-215">String</span><span class="sxs-lookup"><span data-stu-id="b6303-215">String</span></span>|<span data-ttu-id="b6303-216">MailFolder 的父 mailFolder 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b6303-216">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="b6303-217">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="b6303-217">totalItemCount</span></span>|<span data-ttu-id="b6303-218">Int32</span><span class="sxs-lookup"><span data-stu-id="b6303-218">Int32</span></span>|<span data-ttu-id="b6303-219">邮箱中项的数量</span><span class="sxs-lookup"><span data-stu-id="b6303-219">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="b6303-220">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="b6303-220">unreadItemCount</span></span>|<span data-ttu-id="b6303-221">Int32</span><span class="sxs-lookup"><span data-stu-id="b6303-221">Int32</span></span>|<span data-ttu-id="b6303-222">mailFolder 中标记为未读的项的数量。</span><span class="sxs-lookup"><span data-stu-id="b6303-222">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="b6303-223">**有效的访问项计数**</span><span class="sxs-lookup"><span data-stu-id="b6303-223">**Access item counts efficiently**</span></span>

<span data-ttu-id="b6303-224">使用文件夹的 `TotalItemCount` 和 `UnreadItemCount` 的属性可以方便地计算在文件夹中读取的项数。</span><span class="sxs-lookup"><span data-stu-id="b6303-224">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="b6303-225">使你避免进行可产生重大延迟的查询，如下所示：</span><span class="sxs-lookup"><span data-stu-id="b6303-225">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="b6303-226">Outlook 中的邮件文件夹可包含多个类型的项，例如，收件箱可以包含不同于邮件项的会议请求项。</span><span class="sxs-lookup"><span data-stu-id="b6303-226">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="b6303-227">`TotalItemCount` 和 `UnreadItemCount`包括邮件文件夹中的项，无论其项类型如何。</span><span class="sxs-lookup"><span data-stu-id="b6303-227">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="b6303-228">关系</span><span class="sxs-lookup"><span data-stu-id="b6303-228">Relationships</span></span>

| <span data-ttu-id="b6303-229">关系</span><span class="sxs-lookup"><span data-stu-id="b6303-229">Relationship</span></span> | <span data-ttu-id="b6303-230">类型</span><span class="sxs-lookup"><span data-stu-id="b6303-230">Type</span></span> | <span data-ttu-id="b6303-231">说明</span><span class="sxs-lookup"><span data-stu-id="b6303-231">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="b6303-232">childFolders</span><span class="sxs-lookup"><span data-stu-id="b6303-232">childFolders</span></span>|<span data-ttu-id="b6303-233">[MailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b6303-233">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="b6303-234">mailFolder 中的子文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="b6303-234">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="b6303-235">messageRules</span><span class="sxs-lookup"><span data-stu-id="b6303-235">messageRules</span></span> | <span data-ttu-id="b6303-236">[messageRule](messagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b6303-236">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="b6303-237">适用于用户“收件箱”文件夹的规则集合。</span><span class="sxs-lookup"><span data-stu-id="b6303-237">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="b6303-238">messages</span><span class="sxs-lookup"><span data-stu-id="b6303-238">messages</span></span>|<span data-ttu-id="b6303-239">[邮件](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b6303-239">[Message](message.md) collection</span></span>|<span data-ttu-id="b6303-240">mailFolder 中的邮件集合。</span><span class="sxs-lookup"><span data-stu-id="b6303-240">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="b6303-241">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b6303-241">multiValueExtendedProperties</span></span>|<span data-ttu-id="b6303-242">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b6303-242">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b6303-p110">为 mailFolder 定义的多值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="b6303-p110">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b6303-246">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b6303-246">singleValueExtendedProperties</span></span>|<span data-ttu-id="b6303-247">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="b6303-247">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b6303-p111">为 mailFolder 定义的单值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="b6303-p111">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6303-251">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6303-251">JSON representation</span></span>

<span data-ttu-id="b6303-252">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6303-252">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="b6303-253">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b6303-253">See also</span></span>

- [<span data-ttu-id="b6303-254">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="b6303-254">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="b6303-255">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="b6303-255">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
