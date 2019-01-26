---
title: mailFolder 资源类型
description: 用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。 邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 25a491a23840de009386d7fbb2e9ee8d0fef7b4e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576729"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="55f7c-104">mailFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="55f7c-104">mailFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55f7c-105">用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。</span><span class="sxs-lookup"><span data-stu-id="55f7c-105">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="55f7c-106">邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="55f7c-106">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="55f7c-107">该资源支持通过提供 [delta](../api/mailfolder-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="55f7c-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="55f7c-108">**已知文件夹名称**</span><span class="sxs-lookup"><span data-stu-id="55f7c-108">**Well-known folder names**</span></span>

<span data-ttu-id="55f7c-109">Outlook 默认情况下会为用户创建某些文件夹。</span><span class="sxs-lookup"><span data-stu-id="55f7c-109">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="55f7c-110">访问这些文件夹时，而不是使用的相应文件夹**id**值，为方便起见，您可以使用下表中的已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="55f7c-110">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="55f7c-111">例如，您可以获取其已知名称使用以下查询草稿文件夹。</span><span class="sxs-lookup"><span data-stu-id="55f7c-111">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="55f7c-112">已知名称工作无论用户的邮箱的区域设置上述查询将始终返回命名方式无论用户的草稿文件夹。</span><span class="sxs-lookup"><span data-stu-id="55f7c-112">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="55f7c-113">已知文件夹名称</span><span class="sxs-lookup"><span data-stu-id="55f7c-113">Well-known folder name</span></span> | <span data-ttu-id="55f7c-114">说明</span><span class="sxs-lookup"><span data-stu-id="55f7c-114">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="55f7c-115">存档</span><span class="sxs-lookup"><span data-stu-id="55f7c-115">archive</span></span> | <span data-ttu-id="55f7c-116">存档文件夹邮件发送到在支持的 Outlook 客户端使用 One_Click 存档功能时。</span><span class="sxs-lookup"><span data-stu-id="55f7c-116">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="55f7c-117">**注意：** 这是不相同的存档邮箱功能的 Exchange online。</span><span class="sxs-lookup"><span data-stu-id="55f7c-117">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="55f7c-118">混乱</span><span class="sxs-lookup"><span data-stu-id="55f7c-118">clutter</span></span> | <span data-ttu-id="55f7c-119">混乱文件夹低优先级邮件移动到时使用的混乱功能。</span><span class="sxs-lookup"><span data-stu-id="55f7c-119">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="55f7c-120">冲突</span><span class="sxs-lookup"><span data-stu-id="55f7c-120">conflicts</span></span> | <span data-ttu-id="55f7c-121">包含邮箱中的冲突项目的文件夹。</span><span class="sxs-lookup"><span data-stu-id="55f7c-121">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="55f7c-122">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="55f7c-122">conversationhistory</span></span> | <span data-ttu-id="55f7c-123">其中 Skype 保存 IM 对话 （如果 Skype 配置这样） 中的文件夹。</span><span class="sxs-lookup"><span data-stu-id="55f7c-123">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="55f7c-124">DeletedItems</span><span class="sxs-lookup"><span data-stu-id="55f7c-124">deleteditems</span></span> | <span data-ttu-id="55f7c-125">文件夹项目移到时被删除。</span><span class="sxs-lookup"><span data-stu-id="55f7c-125">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="55f7c-126">草稿</span><span class="sxs-lookup"><span data-stu-id="55f7c-126">drafts</span></span> | <span data-ttu-id="55f7c-127">包含未发送的邮件的文件夹。</span><span class="sxs-lookup"><span data-stu-id="55f7c-127">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="55f7c-128">收件箱</span><span class="sxs-lookup"><span data-stu-id="55f7c-128">inbox</span></span> | <span data-ttu-id="55f7c-129">收件箱文件夹中。</span><span class="sxs-lookup"><span data-stu-id="55f7c-129">The inbox folder.</span></span> |
| <span data-ttu-id="55f7c-130">junkemail</span><span class="sxs-lookup"><span data-stu-id="55f7c-130">junkemail</span></span> | <span data-ttu-id="55f7c-131">垃圾邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="55f7c-131">The junk email folder.</span></span> |
| <span data-ttu-id="55f7c-132">localfailures</span><span class="sxs-lookup"><span data-stu-id="55f7c-132">localfailures</span></span> | <span data-ttu-id="55f7c-133">包含本地客户端上存在，但无法上载到服务器的项目的文件夹。</span><span class="sxs-lookup"><span data-stu-id="55f7c-133">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="55f7c-134">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="55f7c-134">msgfolderroot</span></span> | <span data-ttu-id="55f7c-135">"顶部的信息存储"文件夹中。</span><span class="sxs-lookup"><span data-stu-id="55f7c-135">The "Top of Information Store" folder.</span></span> <span data-ttu-id="55f7c-136">此文件夹的父文件夹的普通邮件客户端，如收件箱中显示的文件夹。</span><span class="sxs-lookup"><span data-stu-id="55f7c-136">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="55f7c-137">发件箱</span><span class="sxs-lookup"><span data-stu-id="55f7c-137">outbox</span></span> | <span data-ttu-id="55f7c-138">发件箱文件夹中。</span><span class="sxs-lookup"><span data-stu-id="55f7c-138">The outbox folder.</span></span> |
| <span data-ttu-id="55f7c-139">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="55f7c-139">recoverableitemsdeletions</span></span> | <span data-ttu-id="55f7c-140">包含软删除项目的文件夹： 删除从已删除邮件文件夹中，或通过按 shift + delete 在 Outlook 中。</span><span class="sxs-lookup"><span data-stu-id="55f7c-140">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="55f7c-141">此文件夹不可见在任何 Outlook 电子邮件客户端，但是与其进行交互的最终用户可以通过中 Outlook 或 Outlook web 上的**从服务器恢复已删除邮件**功能。</span><span class="sxs-lookup"><span data-stu-id="55f7c-141">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="55f7c-142">已计划</span><span class="sxs-lookup"><span data-stu-id="55f7c-142">scheduled</span></span> | <span data-ttu-id="55f7c-143">包含计划重新显示在适用于 iOS 的 Outlook 中使用的日程安排功能收件箱中的邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="55f7c-143">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="55f7c-144">searchfolders</span><span class="sxs-lookup"><span data-stu-id="55f7c-144">searchfolders</span></span> | <span data-ttu-id="55f7c-145">在用户的邮箱中定义的所有搜索文件夹的父文件夹。</span><span class="sxs-lookup"><span data-stu-id="55f7c-145">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="55f7c-146">sentitems</span><span class="sxs-lookup"><span data-stu-id="55f7c-146">sentitems</span></span> | <span data-ttu-id="55f7c-147">已发送的邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="55f7c-147">The sent items folder.</span></span> |
| <span data-ttu-id="55f7c-148">serverfailures</span><span class="sxs-lookup"><span data-stu-id="55f7c-148">serverfailures</span></span> | <span data-ttu-id="55f7c-149">包含服务器上存在，但无法同步到本地客户端的项目的文件夹。</span><span class="sxs-lookup"><span data-stu-id="55f7c-149">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="55f7c-150">syncissues</span><span class="sxs-lookup"><span data-stu-id="55f7c-150">syncissues</span></span> | <span data-ttu-id="55f7c-151">包含由 Outlook 创建的同步日志的文件夹。</span><span class="sxs-lookup"><span data-stu-id="55f7c-151">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="55f7c-152">方法</span><span class="sxs-lookup"><span data-stu-id="55f7c-152">Methods</span></span>

| <span data-ttu-id="55f7c-153">方法</span><span class="sxs-lookup"><span data-stu-id="55f7c-153">Method</span></span> | <span data-ttu-id="55f7c-154">返回类型</span><span class="sxs-lookup"><span data-stu-id="55f7c-154">Return Type</span></span> | <span data-ttu-id="55f7c-155">说明</span><span class="sxs-lookup"><span data-stu-id="55f7c-155">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="55f7c-156">获取 mailFolder</span><span class="sxs-lookup"><span data-stu-id="55f7c-156">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="55f7c-157">mailFolder</span><span class="sxs-lookup"><span data-stu-id="55f7c-157">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="55f7c-158">读取 mailFolder 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="55f7c-158">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="55f7c-159">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="55f7c-159">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="55f7c-160">mailFolder</span><span class="sxs-lookup"><span data-stu-id="55f7c-160">mailFolder</span></span>](mailfolder.md)| <span data-ttu-id="55f7c-161">通过发布到 childFolder 集合，在当前 mailFolder 下新建 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="55f7c-161">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="55f7c-162">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="55f7c-162">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="55f7c-163">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55f7c-163">[mailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="55f7c-p107">获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="55f7c-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="55f7c-166">创建邮件</span><span class="sxs-lookup"><span data-stu-id="55f7c-166">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="55f7c-167">message</span><span class="sxs-lookup"><span data-stu-id="55f7c-167">message</span></span>](message.md)| <span data-ttu-id="55f7c-168">通过发布到邮件集合，在当前 mailFolder 中新建邮件。</span><span class="sxs-lookup"><span data-stu-id="55f7c-168">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="55f7c-169">列出邮件</span><span class="sxs-lookup"><span data-stu-id="55f7c-169">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="55f7c-170">[邮件](message.md)集合</span><span class="sxs-lookup"><span data-stu-id="55f7c-170">[message](message.md) collection</span></span>| <span data-ttu-id="55f7c-171">获取已登录用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。</span><span class="sxs-lookup"><span data-stu-id="55f7c-171">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="55f7c-172">更新</span><span class="sxs-lookup"><span data-stu-id="55f7c-172">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="55f7c-173">mailFolder</span><span class="sxs-lookup"><span data-stu-id="55f7c-173">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="55f7c-174">更新指定的 mailFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="55f7c-174">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="55f7c-175">删除</span><span class="sxs-lookup"><span data-stu-id="55f7c-175">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="55f7c-176">无</span><span class="sxs-lookup"><span data-stu-id="55f7c-176">None</span></span> |<span data-ttu-id="55f7c-177">删除指定的 mailFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="55f7c-177">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="55f7c-178">复制</span><span class="sxs-lookup"><span data-stu-id="55f7c-178">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="55f7c-179">mailFolder</span><span class="sxs-lookup"><span data-stu-id="55f7c-179">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="55f7c-180">将 mailfolder 及其内容复制到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="55f7c-180">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="55f7c-181">delta</span><span class="sxs-lookup"><span data-stu-id="55f7c-181">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="55f7c-182">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55f7c-182">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="55f7c-183">获取用户邮箱中已添加、删除或移除的邮件文件夹集。</span><span class="sxs-lookup"><span data-stu-id="55f7c-183">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="55f7c-184">移动</span><span class="sxs-lookup"><span data-stu-id="55f7c-184">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="55f7c-185">mailFolder</span><span class="sxs-lookup"><span data-stu-id="55f7c-185">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="55f7c-186">将 mailFolder 及其内容移动到其他 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="55f7c-186">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="55f7c-187">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="55f7c-187">**Extended properties**</span></span>| | |
|[<span data-ttu-id="55f7c-188">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="55f7c-188">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="55f7c-189">mailFolder</span><span class="sxs-lookup"><span data-stu-id="55f7c-189">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="55f7c-190">在新建或现有的 mailFolder 中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="55f7c-190">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="55f7c-191">获取具有单值扩展属性的 mailFolder</span><span class="sxs-lookup"><span data-stu-id="55f7c-191">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="55f7c-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="55f7c-192">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="55f7c-193">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="55f7c-193">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="55f7c-194">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="55f7c-194">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="55f7c-195">mailFolder</span><span class="sxs-lookup"><span data-stu-id="55f7c-195">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="55f7c-196">在新建或现有的 mailFolder 中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="55f7c-196">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="55f7c-197">获取具有多值扩展属性的 mailFolder</span><span class="sxs-lookup"><span data-stu-id="55f7c-197">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="55f7c-198">mailFolder</span><span class="sxs-lookup"><span data-stu-id="55f7c-198">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="55f7c-199">使用 `$expand` 获取包含一个多值扩展属性的 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="55f7c-199">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="55f7c-200">属性</span><span class="sxs-lookup"><span data-stu-id="55f7c-200">Properties</span></span>

| <span data-ttu-id="55f7c-201">属性</span><span class="sxs-lookup"><span data-stu-id="55f7c-201">Property</span></span> | <span data-ttu-id="55f7c-202">类型</span><span class="sxs-lookup"><span data-stu-id="55f7c-202">Type</span></span> | <span data-ttu-id="55f7c-203">说明</span><span class="sxs-lookup"><span data-stu-id="55f7c-203">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="55f7c-204">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="55f7c-204">childFolderCount</span></span>|<span data-ttu-id="55f7c-205">Int32</span><span class="sxs-lookup"><span data-stu-id="55f7c-205">Int32</span></span>|<span data-ttu-id="55f7c-206">当前 mailFolder 中的直接子 mailFolder 数量。</span><span class="sxs-lookup"><span data-stu-id="55f7c-206">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="55f7c-207">displayName</span><span class="sxs-lookup"><span data-stu-id="55f7c-207">displayName</span></span>|<span data-ttu-id="55f7c-208">String</span><span class="sxs-lookup"><span data-stu-id="55f7c-208">String</span></span>|<span data-ttu-id="55f7c-209">mailFolder 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="55f7c-209">The mailFolder's display name.</span></span>|
|<span data-ttu-id="55f7c-210">id</span><span class="sxs-lookup"><span data-stu-id="55f7c-210">id</span></span>|<span data-ttu-id="55f7c-211">String</span><span class="sxs-lookup"><span data-stu-id="55f7c-211">String</span></span>|<span data-ttu-id="55f7c-212">MailFolder 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="55f7c-212">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="55f7c-213">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="55f7c-213">parentFolderId</span></span>|<span data-ttu-id="55f7c-214">String</span><span class="sxs-lookup"><span data-stu-id="55f7c-214">String</span></span>|<span data-ttu-id="55f7c-215">MailFolder 的父 mailFolder 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="55f7c-215">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="55f7c-216">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="55f7c-216">totalItemCount</span></span>|<span data-ttu-id="55f7c-217">Int32</span><span class="sxs-lookup"><span data-stu-id="55f7c-217">Int32</span></span>|<span data-ttu-id="55f7c-218">邮箱中项的数量</span><span class="sxs-lookup"><span data-stu-id="55f7c-218">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="55f7c-219">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="55f7c-219">unreadItemCount</span></span>|<span data-ttu-id="55f7c-220">Int32</span><span class="sxs-lookup"><span data-stu-id="55f7c-220">Int32</span></span>|<span data-ttu-id="55f7c-221">mailFolder 中标记为未读的项的数量。</span><span class="sxs-lookup"><span data-stu-id="55f7c-221">The number of items in the mailFolder marked as unread.</span></span>|
|<span data-ttu-id="55f7c-222">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="55f7c-222">wellKnownName</span></span>|<span data-ttu-id="55f7c-223">String</span><span class="sxs-lookup"><span data-stu-id="55f7c-223">String</span></span>|<span data-ttu-id="55f7c-224">文件夹的已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="55f7c-224">The well-known folder name for the folder.</span></span> <span data-ttu-id="55f7c-225">上面列出了可能的值。</span><span class="sxs-lookup"><span data-stu-id="55f7c-225">The possible values are listed above.</span></span> <span data-ttu-id="55f7c-226">此属性仅对于创建的 Outlook 默认文件夹设置。</span><span class="sxs-lookup"><span data-stu-id="55f7c-226">This property is only set for default folders created by Outlook.</span></span> <span data-ttu-id="55f7c-227">有关其他文件夹，此属性为**null**。</span><span class="sxs-lookup"><span data-stu-id="55f7c-227">For other folders, this property is **null**.</span></span>|

<span data-ttu-id="55f7c-228">**有效的访问项计数**</span><span class="sxs-lookup"><span data-stu-id="55f7c-228">**Access item counts efficiently**</span></span>

<span data-ttu-id="55f7c-229">`TotalItemCount`和`UnreadItemCount`文件夹的属性，可以方便地计算的文件夹中的读取项目数。</span><span class="sxs-lookup"><span data-stu-id="55f7c-229">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="55f7c-230">它们使您可以避免查询会引发大量延迟如下：</span><span class="sxs-lookup"><span data-stu-id="55f7c-230">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/beta/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="55f7c-231">在 Outlook 中的邮件文件夹可以包含多个类型的项目，例如，可以包含收件箱会议请求项目的不同邮件项目。</span><span class="sxs-lookup"><span data-stu-id="55f7c-231">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="55f7c-232">`TotalItemCount`和`UnreadItemCount`包括而不考虑其项目类型的邮件文件夹中的项目。</span><span class="sxs-lookup"><span data-stu-id="55f7c-232">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="55f7c-233">关系</span><span class="sxs-lookup"><span data-stu-id="55f7c-233">Relationships</span></span>

| <span data-ttu-id="55f7c-234">关系</span><span class="sxs-lookup"><span data-stu-id="55f7c-234">Relationship</span></span> | <span data-ttu-id="55f7c-235">类型</span><span class="sxs-lookup"><span data-stu-id="55f7c-235">Type</span></span> | <span data-ttu-id="55f7c-236">说明</span><span class="sxs-lookup"><span data-stu-id="55f7c-236">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="55f7c-237">childFolders</span><span class="sxs-lookup"><span data-stu-id="55f7c-237">childFolders</span></span>|<span data-ttu-id="55f7c-238">[MailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55f7c-238">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="55f7c-239">mailFolder 中的子文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="55f7c-239">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="55f7c-240">messageRules</span><span class="sxs-lookup"><span data-stu-id="55f7c-240">messageRules</span></span> | <span data-ttu-id="55f7c-241">[messageRule](messagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55f7c-241">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="55f7c-242">适用于用户“收件箱”文件夹的规则集合。</span><span class="sxs-lookup"><span data-stu-id="55f7c-242">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="55f7c-243">messages</span><span class="sxs-lookup"><span data-stu-id="55f7c-243">messages</span></span>|<span data-ttu-id="55f7c-244">[邮件](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55f7c-244">[Message](message.md) collection</span></span>|<span data-ttu-id="55f7c-245">mailFolder 中的邮件集合。</span><span class="sxs-lookup"><span data-stu-id="55f7c-245">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="55f7c-246">multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="55f7c-246">multiValueLegacyExtendedProperty</span></span>|<span data-ttu-id="55f7c-247">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55f7c-247">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="55f7c-p111">为 mailFolder 定义的多值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="55f7c-p111">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="55f7c-251">singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="55f7c-251">singleValueLegacyExtendedProperty</span></span>|<span data-ttu-id="55f7c-252">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="55f7c-252">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="55f7c-p112">为 mailFolder 定义的单值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="55f7c-p112">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55f7c-256">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55f7c-256">JSON representation</span></span>

<span data-ttu-id="55f7c-257">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55f7c-257">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueLegacyExtendedProperty",
    "singleValueLegacyExtendedProperty"
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
  "multiValueLegacyExtendedProperty": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueLegacyExtendedProperty": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a><span data-ttu-id="55f7c-258">另请参阅</span><span class="sxs-lookup"><span data-stu-id="55f7c-258">See also</span></span>

- [<span data-ttu-id="55f7c-259">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="55f7c-259">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="55f7c-260">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="55f7c-260">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
