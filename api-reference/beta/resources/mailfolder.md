---
title: mailFolder 资源类型
description: 用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。 邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。
ms.openlocfilehash: 49fd4571e3ebe35e04e4da4276c1816829ebc599
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044149"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="d42ad-104">mailFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="d42ad-104">mailFolder resource type</span></span>

> <span data-ttu-id="d42ad-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d42ad-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d42ad-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d42ad-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d42ad-107">用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。</span><span class="sxs-lookup"><span data-stu-id="d42ad-107">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="d42ad-108">邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ad-108">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="d42ad-109">该资源支持通过提供 [delta](../api/mailfolder-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="d42ad-109">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="d42ad-110">**已知文件夹名称**</span><span class="sxs-lookup"><span data-stu-id="d42ad-110">**Well-known folder names**</span></span>

<span data-ttu-id="d42ad-111">Outlook 默认情况下会为用户创建某些文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ad-111">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="d42ad-112">访问这些文件夹时，而不是使用的相应文件夹**id**值，为方便起见，您可以使用下表中的已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="d42ad-112">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="d42ad-113">例如，您可以获取其已知名称使用以下查询草稿文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ad-113">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="d42ad-114">已知名称工作无论用户的邮箱的区域设置上述查询将始终返回命名方式无论用户的草稿文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ad-114">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="d42ad-115">已知文件夹名称</span><span class="sxs-lookup"><span data-stu-id="d42ad-115">Well-known folder name</span></span> | <span data-ttu-id="d42ad-116">说明</span><span class="sxs-lookup"><span data-stu-id="d42ad-116">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="d42ad-117">存档</span><span class="sxs-lookup"><span data-stu-id="d42ad-117">archive</span></span> | <span data-ttu-id="d42ad-118">存档文件夹邮件发送到在支持的 Outlook 客户端使用 One_Click 存档功能时。</span><span class="sxs-lookup"><span data-stu-id="d42ad-118">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="d42ad-119">**注意：** 这是不相同的存档邮箱功能的 Exchange online。</span><span class="sxs-lookup"><span data-stu-id="d42ad-119">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="d42ad-120">混乱</span><span class="sxs-lookup"><span data-stu-id="d42ad-120">clutter</span></span> | <span data-ttu-id="d42ad-121">混乱文件夹低优先级邮件移动到时使用的混乱功能。</span><span class="sxs-lookup"><span data-stu-id="d42ad-121">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="d42ad-122">冲突</span><span class="sxs-lookup"><span data-stu-id="d42ad-122">conflicts</span></span> | <span data-ttu-id="d42ad-123">包含邮箱中的冲突项目的文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ad-123">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="d42ad-124">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="d42ad-124">conversationhistory</span></span> | <span data-ttu-id="d42ad-125">其中 Skype 保存 IM 对话 （如果 Skype 配置这样） 中的文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ad-125">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="d42ad-126">DeletedItems</span><span class="sxs-lookup"><span data-stu-id="d42ad-126">deleteditems</span></span> | <span data-ttu-id="d42ad-127">文件夹项目移到时被删除。</span><span class="sxs-lookup"><span data-stu-id="d42ad-127">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="d42ad-128">草稿</span><span class="sxs-lookup"><span data-stu-id="d42ad-128">drafts</span></span> | <span data-ttu-id="d42ad-129">包含未发送的邮件的文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ad-129">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="d42ad-130">收件箱</span><span class="sxs-lookup"><span data-stu-id="d42ad-130">inbox</span></span> | <span data-ttu-id="d42ad-131">收件箱文件夹中。</span><span class="sxs-lookup"><span data-stu-id="d42ad-131">The inbox folder.</span></span> |
| <span data-ttu-id="d42ad-132">junkemail</span><span class="sxs-lookup"><span data-stu-id="d42ad-132">junkemail</span></span> | <span data-ttu-id="d42ad-133">垃圾邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="d42ad-133">The junk email folder.</span></span> |
| <span data-ttu-id="d42ad-134">localfailures</span><span class="sxs-lookup"><span data-stu-id="d42ad-134">localfailures</span></span> | <span data-ttu-id="d42ad-135">包含本地客户端上存在，但无法上载到服务器的项目的文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ad-135">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="d42ad-136">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="d42ad-136">msgfolderroot</span></span> | <span data-ttu-id="d42ad-137">"顶部的信息存储"文件夹中。</span><span class="sxs-lookup"><span data-stu-id="d42ad-137">The "Top of Information Store" folder.</span></span> <span data-ttu-id="d42ad-138">此文件夹的父文件夹的普通邮件客户端，如收件箱中显示的文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ad-138">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="d42ad-139">发件箱</span><span class="sxs-lookup"><span data-stu-id="d42ad-139">outbox</span></span> | <span data-ttu-id="d42ad-140">发件箱文件夹中。</span><span class="sxs-lookup"><span data-stu-id="d42ad-140">The outbox folder.</span></span> |
| <span data-ttu-id="d42ad-141">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="d42ad-141">recoverableitemsdeletions</span></span> | <span data-ttu-id="d42ad-142">包含软删除项目的文件夹： 删除从已删除邮件文件夹中，或通过按 shift + delete 在 Outlook 中。</span><span class="sxs-lookup"><span data-stu-id="d42ad-142">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="d42ad-143">此文件夹不可见在任何 Outlook 电子邮件客户端，但是与其进行交互的最终用户可以通过中 Outlook 或 Outlook web 上的**从服务器恢复已删除邮件**功能。</span><span class="sxs-lookup"><span data-stu-id="d42ad-143">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="d42ad-144">已计划</span><span class="sxs-lookup"><span data-stu-id="d42ad-144">scheduled</span></span> | <span data-ttu-id="d42ad-145">包含计划重新显示在适用于 iOS 的 Outlook 中使用的日程安排功能收件箱中的邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ad-145">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="d42ad-146">searchfolders</span><span class="sxs-lookup"><span data-stu-id="d42ad-146">searchfolders</span></span> | <span data-ttu-id="d42ad-147">在用户的邮箱中定义的所有搜索文件夹的父文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ad-147">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="d42ad-148">sentitems</span><span class="sxs-lookup"><span data-stu-id="d42ad-148">sentitems</span></span> | <span data-ttu-id="d42ad-149">已发送的邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="d42ad-149">The sent items folder.</span></span> |
| <span data-ttu-id="d42ad-150">serverfailures</span><span class="sxs-lookup"><span data-stu-id="d42ad-150">serverfailures</span></span> | <span data-ttu-id="d42ad-151">包含服务器上存在，但无法同步到本地客户端的项目的文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ad-151">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="d42ad-152">syncissues</span><span class="sxs-lookup"><span data-stu-id="d42ad-152">syncissues</span></span> | <span data-ttu-id="d42ad-153">包含由 Outlook 创建的同步日志的文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ad-153">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="d42ad-154">方法</span><span class="sxs-lookup"><span data-stu-id="d42ad-154">Methods</span></span>

| <span data-ttu-id="d42ad-155">方法</span><span class="sxs-lookup"><span data-stu-id="d42ad-155">Method</span></span> | <span data-ttu-id="d42ad-156">返回类型</span><span class="sxs-lookup"><span data-stu-id="d42ad-156">Return Type</span></span> | <span data-ttu-id="d42ad-157">说明</span><span class="sxs-lookup"><span data-stu-id="d42ad-157">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="d42ad-158">获取 mailFolder</span><span class="sxs-lookup"><span data-stu-id="d42ad-158">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="d42ad-159">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d42ad-159">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="d42ad-160">读取 mailFolder 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d42ad-160">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="d42ad-161">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="d42ad-161">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="d42ad-162">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d42ad-162">mailFolder</span></span>](mailfolder.md)| <span data-ttu-id="d42ad-163">通过发布到 childFolder 集合，在当前 mailFolder 下新建 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="d42ad-163">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="d42ad-164">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="d42ad-164">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="d42ad-165">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d42ad-165">[mailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="d42ad-p108">获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ad-p108">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="d42ad-168">创建邮件</span><span class="sxs-lookup"><span data-stu-id="d42ad-168">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="d42ad-169">message</span><span class="sxs-lookup"><span data-stu-id="d42ad-169">message</span></span>](message.md)| <span data-ttu-id="d42ad-170">通过发布到邮件集合，在当前 mailFolder 中新建邮件。</span><span class="sxs-lookup"><span data-stu-id="d42ad-170">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="d42ad-171">列出邮件</span><span class="sxs-lookup"><span data-stu-id="d42ad-171">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="d42ad-172">[邮件](message.md)集合</span><span class="sxs-lookup"><span data-stu-id="d42ad-172">[message](message.md) collection</span></span>| <span data-ttu-id="d42ad-173">获取已登录用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。</span><span class="sxs-lookup"><span data-stu-id="d42ad-173">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="d42ad-174">更新</span><span class="sxs-lookup"><span data-stu-id="d42ad-174">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="d42ad-175">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d42ad-175">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="d42ad-176">更新指定的 mailFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="d42ad-176">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="d42ad-177">删除</span><span class="sxs-lookup"><span data-stu-id="d42ad-177">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="d42ad-178">无</span><span class="sxs-lookup"><span data-stu-id="d42ad-178">None</span></span> |<span data-ttu-id="d42ad-179">删除指定的 mailFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="d42ad-179">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="d42ad-180">复制</span><span class="sxs-lookup"><span data-stu-id="d42ad-180">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="d42ad-181">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d42ad-181">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="d42ad-182">将 mailfolder 及其内容复制到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="d42ad-182">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="d42ad-183">delta</span><span class="sxs-lookup"><span data-stu-id="d42ad-183">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="d42ad-184">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d42ad-184">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="d42ad-185">获取用户邮箱中已添加、删除或移除的邮件文件夹集。</span><span class="sxs-lookup"><span data-stu-id="d42ad-185">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="d42ad-186">移动</span><span class="sxs-lookup"><span data-stu-id="d42ad-186">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="d42ad-187">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d42ad-187">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="d42ad-188">将 mailFolder 及其内容移动到其他 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="d42ad-188">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="d42ad-189">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="d42ad-189">**Extended properties**</span></span>| | |
|[<span data-ttu-id="d42ad-190">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="d42ad-190">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="d42ad-191">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d42ad-191">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="d42ad-192">在新建或现有的 mailFolder 中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d42ad-192">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="d42ad-193">获取具有单值扩展属性的 mailFolder</span><span class="sxs-lookup"><span data-stu-id="d42ad-193">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="d42ad-194">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d42ad-194">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="d42ad-195">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="d42ad-195">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="d42ad-196">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="d42ad-196">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="d42ad-197">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d42ad-197">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="d42ad-198">在新建或现有的 mailFolder 中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d42ad-198">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="d42ad-199">获取具有多值扩展属性的 mailFolder</span><span class="sxs-lookup"><span data-stu-id="d42ad-199">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="d42ad-200">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d42ad-200">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="d42ad-201">使用 `$expand` 获取包含一个多值扩展属性的 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="d42ad-201">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="d42ad-202">属性</span><span class="sxs-lookup"><span data-stu-id="d42ad-202">Properties</span></span>

| <span data-ttu-id="d42ad-203">属性</span><span class="sxs-lookup"><span data-stu-id="d42ad-203">Property</span></span> | <span data-ttu-id="d42ad-204">类型</span><span class="sxs-lookup"><span data-stu-id="d42ad-204">Type</span></span> | <span data-ttu-id="d42ad-205">说明</span><span class="sxs-lookup"><span data-stu-id="d42ad-205">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="d42ad-206">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="d42ad-206">childFolderCount</span></span>|<span data-ttu-id="d42ad-207">Int32</span><span class="sxs-lookup"><span data-stu-id="d42ad-207">Int32</span></span>|<span data-ttu-id="d42ad-208">当前 mailFolder 中的直接子 mailFolder 数量。</span><span class="sxs-lookup"><span data-stu-id="d42ad-208">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="d42ad-209">displayName</span><span class="sxs-lookup"><span data-stu-id="d42ad-209">displayName</span></span>|<span data-ttu-id="d42ad-210">String</span><span class="sxs-lookup"><span data-stu-id="d42ad-210">String</span></span>|<span data-ttu-id="d42ad-211">mailFolder 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d42ad-211">The mailFolder's display name.</span></span>|
|<span data-ttu-id="d42ad-212">id</span><span class="sxs-lookup"><span data-stu-id="d42ad-212">id</span></span>|<span data-ttu-id="d42ad-213">字符串</span><span class="sxs-lookup"><span data-stu-id="d42ad-213">String</span></span>|<span data-ttu-id="d42ad-214">MailFolder 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d42ad-214">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="d42ad-215">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="d42ad-215">parentFolderId</span></span>|<span data-ttu-id="d42ad-216">String</span><span class="sxs-lookup"><span data-stu-id="d42ad-216">String</span></span>|<span data-ttu-id="d42ad-217">MailFolder 的父 mailFolder 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d42ad-217">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="d42ad-218">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="d42ad-218">totalItemCount</span></span>|<span data-ttu-id="d42ad-219">Int32</span><span class="sxs-lookup"><span data-stu-id="d42ad-219">Int32</span></span>|<span data-ttu-id="d42ad-220">邮箱中项的数量</span><span class="sxs-lookup"><span data-stu-id="d42ad-220">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="d42ad-221">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="d42ad-221">unreadItemCount</span></span>|<span data-ttu-id="d42ad-222">Int32</span><span class="sxs-lookup"><span data-stu-id="d42ad-222">Int32</span></span>|<span data-ttu-id="d42ad-223">mailFolder 中标记为未读的项的数量。</span><span class="sxs-lookup"><span data-stu-id="d42ad-223">The number of items in the mailFolder marked as unread.</span></span>|
|<span data-ttu-id="d42ad-224">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="d42ad-224">wellKnownName</span></span>|<span data-ttu-id="d42ad-225">字符串</span><span class="sxs-lookup"><span data-stu-id="d42ad-225">String</span></span>|<span data-ttu-id="d42ad-226">文件夹的已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="d42ad-226">The well-known folder name for the folder.</span></span> <span data-ttu-id="d42ad-227">上面列出了可能的值。</span><span class="sxs-lookup"><span data-stu-id="d42ad-227">The possible values are listed above.</span></span> <span data-ttu-id="d42ad-228">此属性仅对于创建的 Outlook 默认文件夹设置。</span><span class="sxs-lookup"><span data-stu-id="d42ad-228">This property is only set for default folders created by Outlook.</span></span> <span data-ttu-id="d42ad-229">有关其他文件夹，此属性为**null**。</span><span class="sxs-lookup"><span data-stu-id="d42ad-229">For other folders, this property is **null**.</span></span>|

<span data-ttu-id="d42ad-230">**有效的访问项计数**</span><span class="sxs-lookup"><span data-stu-id="d42ad-230">**Access item counts efficiently**</span></span>

<span data-ttu-id="d42ad-231">`TotalItemCount`和`UnreadItemCount`文件夹的属性，可以方便地计算的文件夹中的读取项目数。</span><span class="sxs-lookup"><span data-stu-id="d42ad-231">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="d42ad-232">它们使您可以避免查询会引发大量延迟如下：</span><span class="sxs-lookup"><span data-stu-id="d42ad-232">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/beta/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="d42ad-233">在 Outlook 中的邮件文件夹可以包含多个类型的项目，例如，可以包含收件箱会议请求项目的不同邮件项目。</span><span class="sxs-lookup"><span data-stu-id="d42ad-233">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="d42ad-234">`TotalItemCount`和`UnreadItemCount`包括而不考虑其项目类型的邮件文件夹中的项目。</span><span class="sxs-lookup"><span data-stu-id="d42ad-234">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="d42ad-235">Relationships</span><span class="sxs-lookup"><span data-stu-id="d42ad-235">Relationships</span></span>

| <span data-ttu-id="d42ad-236">关系</span><span class="sxs-lookup"><span data-stu-id="d42ad-236">Relationship</span></span> | <span data-ttu-id="d42ad-237">类型</span><span class="sxs-lookup"><span data-stu-id="d42ad-237">Type</span></span> | <span data-ttu-id="d42ad-238">说明</span><span class="sxs-lookup"><span data-stu-id="d42ad-238">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="d42ad-239">childFolders</span><span class="sxs-lookup"><span data-stu-id="d42ad-239">childFolders</span></span>|<span data-ttu-id="d42ad-240">[MailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d42ad-240">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="d42ad-241">mailFolder 中的子文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="d42ad-241">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="d42ad-242">messageRules</span><span class="sxs-lookup"><span data-stu-id="d42ad-242">messageRules</span></span> | <span data-ttu-id="d42ad-243">[messageRule](messagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d42ad-243">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="d42ad-244">适用于用户“收件箱”文件夹的规则集合。</span><span class="sxs-lookup"><span data-stu-id="d42ad-244">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="d42ad-245">messages</span><span class="sxs-lookup"><span data-stu-id="d42ad-245">messages</span></span>|<span data-ttu-id="d42ad-246">[邮件](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d42ad-246">[Message](message.md) collection</span></span>|<span data-ttu-id="d42ad-247">mailFolder 中的邮件集合。</span><span class="sxs-lookup"><span data-stu-id="d42ad-247">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="d42ad-248">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d42ad-248">multiValueExtendedProperties</span></span>|<span data-ttu-id="d42ad-249">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d42ad-249">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d42ad-p112">为 mailFolder 定义的多值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d42ad-p112">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d42ad-253">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d42ad-253">singleValueExtendedProperties</span></span>|<span data-ttu-id="d42ad-254">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="d42ad-254">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d42ad-p113">为 mailFolder 定义的单值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d42ad-p113">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d42ad-258">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d42ad-258">JSON representation</span></span>

<span data-ttu-id="d42ad-259">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d42ad-259">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
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
  "wellKnownName": "string",
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a><span data-ttu-id="d42ad-260">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d42ad-260">See also</span></span>

- [<span data-ttu-id="d42ad-261">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="d42ad-261">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="d42ad-262">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="d42ad-262">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
