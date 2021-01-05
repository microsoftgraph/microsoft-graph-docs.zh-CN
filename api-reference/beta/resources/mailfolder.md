---
title: mailFolder 资源类型
description: 用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。 邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7f05f70ae9faa6bab0ec0e7d122e4b1c443a8f5c
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753905"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="003f4-104">mailFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="003f4-104">mailFolder resource type</span></span>

<span data-ttu-id="003f4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="003f4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="003f4-106">用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。</span><span class="sxs-lookup"><span data-stu-id="003f4-106">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="003f4-107">邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-107">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="003f4-108">该资源支持通过提供 [delta](../api/mailfolder-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="003f4-108">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="003f4-109">**已知文件夹名称**</span><span class="sxs-lookup"><span data-stu-id="003f4-109">**Well-known folder names**</span></span>

<span data-ttu-id="003f4-110">Outlook 默认情况下会为用户创建某些文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-110">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="003f4-111">为方便起见，可以在访问这些文件夹时使用已知的文件夹名称来替代使用相应的文件夹 **id** 值。</span><span class="sxs-lookup"><span data-stu-id="003f4-111">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="003f4-112">例如，你可以使用其已知名称和以下查询来获取“草稿”文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-112">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="003f4-113">无论用户邮箱的区域设置如何，已知名称都可以工作，因此无论命名方式如何，上述查询都将始终返回用户的“草稿”文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-113">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="003f4-114">已知文件夹名称</span><span class="sxs-lookup"><span data-stu-id="003f4-114">Well-known folder name</span></span> | <span data-ttu-id="003f4-115">说明</span><span class="sxs-lookup"><span data-stu-id="003f4-115">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="003f4-116">archive</span><span class="sxs-lookup"><span data-stu-id="003f4-116">archive</span></span> | <span data-ttu-id="003f4-117">在支持它的 Outlook 客户端中使用 One_Click 存档功能时，将发送存档文件夹邮件。</span><span class="sxs-lookup"><span data-stu-id="003f4-117">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="003f4-118">**注意：** 这与 Exchange Online 的存档邮箱功能并不相同。</span><span class="sxs-lookup"><span data-stu-id="003f4-118">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="003f4-119">clutter</span><span class="sxs-lookup"><span data-stu-id="003f4-119">clutter</span></span> | <span data-ttu-id="003f4-120">使用待筛选邮件功能时，待筛选文件夹低优先级邮件将被移动到这里。</span><span class="sxs-lookup"><span data-stu-id="003f4-120">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="003f4-121">conflicts</span><span class="sxs-lookup"><span data-stu-id="003f4-121">conflicts</span></span> | <span data-ttu-id="003f4-122">包含邮箱中冲突项的文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-122">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="003f4-123">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="003f4-123">conversationhistory</span></span> | <span data-ttu-id="003f4-124">Skype 保存 IM 对话的文件夹（如果 Skype 配置为这样做）。</span><span class="sxs-lookup"><span data-stu-id="003f4-124">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="003f4-125">deleteditems</span><span class="sxs-lookup"><span data-stu-id="003f4-125">deleteditems</span></span> | <span data-ttu-id="003f4-126">文件夹项被删除时，将被移动到这里。</span><span class="sxs-lookup"><span data-stu-id="003f4-126">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="003f4-127">drafts</span><span class="sxs-lookup"><span data-stu-id="003f4-127">drafts</span></span> | <span data-ttu-id="003f4-128">包含未发送邮件的文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-128">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="003f4-129">inbox</span><span class="sxs-lookup"><span data-stu-id="003f4-129">inbox</span></span> | <span data-ttu-id="003f4-130">收件箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-130">The inbox folder.</span></span> |
| <span data-ttu-id="003f4-131">junkemail</span><span class="sxs-lookup"><span data-stu-id="003f4-131">junkemail</span></span> | <span data-ttu-id="003f4-132">“垃圾邮件”文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-132">The junk email folder.</span></span> |
| <span data-ttu-id="003f4-133">localfailures</span><span class="sxs-lookup"><span data-stu-id="003f4-133">localfailures</span></span> | <span data-ttu-id="003f4-134">包含本地客户端上存在但无法上载到服务器的项的文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-134">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="003f4-135">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="003f4-135">msgfolderroot</span></span> | <span data-ttu-id="003f4-136">“最上层的信息文件”文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-136">The "Top of Information Store" folder.</span></span> <span data-ttu-id="003f4-137">此文件夹是在普通邮件客户端（如收件箱）中显示的文件夹的父文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-137">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="003f4-138">outbox</span><span class="sxs-lookup"><span data-stu-id="003f4-138">outbox</span></span> | <span data-ttu-id="003f4-139">“发件箱”文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-139">The outbox folder.</span></span> |
| <span data-ttu-id="003f4-140">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="003f4-140">recoverableitemsdeletions</span></span> | <span data-ttu-id="003f4-141">包含软删除项的文件夹：从“已删除邮件”文件夹中删除，或者在 Outlook 中按 shift+delete 删除。</span><span class="sxs-lookup"><span data-stu-id="003f4-141">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="003f4-142">此文件夹在任何 Outlook 电子邮件客户端中都不可见，但最终用户可以通过 Outlook 中的“**从服务器恢复已删除邮件**”功能或 Web 上的 Outlook 与其进行交互。</span><span class="sxs-lookup"><span data-stu-id="003f4-142">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="003f4-143">scheduled</span><span class="sxs-lookup"><span data-stu-id="003f4-143">scheduled</span></span> | <span data-ttu-id="003f4-144">包含计划使用 Outlook for iOS 中的“计划”功能重新出现在收件箱中的邮件的文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-144">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="003f4-145">searchfolders</span><span class="sxs-lookup"><span data-stu-id="003f4-145">searchfolders</span></span> | <span data-ttu-id="003f4-146">用户邮箱中定义的所有搜索文件夹的父文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-146">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="003f4-147">sentitems</span><span class="sxs-lookup"><span data-stu-id="003f4-147">sentitems</span></span> | <span data-ttu-id="003f4-148">已发送项的文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-148">The sent items folder.</span></span> |
| <span data-ttu-id="003f4-149">serverfailures</span><span class="sxs-lookup"><span data-stu-id="003f4-149">serverfailures</span></span> | <span data-ttu-id="003f4-150">包含服务器上存在但无法同步到本地客户端的项的文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-150">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="003f4-151">syncissues</span><span class="sxs-lookup"><span data-stu-id="003f4-151">syncissues</span></span> | <span data-ttu-id="003f4-152">包含 Outlook 创建的同步日志的文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-152">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="003f4-153">方法</span><span class="sxs-lookup"><span data-stu-id="003f4-153">Methods</span></span>

| <span data-ttu-id="003f4-154">方法</span><span class="sxs-lookup"><span data-stu-id="003f4-154">Method</span></span> | <span data-ttu-id="003f4-155">返回类型</span><span class="sxs-lookup"><span data-stu-id="003f4-155">Return Type</span></span> | <span data-ttu-id="003f4-156">说明</span><span class="sxs-lookup"><span data-stu-id="003f4-156">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="003f4-157">获取 mailFolder</span><span class="sxs-lookup"><span data-stu-id="003f4-157">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="003f4-158">mailFolder</span><span class="sxs-lookup"><span data-stu-id="003f4-158">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="003f4-159">读取 mailFolder 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="003f4-159">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="003f4-160">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="003f4-160">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="003f4-161">mailFolder</span><span class="sxs-lookup"><span data-stu-id="003f4-161">mailFolder</span></span>](mailfolder.md)| <span data-ttu-id="003f4-162">通过发布到 childFolder 集合，在当前 mailFolder 下新建 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="003f4-162">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="003f4-163">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="003f4-163">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="003f4-164">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="003f4-164">[mailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="003f4-p107">获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="003f4-167">创建邮件</span><span class="sxs-lookup"><span data-stu-id="003f4-167">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="003f4-168">邮件</span><span class="sxs-lookup"><span data-stu-id="003f4-168">message</span></span>](message.md)| <span data-ttu-id="003f4-169">通过发布到邮件集合，在当前 mailFolder 中新建邮件。</span><span class="sxs-lookup"><span data-stu-id="003f4-169">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="003f4-170">列出邮件</span><span class="sxs-lookup"><span data-stu-id="003f4-170">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="003f4-171">[message](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="003f4-171">[message](message.md) collection</span></span>| <span data-ttu-id="003f4-172">获取已登录用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。</span><span class="sxs-lookup"><span data-stu-id="003f4-172">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="003f4-173">更新</span><span class="sxs-lookup"><span data-stu-id="003f4-173">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="003f4-174">mailFolder</span><span class="sxs-lookup"><span data-stu-id="003f4-174">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="003f4-175">更新指定的 mailFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="003f4-175">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="003f4-176">删除</span><span class="sxs-lookup"><span data-stu-id="003f4-176">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="003f4-177">无</span><span class="sxs-lookup"><span data-stu-id="003f4-177">None</span></span> |<span data-ttu-id="003f4-178">删除指定的 mailFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="003f4-178">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="003f4-179">复制</span><span class="sxs-lookup"><span data-stu-id="003f4-179">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="003f4-180">mailFolder</span><span class="sxs-lookup"><span data-stu-id="003f4-180">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="003f4-181">将 mailfolder 及其内容复制到其他 mailfolder。</span><span class="sxs-lookup"><span data-stu-id="003f4-181">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="003f4-182">delta</span><span class="sxs-lookup"><span data-stu-id="003f4-182">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="003f4-183">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="003f4-183">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="003f4-184">获取用户邮箱中已添加、删除或移除的邮件文件夹集。</span><span class="sxs-lookup"><span data-stu-id="003f4-184">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="003f4-185">移动</span><span class="sxs-lookup"><span data-stu-id="003f4-185">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="003f4-186">mailFolder</span><span class="sxs-lookup"><span data-stu-id="003f4-186">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="003f4-187">将 mailFolder 及其内容移动到其他 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="003f4-187">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="003f4-188">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="003f4-188">**Extended properties**</span></span>| | |
|[<span data-ttu-id="003f4-189">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="003f4-189">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="003f4-190">mailFolder</span><span class="sxs-lookup"><span data-stu-id="003f4-190">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="003f4-191">在新建或现有的 mailFolder 中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="003f4-191">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="003f4-192">获取具有单值扩展属性的 mailFolder</span><span class="sxs-lookup"><span data-stu-id="003f4-192">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="003f4-193">mailFolder</span><span class="sxs-lookup"><span data-stu-id="003f4-193">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="003f4-194">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="003f4-194">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="003f4-195">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="003f4-195">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="003f4-196">mailFolder</span><span class="sxs-lookup"><span data-stu-id="003f4-196">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="003f4-197">在新建或现有的 mailFolder 中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="003f4-197">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="003f4-198">获取具有多值扩展属性的 mailFolder</span><span class="sxs-lookup"><span data-stu-id="003f4-198">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="003f4-199">mailFolder</span><span class="sxs-lookup"><span data-stu-id="003f4-199">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="003f4-200">使用 `$expand` 获取包含一个多值扩展属性的 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="003f4-200">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="003f4-201">属性</span><span class="sxs-lookup"><span data-stu-id="003f4-201">Properties</span></span>

| <span data-ttu-id="003f4-202">属性</span><span class="sxs-lookup"><span data-stu-id="003f4-202">Property</span></span> | <span data-ttu-id="003f4-203">类型</span><span class="sxs-lookup"><span data-stu-id="003f4-203">Type</span></span> | <span data-ttu-id="003f4-204">说明</span><span class="sxs-lookup"><span data-stu-id="003f4-204">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="003f4-205">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="003f4-205">childFolderCount</span></span>|<span data-ttu-id="003f4-206">Int32</span><span class="sxs-lookup"><span data-stu-id="003f4-206">Int32</span></span>|<span data-ttu-id="003f4-207">当前 mailFolder 中的直接子 mailFolder 数量。</span><span class="sxs-lookup"><span data-stu-id="003f4-207">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="003f4-208">displayName</span><span class="sxs-lookup"><span data-stu-id="003f4-208">displayName</span></span>|<span data-ttu-id="003f4-209">String</span><span class="sxs-lookup"><span data-stu-id="003f4-209">String</span></span>|<span data-ttu-id="003f4-210">mailFolder 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="003f4-210">The mailFolder's display name.</span></span>|
|<span data-ttu-id="003f4-211">id</span><span class="sxs-lookup"><span data-stu-id="003f4-211">id</span></span>|<span data-ttu-id="003f4-212">String</span><span class="sxs-lookup"><span data-stu-id="003f4-212">String</span></span>|<span data-ttu-id="003f4-213">MailFolder 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="003f4-213">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="003f4-214">isHidden</span><span class="sxs-lookup"><span data-stu-id="003f4-214">isHidden</span></span>|<span data-ttu-id="003f4-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="003f4-215">Boolean</span></span>|<span data-ttu-id="003f4-216">指示 mailFolder 是否隐藏。</span><span class="sxs-lookup"><span data-stu-id="003f4-216">Indicates whether the mailFolder is hidden.</span></span> <span data-ttu-id="003f4-217">此属性只能在创建文件夹时设置。</span><span class="sxs-lookup"><span data-stu-id="003f4-217">This property can be set only when creating the folder.</span></span> <span data-ttu-id="003f4-218">在"隐藏"邮件 [文件夹中查找更多信息](#hidden-mail-folders)。</span><span class="sxs-lookup"><span data-stu-id="003f4-218">Find more information in [Hidden mail folders](#hidden-mail-folders).</span></span>|
|<span data-ttu-id="003f4-219">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="003f4-219">parentFolderId</span></span>|<span data-ttu-id="003f4-220">String</span><span class="sxs-lookup"><span data-stu-id="003f4-220">String</span></span>|<span data-ttu-id="003f4-221">MailFolder 的父 mailFolder 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="003f4-221">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="003f4-222">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="003f4-222">totalItemCount</span></span>|<span data-ttu-id="003f4-223">Int32</span><span class="sxs-lookup"><span data-stu-id="003f4-223">Int32</span></span>|<span data-ttu-id="003f4-224">邮箱中项的数量</span><span class="sxs-lookup"><span data-stu-id="003f4-224">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="003f4-225">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="003f4-225">unreadItemCount</span></span>|<span data-ttu-id="003f4-226">Int32</span><span class="sxs-lookup"><span data-stu-id="003f4-226">Int32</span></span>|<span data-ttu-id="003f4-227">mailFolder 中标记为未读的项的数量。</span><span class="sxs-lookup"><span data-stu-id="003f4-227">The number of items in the mailFolder marked as unread.</span></span>|
|<span data-ttu-id="003f4-228">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="003f4-228">wellKnownName</span></span>|<span data-ttu-id="003f4-229">String</span><span class="sxs-lookup"><span data-stu-id="003f4-229">String</span></span>|<span data-ttu-id="003f4-230">文件夹的已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="003f4-230">The well-known folder name for the folder.</span></span> <span data-ttu-id="003f4-231">以上列出了可能的值。</span><span class="sxs-lookup"><span data-stu-id="003f4-231">The possible values are listed above.</span></span> <span data-ttu-id="003f4-232">此属性仅为 Outlook 创建的默认文件夹设置。</span><span class="sxs-lookup"><span data-stu-id="003f4-232">This property is only set for default folders created by Outlook.</span></span> <span data-ttu-id="003f4-233">对于其他文件夹，此属性为 **null。**</span><span class="sxs-lookup"><span data-stu-id="003f4-233">For other folders, this property is **null**.</span></span>|

<span data-ttu-id="003f4-234">**有效的访问项计数**</span><span class="sxs-lookup"><span data-stu-id="003f4-234">**Access item counts efficiently**</span></span>

<span data-ttu-id="003f4-235">使用文件夹的 `TotalItemCount` 和 `UnreadItemCount` 的属性可以方便地计算在文件夹中读取的项数。</span><span class="sxs-lookup"><span data-stu-id="003f4-235">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="003f4-236">使你避免进行可产生重大延迟的查询，如下所示：</span><span class="sxs-lookup"><span data-stu-id="003f4-236">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/beta/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="003f4-237">Outlook 中的邮件文件夹可包含多个类型的项，例如，收件箱可以包含不同于邮件项的会议请求项。</span><span class="sxs-lookup"><span data-stu-id="003f4-237">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="003f4-238">`TotalItemCount` 和 `UnreadItemCount`包括邮件文件夹中的项，无论其项类型如何。</span><span class="sxs-lookup"><span data-stu-id="003f4-238">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

### <a name="hidden-mail-folders"></a><span data-ttu-id="003f4-239">隐藏的邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="003f4-239">Hidden mail folders</span></span>
<span data-ttu-id="003f4-240">该属性的 `isHidden` 默认值为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="003f4-240">The default value of the `isHidden` property is `false`.</span></span> <span data-ttu-id="003f4-241">创建 [mailFolder](../api/user-post-mailfolders.md)时，只能设置 **isHidden** 一次。</span><span class="sxs-lookup"><span data-stu-id="003f4-241">You can set **isHidden** only once when [creating the mailFolder](../api/user-post-mailfolders.md).</span></span> <span data-ttu-id="003f4-242">不能使用 PATCH 操作更新属性。</span><span class="sxs-lookup"><span data-stu-id="003f4-242">You cannot update the property using a PATCH operation.</span></span> <span data-ttu-id="003f4-243">若要更改 **文件夹的 isHidden** 属性，请删除现有文件夹并创建具有所需值的新文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-243">To change the **isHidden** property of a folder, delete the existing folder and create a new one with the desired value.</span></span>

<span data-ttu-id="003f4-244">隐藏的邮件文件夹支持常规邮件文件夹支持的所有操作。</span><span class="sxs-lookup"><span data-stu-id="003f4-244">Hidden mail folders support all operations that are supported by a regular mail folder.</span></span>

<span data-ttu-id="003f4-245">默认情况下， [列出 mailFolders](../api/user-list-mailfolders.md) 仅返回未隐藏的邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="003f4-245">By default, [listing mailFolders](../api/user-list-mailfolders.md) returns only mail folders that are not hidden.</span></span> <span data-ttu-id="003f4-246">若要在响应中包括隐藏的邮件文件夹，请使用查询参数 `includeHiddenFolders=true` 。</span><span class="sxs-lookup"><span data-stu-id="003f4-246">To include hidden mail folders in the response, use the query parameter `includeHiddenFolders=true`.</span></span> <span data-ttu-id="003f4-247">然后使用 **isHidden** 属性标识邮件文件夹是否隐藏。</span><span class="sxs-lookup"><span data-stu-id="003f4-247">Then use the **isHidden** property to identify whether a mail folder is hidden.</span></span> 

## <a name="relationships"></a><span data-ttu-id="003f4-248">关系</span><span class="sxs-lookup"><span data-stu-id="003f4-248">Relationships</span></span>

| <span data-ttu-id="003f4-249">关系</span><span class="sxs-lookup"><span data-stu-id="003f4-249">Relationship</span></span> | <span data-ttu-id="003f4-250">类型</span><span class="sxs-lookup"><span data-stu-id="003f4-250">Type</span></span> | <span data-ttu-id="003f4-251">说明</span><span class="sxs-lookup"><span data-stu-id="003f4-251">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="003f4-252">childFolders</span><span class="sxs-lookup"><span data-stu-id="003f4-252">childFolders</span></span>|<span data-ttu-id="003f4-253">[MailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="003f4-253">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="003f4-254">mailFolder 中的子文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="003f4-254">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="003f4-255">messageRules</span><span class="sxs-lookup"><span data-stu-id="003f4-255">messageRules</span></span> | <span data-ttu-id="003f4-256">[messageRule](messagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="003f4-256">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="003f4-257">适用于用户“收件箱”文件夹的规则集合。</span><span class="sxs-lookup"><span data-stu-id="003f4-257">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="003f4-258">messages</span><span class="sxs-lookup"><span data-stu-id="003f4-258">messages</span></span>|<span data-ttu-id="003f4-259">[邮件](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="003f4-259">[Message](message.md) collection</span></span>|<span data-ttu-id="003f4-260">mailFolder 中的邮件集合。</span><span class="sxs-lookup"><span data-stu-id="003f4-260">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="003f4-261">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="003f4-261">multiValueExtendedProperties</span></span>|<span data-ttu-id="003f4-262">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="003f4-262">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="003f4-p114">为 mailFolder 定义的多值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="003f4-p114">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="003f4-266">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="003f4-266">singleValueExtendedProperties</span></span>|<span data-ttu-id="003f4-267">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="003f4-267">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="003f4-p115">为 mailFolder 定义的单值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="003f4-p115">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="003f4-271">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="003f4-271">JSON representation</span></span>

<span data-ttu-id="003f4-272">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="003f4-272">The following is a JSON representation of the resource.</span></span>

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
  "isHidden": false,
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a><span data-ttu-id="003f4-273">另请参阅</span><span class="sxs-lookup"><span data-stu-id="003f4-273">See also</span></span>

- [<span data-ttu-id="003f4-274">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="003f4-274">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="003f4-275">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="003f4-275">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


