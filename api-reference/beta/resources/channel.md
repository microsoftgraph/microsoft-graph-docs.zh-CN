---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8b055a8a76a888fc5fc2e3f213b8be69f34f6413
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024425"
---
# <a name="channel-resource-type"></a><span data-ttu-id="f7826-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="f7826-103">channel resource type</span></span>

<span data-ttu-id="f7826-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7826-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7826-105">[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。</span><span class="sxs-lookup"><span data-stu-id="f7826-105">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="f7826-106">每个频道专用于特定主题、部门或项目。</span><span class="sxs-lookup"><span data-stu-id="f7826-106">Each channel is dedicated to a specific topic, department, or project.</span></span> <span data-ttu-id="f7826-107">频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。</span><span class="sxs-lookup"><span data-stu-id="f7826-107">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="f7826-108">方法</span><span class="sxs-lookup"><span data-stu-id="f7826-108">Methods</span></span>

| <span data-ttu-id="f7826-109">方法</span><span class="sxs-lookup"><span data-stu-id="f7826-109">Method</span></span>       | <span data-ttu-id="f7826-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f7826-110">Return Type</span></span>  |<span data-ttu-id="f7826-111">说明</span><span class="sxs-lookup"><span data-stu-id="f7826-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f7826-112">列出频道</span><span class="sxs-lookup"><span data-stu-id="f7826-112">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="f7826-113">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="f7826-113">[channel](channel.md) collection</span></span> | <span data-ttu-id="f7826-114">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="f7826-114">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="f7826-115">创建频道</span><span class="sxs-lookup"><span data-stu-id="f7826-115">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="f7826-116">频道</span><span class="sxs-lookup"><span data-stu-id="f7826-116">channel</span></span>](channel.md) | <span data-ttu-id="f7826-117">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="f7826-117">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="f7826-118">获取频道</span><span class="sxs-lookup"><span data-stu-id="f7826-118">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="f7826-119">频道</span><span class="sxs-lookup"><span data-stu-id="f7826-119">channel</span></span>](channel.md) | <span data-ttu-id="f7826-120">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7826-120">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="f7826-121">更新频道</span><span class="sxs-lookup"><span data-stu-id="f7826-121">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="f7826-122">频道</span><span class="sxs-lookup"><span data-stu-id="f7826-122">channel</span></span>](channel.md) | <span data-ttu-id="f7826-123">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="f7826-123">Update properties of the channel.</span></span>|
|[<span data-ttu-id="f7826-124">删除频道</span><span class="sxs-lookup"><span data-stu-id="f7826-124">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="f7826-125">无</span><span class="sxs-lookup"><span data-stu-id="f7826-125">None</span></span> | <span data-ttu-id="f7826-126">删除通道。</span><span class="sxs-lookup"><span data-stu-id="f7826-126">Delete a channel.</span></span>|
|[<span data-ttu-id="f7826-127">获取消息 Delta</span><span class="sxs-lookup"><span data-stu-id="f7826-127">Get message delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="f7826-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f7826-128">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="f7826-129">获取频道中的增量消息。</span><span class="sxs-lookup"><span data-stu-id="f7826-129">Get incremental messages in a channel.</span></span> |
|[<span data-ttu-id="f7826-130">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="f7826-130">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="f7826-131">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f7826-131">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="f7826-132">获取频道中的消息</span><span class="sxs-lookup"><span data-stu-id="f7826-132">Get messages in a channel</span></span> |
|[<span data-ttu-id="f7826-133">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="f7826-133">List channel members</span></span>](../api/conversationmember-list.md)| <span data-ttu-id="f7826-134">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f7826-134">[conversationMember](conversationmember.md) collection</span></span>| <span data-ttu-id="f7826-135">列出频道的成员。</span><span class="sxs-lookup"><span data-stu-id="f7826-135">List the members of a channel.</span></span> |
|[<span data-ttu-id="f7826-136">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="f7826-136">Get channel member</span></span>](../api/conversationmember-get.md)| [<span data-ttu-id="f7826-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="f7826-137">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="f7826-138">获取频道的成员。</span><span class="sxs-lookup"><span data-stu-id="f7826-138">Get a member of a channel.</span></span> |
|[<span data-ttu-id="f7826-139">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="f7826-139">Add channel member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="f7826-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="f7826-140">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="f7826-141">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="f7826-141">Add a member to a channel.</span></span> <span data-ttu-id="f7826-142">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="f7826-142">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="f7826-143">更新频道成员</span><span class="sxs-lookup"><span data-stu-id="f7826-143">Update channel member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="f7826-144">conversationMember</span><span class="sxs-lookup"><span data-stu-id="f7826-144">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="f7826-145">更新聊天成员。</span><span class="sxs-lookup"><span data-stu-id="f7826-145">Update a member of a channel.</span></span> <span data-ttu-id="f7826-146">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="f7826-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="f7826-147">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="f7826-147">Delete channel member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="f7826-148">conversationMember</span><span class="sxs-lookup"><span data-stu-id="f7826-148">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="f7826-149">删除频道的成员。</span><span class="sxs-lookup"><span data-stu-id="f7826-149">Delete a member of a channel.</span></span> <span data-ttu-id="f7826-150">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="f7826-150">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="f7826-151">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="f7826-151">Create chatMessage in a channel</span></span>](../api/channel-post-message.md) | [<span data-ttu-id="f7826-152">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f7826-152">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="f7826-153">向频道发送消息。</span><span class="sxs-lookup"><span data-stu-id="f7826-153">Send a message to a channel.</span></span> |
|[<span data-ttu-id="f7826-154">在频道中创建 chatMessage 回复</span><span class="sxs-lookup"><span data-stu-id="f7826-154">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="f7826-155">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f7826-155">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="f7826-156">在频道中回复消息。</span><span class="sxs-lookup"><span data-stu-id="f7826-156">Reply to a message in a channel.</span></span>|
|[<span data-ttu-id="f7826-157">获取文件文件夹</span><span class="sxs-lookup"><span data-stu-id="f7826-157">Get files folder</span></span>](../api/driveitem-get.md)| [<span data-ttu-id="f7826-158">driveItem</span><span class="sxs-lookup"><span data-stu-id="f7826-158">driveItem</span></span>](driveitem.md) | <span data-ttu-id="f7826-159">检索用于存储频道文件的 SharePoint 文件夹的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f7826-159">Retrieves the details of the SharePoint folder where the files for the channel are stored.</span></span> |

## <a name="properties"></a><span data-ttu-id="f7826-160">属性</span><span class="sxs-lookup"><span data-stu-id="f7826-160">Properties</span></span>

| <span data-ttu-id="f7826-161">属性</span><span class="sxs-lookup"><span data-stu-id="f7826-161">Property</span></span>   | <span data-ttu-id="f7826-162">类型</span><span class="sxs-lookup"><span data-stu-id="f7826-162">Type</span></span> |<span data-ttu-id="f7826-163">说明</span><span class="sxs-lookup"><span data-stu-id="f7826-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7826-164">说明</span><span class="sxs-lookup"><span data-stu-id="f7826-164">description</span></span>|<span data-ttu-id="f7826-165">String</span><span class="sxs-lookup"><span data-stu-id="f7826-165">String</span></span>|<span data-ttu-id="f7826-166">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="f7826-166">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="f7826-167">displayName</span><span class="sxs-lookup"><span data-stu-id="f7826-167">displayName</span></span>|<span data-ttu-id="f7826-168">String</span><span class="sxs-lookup"><span data-stu-id="f7826-168">String</span></span>|<span data-ttu-id="f7826-169">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="f7826-169">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="f7826-170">id</span><span class="sxs-lookup"><span data-stu-id="f7826-170">id</span></span>|<span data-ttu-id="f7826-171">String</span><span class="sxs-lookup"><span data-stu-id="f7826-171">String</span></span>|<span data-ttu-id="f7826-172">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f7826-172">The channel's unique identifier.</span></span> <span data-ttu-id="f7826-173">只读。</span><span class="sxs-lookup"><span data-stu-id="f7826-173">Read-only.</span></span>|
|<span data-ttu-id="f7826-174">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="f7826-174">isFavoriteByDefault</span></span>|<span data-ttu-id="f7826-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7826-175">Boolean</span></span>|<span data-ttu-id="f7826-176">指示是否应对团队的所有成员将频道自动标记到“收藏夹”。</span><span class="sxs-lookup"><span data-stu-id="f7826-176">Indicates whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="f7826-177">仅可使用“[创建团队](../api/team-post.md)”以编程方式设置。</span><span class="sxs-lookup"><span data-stu-id="f7826-177">Can only be set programmatically with [Create team](../api/team-post.md).</span></span> <span data-ttu-id="f7826-178">默认值：`false`。</span><span class="sxs-lookup"><span data-stu-id="f7826-178">Default: `false`.</span></span>|
|<span data-ttu-id="f7826-179">email</span><span class="sxs-lookup"><span data-stu-id="f7826-179">email</span></span>|<span data-ttu-id="f7826-180">String</span><span class="sxs-lookup"><span data-stu-id="f7826-180">String</span></span>| <span data-ttu-id="f7826-181">用于向频道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="f7826-181">The email address for sending messages to the channel.</span></span> <span data-ttu-id="f7826-182">只读。</span><span class="sxs-lookup"><span data-stu-id="f7826-182">Read-only.</span></span>|
|<span data-ttu-id="f7826-183">webUrl</span><span class="sxs-lookup"><span data-stu-id="f7826-183">webUrl</span></span>|<span data-ttu-id="f7826-184">String</span><span class="sxs-lookup"><span data-stu-id="f7826-184">String</span></span>|<span data-ttu-id="f7826-185">将转到 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="f7826-185">A hyperlink that will go to the channel in Microsoft Teams.</span></span> <span data-ttu-id="f7826-186">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="f7826-186">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="f7826-187">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="f7826-187">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="f7826-188">只读。</span><span class="sxs-lookup"><span data-stu-id="f7826-188">Read-only.</span></span>|
|<span data-ttu-id="f7826-189">membershipType</span><span class="sxs-lookup"><span data-stu-id="f7826-189">membershipType</span></span>|[<span data-ttu-id="f7826-190">channelMembershipType</span><span class="sxs-lookup"><span data-stu-id="f7826-190">channelMembershipType</span></span>](../resources/enums.md#channelmembershiptype-values)|<span data-ttu-id="f7826-191">频道的类型。</span><span class="sxs-lookup"><span data-stu-id="f7826-191">The type of the channel.</span></span> <span data-ttu-id="f7826-192">可在创建期间设置，但不可更改。</span><span class="sxs-lookup"><span data-stu-id="f7826-192">Can be set during creation and cannot be changed.</span></span> <span data-ttu-id="f7826-193">默认：标准。</span><span class="sxs-lookup"><span data-stu-id="f7826-193">Default: standard.</span></span>|
|<span data-ttu-id="f7826-194">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7826-194">createdDateTime</span></span>|<span data-ttu-id="f7826-195">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7826-195">dateTimeOffset</span></span>|<span data-ttu-id="f7826-196">只读。</span><span class="sxs-lookup"><span data-stu-id="f7826-196">Read only.</span></span> <span data-ttu-id="f7826-197">创建频道的时间戳。</span><span class="sxs-lookup"><span data-stu-id="f7826-197">Timestamp at which the channel was created.</span></span>|

### <a name="instance-attributes"></a><span data-ttu-id="f7826-198">实例属性</span><span class="sxs-lookup"><span data-stu-id="f7826-198">Instance attributes</span></span>

<span data-ttu-id="f7826-p111">实例属性是具有特殊行为的属性。这些属性是临时的，并且 a) 定义服务应执行的行为或 b) 提供短期的属性值，例如过期项目的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f7826-p111">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="f7826-201">属性名称</span><span class="sxs-lookup"><span data-stu-id="f7826-201">Property name</span></span>| <span data-ttu-id="f7826-202">类型</span><span class="sxs-lookup"><span data-stu-id="f7826-202">Type</span></span>   | <span data-ttu-id="f7826-203">说明</span><span class="sxs-lookup"><span data-stu-id="f7826-203">Description</span></span>
|:-----------------------|:-------|:-------------------------|
|<span data-ttu-id="f7826-204">@microsoft. graph channelCreationMode</span><span class="sxs-lookup"><span data-stu-id="f7826-204">@microsoft.graph.channelCreationMode</span></span>|<span data-ttu-id="f7826-205">string</span><span class="sxs-lookup"><span data-stu-id="f7826-205">string</span></span>|<span data-ttu-id="f7826-206">指示频道处于迁移状态，并且当前正用于迁移目的。</span><span class="sxs-lookup"><span data-stu-id="f7826-206">Indicates that the channel is in migration state and is currently being used for migration purposes.</span></span> <span data-ttu-id="f7826-207">它接受一个值：`migration`。</span><span class="sxs-lookup"><span data-stu-id="f7826-207">It accepts one value: `migration`.</span></span>|

> <span data-ttu-id="f7826-208">**注意**：`ChannelCreationMode` 是采用值 `migration`的枚举。</span><span class="sxs-lookup"><span data-stu-id="f7826-208">**Note**: `ChannelCreationMode`  is an enum that takes the value `migration`.</span></span>

<span data-ttu-id="f7826-209">有关 POST 请求示例，请参阅[请求（在迁移状态下创建频道）](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams#request-create-a-team-in-migration-state)。</span><span class="sxs-lookup"><span data-stu-id="f7826-209">For a POST request example, see [Request (create channel in migration state)](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams#request-create-a-team-in-migration-state).</span></span>

## <a name="relationships"></a><span data-ttu-id="f7826-210">关系</span><span class="sxs-lookup"><span data-stu-id="f7826-210">Relationships</span></span>

| <span data-ttu-id="f7826-211">关系</span><span class="sxs-lookup"><span data-stu-id="f7826-211">Relationship</span></span> | <span data-ttu-id="f7826-212">类型</span><span class="sxs-lookup"><span data-stu-id="f7826-212">Type</span></span> |<span data-ttu-id="f7826-213">说明</span><span class="sxs-lookup"><span data-stu-id="f7826-213">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7826-214">messages</span><span class="sxs-lookup"><span data-stu-id="f7826-214">messages</span></span>|<span data-ttu-id="f7826-215">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f7826-215">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="f7826-216">频道中的所有消息集合。</span><span class="sxs-lookup"><span data-stu-id="f7826-216">A collection of all the messages in the channel.</span></span> <span data-ttu-id="f7826-217">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="f7826-217">A navigation property.</span></span> <span data-ttu-id="f7826-218">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="f7826-218">Nullable.</span></span>|
|<span data-ttu-id="f7826-219">选项卡</span><span class="sxs-lookup"><span data-stu-id="f7826-219">tabs</span></span>|<span data-ttu-id="f7826-220">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f7826-220">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="f7826-221">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="f7826-221">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="f7826-222">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="f7826-222">A navigation property.</span></span>|
|<span data-ttu-id="f7826-223">成员</span><span class="sxs-lookup"><span data-stu-id="f7826-223">members</span></span>|<span data-ttu-id="f7826-224">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f7826-224">[conversationMember](conversationmember.md) collection</span></span>|<span data-ttu-id="f7826-225">与频道关联的成员资格记录的集合。</span><span class="sxs-lookup"><span data-stu-id="f7826-225">A collection of membership records associated with the channel.</span></span>|
|[<span data-ttu-id="f7826-226">filesFolder</span><span class="sxs-lookup"><span data-stu-id="f7826-226">filesFolder</span></span>](../api/channel-get-filesfolder.md)|[<span data-ttu-id="f7826-227">driveItem</span><span class="sxs-lookup"><span data-stu-id="f7826-227">driveItem</span></span>](driveitem.md)|<span data-ttu-id="f7826-228">用于存储频道文件的位置的元数据。</span><span class="sxs-lookup"><span data-stu-id="f7826-228">Metadata for the location where the channel's files are stored.</span></span>|
|<span data-ttu-id="f7826-229">operations</span><span class="sxs-lookup"><span data-stu-id="f7826-229">operations</span></span>|<span data-ttu-id="f7826-230">[teamsAsyncOperation](teamsasyncoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f7826-230">[teamsAsyncOperation](teamsasyncoperation.md) collection</span></span>| <span data-ttu-id="f7826-231">在此团队中运行过或正在运行的异步操作。</span><span class="sxs-lookup"><span data-stu-id="f7826-231">The async operations that ran or are running on this team.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f7826-232">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7826-232">JSON representation</span></span>

<span data-ttu-id="f7826-233">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7826-233">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messages"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "isFavoriteByDefault": true,
  "email": "string",
  "webUrl": "string",
  "membershipType": "channelMembershipType",
  "createdDateTime": "string (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


