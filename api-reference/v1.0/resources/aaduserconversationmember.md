---
title: aadUserConversationMember 资源类型
description: 表示聊天或频道中的 Azure Active Directory 用户。
localization_priority: Priority
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6632dad56f76b4747285eb1df9f69046b1de3cc1
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060297"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="d78f0-103">aadUserConversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="d78f0-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="d78f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d78f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d78f0-105">表示[团队](team.md)、[频道](channel.md)或[聊天](chat.md)中的 Azure Active Directory 用户。</span><span class="sxs-lookup"><span data-stu-id="d78f0-105">Represents an Azure Active Directory user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="d78f0-106">此类型继承自 [conversationMember](conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="d78f0-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d78f0-107">方法</span><span class="sxs-lookup"><span data-stu-id="d78f0-107">Methods</span></span>

| <span data-ttu-id="d78f0-108">方法</span><span class="sxs-lookup"><span data-stu-id="d78f0-108">Method</span></span>       | <span data-ttu-id="d78f0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d78f0-109">Return Type</span></span>  |<span data-ttu-id="d78f0-110">说明</span><span class="sxs-lookup"><span data-stu-id="d78f0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d78f0-111">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="d78f0-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="d78f0-112">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78f0-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="d78f0-113">获取此团队中的成员列表。</span><span class="sxs-lookup"><span data-stu-id="d78f0-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="d78f0-114">添加团队成员</span><span class="sxs-lookup"><span data-stu-id="d78f0-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="d78f0-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d78f0-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="d78f0-116">向团队中添加新成员。</span><span class="sxs-lookup"><span data-stu-id="d78f0-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="d78f0-117">获取团队成员</span><span class="sxs-lookup"><span data-stu-id="d78f0-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="d78f0-118">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78f0-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="d78f0-119">获取团队中的成员。</span><span class="sxs-lookup"><span data-stu-id="d78f0-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="d78f0-120">更新成员角色</span><span class="sxs-lookup"><span data-stu-id="d78f0-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="d78f0-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d78f0-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="d78f0-122">将成员更改为所有者或返回为常规成员。</span><span class="sxs-lookup"><span data-stu-id="d78f0-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="d78f0-123">删除团队成员</span><span class="sxs-lookup"><span data-stu-id="d78f0-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="d78f0-124">无</span><span class="sxs-lookup"><span data-stu-id="d78f0-124">None</span></span>|<span data-ttu-id="d78f0-125">删除团队中的一个现有成员。</span><span class="sxs-lookup"><span data-stu-id="d78f0-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="d78f0-126">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="d78f0-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="d78f0-127">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78f0-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="d78f0-128">获取频道中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="d78f0-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="d78f0-129">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="d78f0-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="d78f0-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d78f0-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="d78f0-131">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="d78f0-131">Add a member to a channel.</span></span> <span data-ttu-id="d78f0-132">仅支持 membershipType 为 `private` 的 `channel`。</span><span class="sxs-lookup"><span data-stu-id="d78f0-132">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="d78f0-133">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="d78f0-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="d78f0-134">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78f0-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="d78f0-135">获取频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="d78f0-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="d78f0-136">更新频道成员角色</span><span class="sxs-lookup"><span data-stu-id="d78f0-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="d78f0-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d78f0-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="d78f0-138">更新频道成员的属性。</span><span class="sxs-lookup"><span data-stu-id="d78f0-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="d78f0-139">仅支持 membershipType 为 `private` 的频道。</span><span class="sxs-lookup"><span data-stu-id="d78f0-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="d78f0-140">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="d78f0-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="d78f0-141">无</span><span class="sxs-lookup"><span data-stu-id="d78f0-141">None</span></span> | <span data-ttu-id="d78f0-142">从频道中删除一个成员。</span><span class="sxs-lookup"><span data-stu-id="d78f0-142">Delete a member from a channel.</span></span> <span data-ttu-id="d78f0-143">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="d78f0-143">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="d78f0-144">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="d78f0-144">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="d78f0-145">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78f0-145">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="d78f0-146">获取聊天中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="d78f0-146">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="d78f0-147">添加聊天成员</span><span class="sxs-lookup"><span data-stu-id="d78f0-147">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="d78f0-148">位置标头</span><span class="sxs-lookup"><span data-stu-id="d78f0-148">Location header</span></span> | <span data-ttu-id="d78f0-149">向聊天添加成员。</span><span class="sxs-lookup"><span data-stu-id="d78f0-149">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="d78f0-150">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="d78f0-150">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="d78f0-151">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d78f0-151">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="d78f0-152">获取聊天中的成员。</span><span class="sxs-lookup"><span data-stu-id="d78f0-152">Get a member in a chat.</span></span>|
|[<span data-ttu-id="d78f0-153">删除聊天成员</span><span class="sxs-lookup"><span data-stu-id="d78f0-153">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="d78f0-154">无</span><span class="sxs-lookup"><span data-stu-id="d78f0-154">None</span></span> | <span data-ttu-id="d78f0-155">从聊天中删除成员。</span><span class="sxs-lookup"><span data-stu-id="d78f0-155">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="d78f0-156">属性</span><span class="sxs-lookup"><span data-stu-id="d78f0-156">Properties</span></span>

| <span data-ttu-id="d78f0-157">属性</span><span class="sxs-lookup"><span data-stu-id="d78f0-157">Property</span></span>   | <span data-ttu-id="d78f0-158">类型</span><span class="sxs-lookup"><span data-stu-id="d78f0-158">Type</span></span> |<span data-ttu-id="d78f0-159">说明</span><span class="sxs-lookup"><span data-stu-id="d78f0-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d78f0-160">id</span><span class="sxs-lookup"><span data-stu-id="d78f0-160">id</span></span>|<span data-ttu-id="d78f0-161">String</span><span class="sxs-lookup"><span data-stu-id="d78f0-161">String</span></span>| <span data-ttu-id="d78f0-p105">只读。用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="d78f0-p105">Read-only. Unique ID of the user.</span></span>|
|<span data-ttu-id="d78f0-164">displayName</span><span class="sxs-lookup"><span data-stu-id="d78f0-164">displayName</span></span>| <span data-ttu-id="d78f0-165">string</span><span class="sxs-lookup"><span data-stu-id="d78f0-165">string</span></span> | <span data-ttu-id="d78f0-166">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d78f0-166">The display name of the user.</span></span> |
|<span data-ttu-id="d78f0-167">角色</span><span class="sxs-lookup"><span data-stu-id="d78f0-167">roles</span></span>| <span data-ttu-id="d78f0-168">string 集合</span><span class="sxs-lookup"><span data-stu-id="d78f0-168">string collection</span></span> | <span data-ttu-id="d78f0-169">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="d78f0-169">The roles for that user.</span></span> |
|<span data-ttu-id="d78f0-170">userId</span><span class="sxs-lookup"><span data-stu-id="d78f0-170">userId</span></span>| <span data-ttu-id="d78f0-171">string</span><span class="sxs-lookup"><span data-stu-id="d78f0-171">string</span></span> | <span data-ttu-id="d78f0-172">用户的 GUID。</span><span class="sxs-lookup"><span data-stu-id="d78f0-172">The guid of the user.</span></span> |
|<span data-ttu-id="d78f0-173">email</span><span class="sxs-lookup"><span data-stu-id="d78f0-173">email</span></span>| <span data-ttu-id="d78f0-174">string</span><span class="sxs-lookup"><span data-stu-id="d78f0-174">string</span></span>  | <span data-ttu-id="d78f0-175">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d78f0-175">The email address of the user.</span></span> |
|<span data-ttu-id="d78f0-176">tenantId</span><span class="sxs-lookup"><span data-stu-id="d78f0-176">tenantId</span></span>| <span data-ttu-id="d78f0-177">string</span><span class="sxs-lookup"><span data-stu-id="d78f0-177">string</span></span>  | <span data-ttu-id="d78f0-178">Azure AD 用户从属的 TenantId。</span><span class="sxs-lookup"><span data-stu-id="d78f0-178">TenantId which the Azure AD user belongs to.</span></span> |
|<span data-ttu-id="d78f0-179">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="d78f0-179">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="d78f0-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d78f0-180">DateTimeOffset</span></span>  | <span data-ttu-id="d78f0-181">表示对话历史久远程度的时间戳与对话成员共享。</span><span class="sxs-lookup"><span data-stu-id="d78f0-181">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="d78f0-182">此属性只对聊天成员可设置。</span><span class="sxs-lookup"><span data-stu-id="d78f0-182">This property is settable only for members of a chat.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d78f0-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d78f0-183">JSON representation</span></span>

<span data-ttu-id="d78f0-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d78f0-184">The following is a JSON representation of the resource.</span></span>

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
  "id": "string (identifier)",
  "displayName" : "string",
  "visibleHistoryStartDateTime": "string (timestamp)",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string",
  "tenantId": "string"
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

