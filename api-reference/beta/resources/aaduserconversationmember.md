---
title: aadUserConversationMember 资源类型
description: 表示聊天或频道中的 Azure Active Directory 用户。
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7f19c5a2b711ab6c39069364c641066f1d9c6dbf
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705966"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="dc74f-103">aadUserConversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc74f-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="dc74f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc74f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc74f-105">表示[聊天](chat.md)或[频道](channel.md)中的 Azure Active Directory 用户。</span><span class="sxs-lookup"><span data-stu-id="dc74f-105">Represents an Azure Active Directory user in a [chat](chat.md) or [channel](channel.md).</span></span> <span data-ttu-id="dc74f-106">此类型继承自 [conversationMember](conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="dc74f-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dc74f-107">方法</span><span class="sxs-lookup"><span data-stu-id="dc74f-107">Methods</span></span>

| <span data-ttu-id="dc74f-108">方法</span><span class="sxs-lookup"><span data-stu-id="dc74f-108">Method</span></span>       | <span data-ttu-id="dc74f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="dc74f-109">Return Type</span></span>  |<span data-ttu-id="dc74f-110">说明</span><span class="sxs-lookup"><span data-stu-id="dc74f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dc74f-111">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="dc74f-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="dc74f-112">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc74f-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="dc74f-113">获取此团队中的成员列表。</span><span class="sxs-lookup"><span data-stu-id="dc74f-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="dc74f-114">获取团队成员</span><span class="sxs-lookup"><span data-stu-id="dc74f-114">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="dc74f-115">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc74f-115">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="dc74f-116">获取团队中的成员。</span><span class="sxs-lookup"><span data-stu-id="dc74f-116">Get a member in the team.</span></span>|
|[<span data-ttu-id="dc74f-117">添加团队成员</span><span class="sxs-lookup"><span data-stu-id="dc74f-117">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="dc74f-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="dc74f-118">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="dc74f-119">向团队中添加新成员。</span><span class="sxs-lookup"><span data-stu-id="dc74f-119">Add a new member to the team.</span></span>|
|[<span data-ttu-id="dc74f-120">批量添加团队成员。</span><span class="sxs-lookup"><span data-stu-id="dc74f-120">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="dc74f-121">[actionResultPart](../resources/actionresultpart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc74f-121">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="dc74f-122">在单个请求中将多个成员添加到团队中。</span><span class="sxs-lookup"><span data-stu-id="dc74f-122">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="dc74f-123">更新成员角色</span><span class="sxs-lookup"><span data-stu-id="dc74f-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="dc74f-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="dc74f-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="dc74f-125">将成员更改为所有者或返回为常规成员。</span><span class="sxs-lookup"><span data-stu-id="dc74f-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="dc74f-126">删除团队成员</span><span class="sxs-lookup"><span data-stu-id="dc74f-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="dc74f-127">无</span><span class="sxs-lookup"><span data-stu-id="dc74f-127">None</span></span>|<span data-ttu-id="dc74f-128">删除团队中的一个现有成员。</span><span class="sxs-lookup"><span data-stu-id="dc74f-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="dc74f-129">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="dc74f-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="dc74f-130">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc74f-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="dc74f-131">获取频道中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="dc74f-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="dc74f-132">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="dc74f-132">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="dc74f-133">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc74f-133">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="dc74f-134">获取频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="dc74f-134">Get a member in a channel.</span></span>|
|[<span data-ttu-id="dc74f-135">创建频道成员</span><span class="sxs-lookup"><span data-stu-id="dc74f-135">Create channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="dc74f-136">conversationMember</span><span class="sxs-lookup"><span data-stu-id="dc74f-136">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="dc74f-137">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="dc74f-137">Add a member to a channel.</span></span> <span data-ttu-id="dc74f-138">仅支持 membershipType 为 `private` 的 `channel`。</span><span class="sxs-lookup"><span data-stu-id="dc74f-138">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="dc74f-139">更新频道成员角色</span><span class="sxs-lookup"><span data-stu-id="dc74f-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="dc74f-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="dc74f-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="dc74f-141">更新频道成员的属性。</span><span class="sxs-lookup"><span data-stu-id="dc74f-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="dc74f-142">仅支持 membershipType 为 `private` 的频道。</span><span class="sxs-lookup"><span data-stu-id="dc74f-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="dc74f-143">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="dc74f-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="dc74f-144">无</span><span class="sxs-lookup"><span data-stu-id="dc74f-144">None</span></span> | <span data-ttu-id="dc74f-145">从频道中删除一个成员。</span><span class="sxs-lookup"><span data-stu-id="dc74f-145">Delete a member from a channel.</span></span> <span data-ttu-id="dc74f-146">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="dc74f-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="dc74f-147">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="dc74f-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="dc74f-148">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc74f-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="dc74f-149">获取聊天中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="dc74f-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="dc74f-150">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="dc74f-150">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="dc74f-151">conversationMember</span><span class="sxs-lookup"><span data-stu-id="dc74f-151">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="dc74f-152">获取频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="dc74f-152">Get a member in a chat.</span></span>|
|[<span data-ttu-id="dc74f-153">添加聊天成员</span><span class="sxs-lookup"><span data-stu-id="dc74f-153">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="dc74f-154">位置标头</span><span class="sxs-lookup"><span data-stu-id="dc74f-154">Location header</span></span> | <span data-ttu-id="dc74f-155">向聊天添加成员。</span><span class="sxs-lookup"><span data-stu-id="dc74f-155">Add a member to a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="dc74f-156">属性</span><span class="sxs-lookup"><span data-stu-id="dc74f-156">Properties</span></span>

| <span data-ttu-id="dc74f-157">属性</span><span class="sxs-lookup"><span data-stu-id="dc74f-157">Property</span></span>   | <span data-ttu-id="dc74f-158">类型</span><span class="sxs-lookup"><span data-stu-id="dc74f-158">Type</span></span> |<span data-ttu-id="dc74f-159">说明</span><span class="sxs-lookup"><span data-stu-id="dc74f-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc74f-160">id</span><span class="sxs-lookup"><span data-stu-id="dc74f-160">id</span></span>| <span data-ttu-id="dc74f-161">字符串</span><span class="sxs-lookup"><span data-stu-id="dc74f-161">String</span></span> | <span data-ttu-id="dc74f-162">只读。</span><span class="sxs-lookup"><span data-stu-id="dc74f-162">Read-only.</span></span> <span data-ttu-id="dc74f-163">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="dc74f-163">Unique ID of the user.</span></span>|
|<span data-ttu-id="dc74f-164">displayName</span><span class="sxs-lookup"><span data-stu-id="dc74f-164">displayName</span></span>| <span data-ttu-id="dc74f-165">字符串</span><span class="sxs-lookup"><span data-stu-id="dc74f-165">String</span></span> | <span data-ttu-id="dc74f-166">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dc74f-166">The display name of the user.</span></span> |
|<span data-ttu-id="dc74f-167">角色</span><span class="sxs-lookup"><span data-stu-id="dc74f-167">roles</span></span>| <span data-ttu-id="dc74f-168">String 集合</span><span class="sxs-lookup"><span data-stu-id="dc74f-168">String collection</span></span> | <span data-ttu-id="dc74f-169">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="dc74f-169">The roles for that user.</span></span> |
|<span data-ttu-id="dc74f-170">userId</span><span class="sxs-lookup"><span data-stu-id="dc74f-170">userId</span></span>| <span data-ttu-id="dc74f-171">字符串</span><span class="sxs-lookup"><span data-stu-id="dc74f-171">String</span></span> | <span data-ttu-id="dc74f-172">用户的 GUID。</span><span class="sxs-lookup"><span data-stu-id="dc74f-172">The GUID of the user.</span></span> |
|<span data-ttu-id="dc74f-173">email</span><span class="sxs-lookup"><span data-stu-id="dc74f-173">email</span></span>| <span data-ttu-id="dc74f-174">字符串</span><span class="sxs-lookup"><span data-stu-id="dc74f-174">String</span></span>  | <span data-ttu-id="dc74f-175">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="dc74f-175">The email address of the user.</span></span> |
|<span data-ttu-id="dc74f-176">tenantId</span><span class="sxs-lookup"><span data-stu-id="dc74f-176">tenantId</span></span>| <span data-ttu-id="dc74f-177">string</span><span class="sxs-lookup"><span data-stu-id="dc74f-177">string</span></span>  | <span data-ttu-id="dc74f-178">Azure AD 用户从属的 TenantId。</span><span class="sxs-lookup"><span data-stu-id="dc74f-178">TenantId which the Azure AD user belongs to.</span></span> |
|<span data-ttu-id="dc74f-179">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="dc74f-179">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="dc74f-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc74f-180">DateTimeOffset</span></span>  | <span data-ttu-id="dc74f-181">表示对话历史久远程度的时间戳与对话成员共享。</span><span class="sxs-lookup"><span data-stu-id="dc74f-181">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="dc74f-182">此属性只对聊天成员可设置。</span><span class="sxs-lookup"><span data-stu-id="dc74f-182">This property is settable only for members of a chat.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc74f-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc74f-183">JSON representation</span></span>

<span data-ttu-id="dc74f-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc74f-184">The following is a JSON representation of the resource.</span></span>

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
