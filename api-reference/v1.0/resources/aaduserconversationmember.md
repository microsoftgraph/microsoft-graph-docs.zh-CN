---
title: aadUserConversationMember 资源类型
description: 表示聊天或频道中的 Azure Active Directory 用户。
localization_priority: Priority
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cf678e090f4af26aca1222ba464771111b0b6a60
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754297"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="d5a34-103">aadUserConversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5a34-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="d5a34-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5a34-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5a34-105">表示[团队](team.md)、[频道](channel.md)或[聊天](chat.md)中的 Azure Active Directory 用户。</span><span class="sxs-lookup"><span data-stu-id="d5a34-105">Represents an Azure Active Directory user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="d5a34-106">此类型继承自 [conversationMember](conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="d5a34-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d5a34-107">方法</span><span class="sxs-lookup"><span data-stu-id="d5a34-107">Methods</span></span>

| <span data-ttu-id="d5a34-108">方法</span><span class="sxs-lookup"><span data-stu-id="d5a34-108">Method</span></span>       | <span data-ttu-id="d5a34-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d5a34-109">Return Type</span></span>  |<span data-ttu-id="d5a34-110">说明</span><span class="sxs-lookup"><span data-stu-id="d5a34-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d5a34-111">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="d5a34-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="d5a34-112">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5a34-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="d5a34-113">获取此团队中的成员列表。</span><span class="sxs-lookup"><span data-stu-id="d5a34-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="d5a34-114">添加团队成员</span><span class="sxs-lookup"><span data-stu-id="d5a34-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="d5a34-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d5a34-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="d5a34-116">向团队中添加新成员。</span><span class="sxs-lookup"><span data-stu-id="d5a34-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="d5a34-117">获取团队成员</span><span class="sxs-lookup"><span data-stu-id="d5a34-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="d5a34-118">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5a34-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="d5a34-119">获取团队中的成员。</span><span class="sxs-lookup"><span data-stu-id="d5a34-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="d5a34-120">更新成员角色</span><span class="sxs-lookup"><span data-stu-id="d5a34-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="d5a34-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d5a34-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="d5a34-122">将成员更改为所有者或返回为常规成员。</span><span class="sxs-lookup"><span data-stu-id="d5a34-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="d5a34-123">删除团队成员</span><span class="sxs-lookup"><span data-stu-id="d5a34-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="d5a34-124">无</span><span class="sxs-lookup"><span data-stu-id="d5a34-124">None</span></span>|<span data-ttu-id="d5a34-125">删除团队中的一个现有成员。</span><span class="sxs-lookup"><span data-stu-id="d5a34-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="d5a34-126">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="d5a34-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="d5a34-127">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5a34-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="d5a34-128">获取频道中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="d5a34-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="d5a34-129">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="d5a34-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="d5a34-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d5a34-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="d5a34-131">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="d5a34-131">Add a member to a channel.</span></span> <span data-ttu-id="d5a34-132">仅支持 membershipType 为 `private` 的 `channel`。</span><span class="sxs-lookup"><span data-stu-id="d5a34-132">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="d5a34-133">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="d5a34-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="d5a34-134">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5a34-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="d5a34-135">获取频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="d5a34-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="d5a34-136">更新频道成员角色</span><span class="sxs-lookup"><span data-stu-id="d5a34-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="d5a34-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d5a34-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="d5a34-138">更新频道成员的属性。</span><span class="sxs-lookup"><span data-stu-id="d5a34-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="d5a34-139">仅支持 membershipType 为 `private` 的频道。</span><span class="sxs-lookup"><span data-stu-id="d5a34-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="d5a34-140">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="d5a34-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="d5a34-141">无</span><span class="sxs-lookup"><span data-stu-id="d5a34-141">None</span></span> | <span data-ttu-id="d5a34-142">从频道中删除一个成员。</span><span class="sxs-lookup"><span data-stu-id="d5a34-142">Delete a member from a channel.</span></span> <span data-ttu-id="d5a34-143">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="d5a34-143">Only supported for `channelType` of `private`.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5a34-144">属性</span><span class="sxs-lookup"><span data-stu-id="d5a34-144">Properties</span></span>

| <span data-ttu-id="d5a34-145">属性</span><span class="sxs-lookup"><span data-stu-id="d5a34-145">Property</span></span>   | <span data-ttu-id="d5a34-146">类型</span><span class="sxs-lookup"><span data-stu-id="d5a34-146">Type</span></span> |<span data-ttu-id="d5a34-147">说明</span><span class="sxs-lookup"><span data-stu-id="d5a34-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5a34-148">id</span><span class="sxs-lookup"><span data-stu-id="d5a34-148">id</span></span>|<span data-ttu-id="d5a34-149">String</span><span class="sxs-lookup"><span data-stu-id="d5a34-149">String</span></span>| <span data-ttu-id="d5a34-150">只读。</span><span class="sxs-lookup"><span data-stu-id="d5a34-150">Read-only.</span></span> <span data-ttu-id="d5a34-151">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="d5a34-151">Unique ID of the user.</span></span>|
|<span data-ttu-id="d5a34-152">displayName</span><span class="sxs-lookup"><span data-stu-id="d5a34-152">displayName</span></span>| <span data-ttu-id="d5a34-153">string</span><span class="sxs-lookup"><span data-stu-id="d5a34-153">string</span></span> | <span data-ttu-id="d5a34-154">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d5a34-154">The display name of the user.</span></span> |
|<span data-ttu-id="d5a34-155">角色</span><span class="sxs-lookup"><span data-stu-id="d5a34-155">roles</span></span>| <span data-ttu-id="d5a34-156">string 集合</span><span class="sxs-lookup"><span data-stu-id="d5a34-156">string collection</span></span> | <span data-ttu-id="d5a34-157">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="d5a34-157">The roles for that user.</span></span> |
|<span data-ttu-id="d5a34-158">userId</span><span class="sxs-lookup"><span data-stu-id="d5a34-158">userId</span></span>| <span data-ttu-id="d5a34-159">string</span><span class="sxs-lookup"><span data-stu-id="d5a34-159">string</span></span> | <span data-ttu-id="d5a34-160">用户的 GUID。</span><span class="sxs-lookup"><span data-stu-id="d5a34-160">The guid of the user.</span></span> |
|<span data-ttu-id="d5a34-161">email</span><span class="sxs-lookup"><span data-stu-id="d5a34-161">email</span></span>| <span data-ttu-id="d5a34-162">string</span><span class="sxs-lookup"><span data-stu-id="d5a34-162">string</span></span>  | <span data-ttu-id="d5a34-163">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d5a34-163">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d5a34-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5a34-164">JSON representation</span></span>

<span data-ttu-id="d5a34-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5a34-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.aadUserConversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string"
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

