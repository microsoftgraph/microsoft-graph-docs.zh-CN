---
title: aadUserConversationMember 资源类型
description: 表示聊天或频道中的 Azure Active Directory 用户。
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4cd7b6ac208c719663eb04adf91a98ae6fa7da39
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714338"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="48544-103">aadUserConversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="48544-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="48544-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48544-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48544-105">表示[团队](team.md)[频道](channel.md)或[聊天](chat.md)中的 Azure Active Directory 用户。</span><span class="sxs-lookup"><span data-stu-id="48544-105">Represents an Azure Active Directory user in a [team](team.md) or a [channel](channel.md) or a [chat](chat.md).</span></span> <span data-ttu-id="48544-106">此类型继承自 [conversationMember](conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="48544-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="48544-107">方法</span><span class="sxs-lookup"><span data-stu-id="48544-107">Methods</span></span>

| <span data-ttu-id="48544-108">方法</span><span class="sxs-lookup"><span data-stu-id="48544-108">Method</span></span>       | <span data-ttu-id="48544-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="48544-109">Return Type</span></span>  |<span data-ttu-id="48544-110">说明</span><span class="sxs-lookup"><span data-stu-id="48544-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48544-111">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="48544-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="48544-112">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="48544-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="48544-113">获取此团队中的成员列表。</span><span class="sxs-lookup"><span data-stu-id="48544-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="48544-114">添加团队成员</span><span class="sxs-lookup"><span data-stu-id="48544-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="48544-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="48544-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="48544-116">向团队中添加新成员。</span><span class="sxs-lookup"><span data-stu-id="48544-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="48544-117">批量添加团队成员。</span><span class="sxs-lookup"><span data-stu-id="48544-117">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="48544-118">[actionResultPart](../resources/actionresultpart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="48544-118">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="48544-119">在单个请求中将多个成员添加到团队中。</span><span class="sxs-lookup"><span data-stu-id="48544-119">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="48544-120">获取团队成员</span><span class="sxs-lookup"><span data-stu-id="48544-120">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="48544-121">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="48544-121">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="48544-122">获取团队中的成员。</span><span class="sxs-lookup"><span data-stu-id="48544-122">Get a member in the team.</span></span>|
|[<span data-ttu-id="48544-123">更新成员角色</span><span class="sxs-lookup"><span data-stu-id="48544-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="48544-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="48544-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="48544-125">将成员更改为所有者或返回为常规成员。</span><span class="sxs-lookup"><span data-stu-id="48544-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="48544-126">删除团队成员</span><span class="sxs-lookup"><span data-stu-id="48544-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="48544-127">无</span><span class="sxs-lookup"><span data-stu-id="48544-127">None</span></span>|<span data-ttu-id="48544-128">删除团队中的一个现有成员。</span><span class="sxs-lookup"><span data-stu-id="48544-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="48544-129">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="48544-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="48544-130">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="48544-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="48544-131">获取频道中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="48544-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="48544-132">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="48544-132">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="48544-133">conversationMember</span><span class="sxs-lookup"><span data-stu-id="48544-133">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="48544-134">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="48544-134">Add a member to a channel.</span></span> <span data-ttu-id="48544-135">仅支持 membershipType 为 `private` 的 `channel`。</span><span class="sxs-lookup"><span data-stu-id="48544-135">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="48544-136">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="48544-136">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="48544-137">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="48544-137">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="48544-138">获取频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="48544-138">Get a member in a channel.</span></span>|
|[<span data-ttu-id="48544-139">更新频道成员角色</span><span class="sxs-lookup"><span data-stu-id="48544-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="48544-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="48544-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="48544-141">更新频道成员的属性。</span><span class="sxs-lookup"><span data-stu-id="48544-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="48544-142">仅支持 membershipType 为 `private` 的频道。</span><span class="sxs-lookup"><span data-stu-id="48544-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="48544-143">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="48544-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="48544-144">无</span><span class="sxs-lookup"><span data-stu-id="48544-144">None</span></span> | <span data-ttu-id="48544-145">从频道中删除一个成员。</span><span class="sxs-lookup"><span data-stu-id="48544-145">Delete a member from a channel.</span></span> <span data-ttu-id="48544-146">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="48544-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="48544-147">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="48544-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="48544-148">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="48544-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="48544-149">获取聊天中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="48544-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="48544-150">添加聊天成员</span><span class="sxs-lookup"><span data-stu-id="48544-150">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="48544-151">位置标头</span><span class="sxs-lookup"><span data-stu-id="48544-151">Location header</span></span> | <span data-ttu-id="48544-152">向聊天添加成员。</span><span class="sxs-lookup"><span data-stu-id="48544-152">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="48544-153">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="48544-153">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="48544-154">conversationMember</span><span class="sxs-lookup"><span data-stu-id="48544-154">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="48544-155">获取聊天中的成员。</span><span class="sxs-lookup"><span data-stu-id="48544-155">Get a member in a chat.</span></span>|
|[<span data-ttu-id="48544-156">删除聊天成员</span><span class="sxs-lookup"><span data-stu-id="48544-156">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="48544-157">无</span><span class="sxs-lookup"><span data-stu-id="48544-157">None</span></span> | <span data-ttu-id="48544-158">从聊天中删除成员。</span><span class="sxs-lookup"><span data-stu-id="48544-158">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="48544-159">属性</span><span class="sxs-lookup"><span data-stu-id="48544-159">Properties</span></span>

| <span data-ttu-id="48544-160">属性</span><span class="sxs-lookup"><span data-stu-id="48544-160">Property</span></span>   | <span data-ttu-id="48544-161">类型</span><span class="sxs-lookup"><span data-stu-id="48544-161">Type</span></span> |<span data-ttu-id="48544-162">说明</span><span class="sxs-lookup"><span data-stu-id="48544-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48544-163">id</span><span class="sxs-lookup"><span data-stu-id="48544-163">id</span></span>| <span data-ttu-id="48544-164">String</span><span class="sxs-lookup"><span data-stu-id="48544-164">String</span></span> | <span data-ttu-id="48544-165">只读。</span><span class="sxs-lookup"><span data-stu-id="48544-165">Read-only.</span></span> <span data-ttu-id="48544-166">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="48544-166">Unique ID of the user.</span></span>|
|<span data-ttu-id="48544-167">displayName</span><span class="sxs-lookup"><span data-stu-id="48544-167">displayName</span></span>| <span data-ttu-id="48544-168">String</span><span class="sxs-lookup"><span data-stu-id="48544-168">String</span></span> | <span data-ttu-id="48544-169">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="48544-169">The display name of the user.</span></span> |
|<span data-ttu-id="48544-170">角色</span><span class="sxs-lookup"><span data-stu-id="48544-170">roles</span></span>| <span data-ttu-id="48544-171">String 集合</span><span class="sxs-lookup"><span data-stu-id="48544-171">String collection</span></span> | <span data-ttu-id="48544-172">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="48544-172">The roles for that user.</span></span> |
|<span data-ttu-id="48544-173">userId</span><span class="sxs-lookup"><span data-stu-id="48544-173">userId</span></span>| <span data-ttu-id="48544-174">String</span><span class="sxs-lookup"><span data-stu-id="48544-174">String</span></span> | <span data-ttu-id="48544-175">用户的 GUID。</span><span class="sxs-lookup"><span data-stu-id="48544-175">The GUID of the user.</span></span> |
|<span data-ttu-id="48544-176">email</span><span class="sxs-lookup"><span data-stu-id="48544-176">email</span></span>| <span data-ttu-id="48544-177">String</span><span class="sxs-lookup"><span data-stu-id="48544-177">String</span></span>  | <span data-ttu-id="48544-178">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="48544-178">The email address of the user.</span></span> |
|<span data-ttu-id="48544-179">tenantId</span><span class="sxs-lookup"><span data-stu-id="48544-179">tenantId</span></span>| <span data-ttu-id="48544-180">string</span><span class="sxs-lookup"><span data-stu-id="48544-180">string</span></span>  | <span data-ttu-id="48544-181">Azure AD 用户从属的 TenantId。</span><span class="sxs-lookup"><span data-stu-id="48544-181">TenantId which the Azure AD user belongs to.</span></span> |
|<span data-ttu-id="48544-182">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="48544-182">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="48544-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48544-183">DateTimeOffset</span></span>  | <span data-ttu-id="48544-184">表示对话历史久远程度的时间戳与对话成员共享。</span><span class="sxs-lookup"><span data-stu-id="48544-184">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="48544-185">此属性只对聊天成员可设置。</span><span class="sxs-lookup"><span data-stu-id="48544-185">This property is settable only for members of a chat.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48544-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48544-186">JSON representation</span></span>

<span data-ttu-id="48544-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48544-187">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.aadUserConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)",
  "userId": "String",
  "email": "String",
  "tenantId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "aadUserConversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
