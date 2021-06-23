---
title: aadUserConversationMember 资源类型
description: 表示聊天或频道中的 Azure Active Directory 用户。
localization_priority: Priority
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c7d65249e6e284efeaf0b34a4ffaf027026932d4
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060279"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="2fcef-103">aadUserConversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="2fcef-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="2fcef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fcef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fcef-105">表示[团队](team.md)[频道](channel.md)或[聊天](chat.md)中的 Azure Active Directory 用户。</span><span class="sxs-lookup"><span data-stu-id="2fcef-105">Represents an Azure Active Directory user in a [team](team.md) or a [channel](channel.md) or a [chat](chat.md).</span></span> <span data-ttu-id="2fcef-106">此类型继承自 [conversationMember](conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="2fcef-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2fcef-107">方法</span><span class="sxs-lookup"><span data-stu-id="2fcef-107">Methods</span></span>

| <span data-ttu-id="2fcef-108">方法</span><span class="sxs-lookup"><span data-stu-id="2fcef-108">Method</span></span>       | <span data-ttu-id="2fcef-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2fcef-109">Return Type</span></span>  |<span data-ttu-id="2fcef-110">说明</span><span class="sxs-lookup"><span data-stu-id="2fcef-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2fcef-111">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="2fcef-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="2fcef-112">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2fcef-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="2fcef-113">获取此团队中的成员列表。</span><span class="sxs-lookup"><span data-stu-id="2fcef-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="2fcef-114">添加团队成员</span><span class="sxs-lookup"><span data-stu-id="2fcef-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="2fcef-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="2fcef-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="2fcef-116">向团队中添加新成员。</span><span class="sxs-lookup"><span data-stu-id="2fcef-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="2fcef-117">批量添加团队成员。</span><span class="sxs-lookup"><span data-stu-id="2fcef-117">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="2fcef-118">[actionResultPart](../resources/actionresultpart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2fcef-118">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="2fcef-119">在单个请求中将多个成员添加到团队中。</span><span class="sxs-lookup"><span data-stu-id="2fcef-119">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="2fcef-120">获取团队成员</span><span class="sxs-lookup"><span data-stu-id="2fcef-120">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="2fcef-121">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2fcef-121">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="2fcef-122">获取团队中的成员。</span><span class="sxs-lookup"><span data-stu-id="2fcef-122">Get a member in the team.</span></span>|
|[<span data-ttu-id="2fcef-123">更新成员角色</span><span class="sxs-lookup"><span data-stu-id="2fcef-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="2fcef-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="2fcef-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="2fcef-125">将成员更改为所有者或返回为常规成员。</span><span class="sxs-lookup"><span data-stu-id="2fcef-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="2fcef-126">删除团队成员</span><span class="sxs-lookup"><span data-stu-id="2fcef-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="2fcef-127">无</span><span class="sxs-lookup"><span data-stu-id="2fcef-127">None</span></span>|<span data-ttu-id="2fcef-128">删除团队中的一个现有成员。</span><span class="sxs-lookup"><span data-stu-id="2fcef-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="2fcef-129">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="2fcef-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="2fcef-130">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2fcef-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="2fcef-131">获取频道中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="2fcef-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="2fcef-132">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="2fcef-132">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="2fcef-133">conversationMember</span><span class="sxs-lookup"><span data-stu-id="2fcef-133">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="2fcef-134">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="2fcef-134">Add a member to a channel.</span></span> <span data-ttu-id="2fcef-135">仅支持 membershipType 为 `private` 的 `channel`。</span><span class="sxs-lookup"><span data-stu-id="2fcef-135">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="2fcef-136">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="2fcef-136">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="2fcef-137">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2fcef-137">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="2fcef-138">获取频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="2fcef-138">Get a member in a channel.</span></span>|
|[<span data-ttu-id="2fcef-139">更新频道成员角色</span><span class="sxs-lookup"><span data-stu-id="2fcef-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="2fcef-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="2fcef-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="2fcef-141">更新频道成员的属性。</span><span class="sxs-lookup"><span data-stu-id="2fcef-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="2fcef-142">仅支持 membershipType 为 `private` 的频道。</span><span class="sxs-lookup"><span data-stu-id="2fcef-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="2fcef-143">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="2fcef-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="2fcef-144">无</span><span class="sxs-lookup"><span data-stu-id="2fcef-144">None</span></span> | <span data-ttu-id="2fcef-145">从频道中删除一个成员。</span><span class="sxs-lookup"><span data-stu-id="2fcef-145">Delete a member from a channel.</span></span> <span data-ttu-id="2fcef-146">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="2fcef-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="2fcef-147">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="2fcef-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="2fcef-148">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2fcef-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="2fcef-149">获取聊天中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="2fcef-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="2fcef-150">添加聊天成员</span><span class="sxs-lookup"><span data-stu-id="2fcef-150">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="2fcef-151">位置标头</span><span class="sxs-lookup"><span data-stu-id="2fcef-151">Location header</span></span> | <span data-ttu-id="2fcef-152">向聊天添加成员。</span><span class="sxs-lookup"><span data-stu-id="2fcef-152">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="2fcef-153">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="2fcef-153">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="2fcef-154">conversationMember</span><span class="sxs-lookup"><span data-stu-id="2fcef-154">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="2fcef-155">获取聊天中的成员。</span><span class="sxs-lookup"><span data-stu-id="2fcef-155">Get a member in a chat.</span></span>|
|[<span data-ttu-id="2fcef-156">删除聊天成员</span><span class="sxs-lookup"><span data-stu-id="2fcef-156">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="2fcef-157">无</span><span class="sxs-lookup"><span data-stu-id="2fcef-157">None</span></span> | <span data-ttu-id="2fcef-158">从聊天中删除成员。</span><span class="sxs-lookup"><span data-stu-id="2fcef-158">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="2fcef-159">属性</span><span class="sxs-lookup"><span data-stu-id="2fcef-159">Properties</span></span>

| <span data-ttu-id="2fcef-160">属性</span><span class="sxs-lookup"><span data-stu-id="2fcef-160">Property</span></span>   | <span data-ttu-id="2fcef-161">类型</span><span class="sxs-lookup"><span data-stu-id="2fcef-161">Type</span></span> |<span data-ttu-id="2fcef-162">说明</span><span class="sxs-lookup"><span data-stu-id="2fcef-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fcef-163">id</span><span class="sxs-lookup"><span data-stu-id="2fcef-163">id</span></span>| <span data-ttu-id="2fcef-164">String</span><span class="sxs-lookup"><span data-stu-id="2fcef-164">String</span></span> | <span data-ttu-id="2fcef-p105">只读。用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2fcef-p105">Read-only. Unique ID of the user.</span></span>|
|<span data-ttu-id="2fcef-167">displayName</span><span class="sxs-lookup"><span data-stu-id="2fcef-167">displayName</span></span>| <span data-ttu-id="2fcef-168">String</span><span class="sxs-lookup"><span data-stu-id="2fcef-168">String</span></span> | <span data-ttu-id="2fcef-169">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2fcef-169">The display name of the user.</span></span> |
|<span data-ttu-id="2fcef-170">角色</span><span class="sxs-lookup"><span data-stu-id="2fcef-170">roles</span></span>| <span data-ttu-id="2fcef-171">String 集合</span><span class="sxs-lookup"><span data-stu-id="2fcef-171">String collection</span></span> | <span data-ttu-id="2fcef-172">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="2fcef-172">The roles for that user.</span></span> |
|<span data-ttu-id="2fcef-173">userId</span><span class="sxs-lookup"><span data-stu-id="2fcef-173">userId</span></span>| <span data-ttu-id="2fcef-174">String</span><span class="sxs-lookup"><span data-stu-id="2fcef-174">String</span></span> | <span data-ttu-id="2fcef-175">用户的 GUID。</span><span class="sxs-lookup"><span data-stu-id="2fcef-175">The GUID of the user.</span></span> |
|<span data-ttu-id="2fcef-176">email</span><span class="sxs-lookup"><span data-stu-id="2fcef-176">email</span></span>| <span data-ttu-id="2fcef-177">String</span><span class="sxs-lookup"><span data-stu-id="2fcef-177">String</span></span>  | <span data-ttu-id="2fcef-178">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="2fcef-178">The email address of the user.</span></span> |
|<span data-ttu-id="2fcef-179">tenantId</span><span class="sxs-lookup"><span data-stu-id="2fcef-179">tenantId</span></span>| <span data-ttu-id="2fcef-180">string</span><span class="sxs-lookup"><span data-stu-id="2fcef-180">string</span></span>  | <span data-ttu-id="2fcef-181">Azure AD 用户从属的 TenantId。</span><span class="sxs-lookup"><span data-stu-id="2fcef-181">TenantId which the Azure AD user belongs to.</span></span> |
|<span data-ttu-id="2fcef-182">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="2fcef-182">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="2fcef-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fcef-183">DateTimeOffset</span></span>  | <span data-ttu-id="2fcef-184">表示对话历史久远程度的时间戳与对话成员共享。</span><span class="sxs-lookup"><span data-stu-id="2fcef-184">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="2fcef-185">此属性只对聊天成员可设置。</span><span class="sxs-lookup"><span data-stu-id="2fcef-185">This property is settable only for members of a chat.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2fcef-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2fcef-186">JSON representation</span></span>

<span data-ttu-id="2fcef-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2fcef-187">The following is a JSON representation of the resource.</span></span>

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
