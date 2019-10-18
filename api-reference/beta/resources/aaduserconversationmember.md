---
title: aadUserConversationMember 资源类型
description: 表示聊天或频道中的 Azure Active Directory 用户。
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 058164d44ef6d9d6ba6667cf1cb7249bf57c2a83
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633508"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="dca96-103">aadUserConversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="dca96-103">aadUserConversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dca96-104">表示[聊天](chat.md)或[频道](channel.md)中的 Azure Active Directory 用户。</span><span class="sxs-lookup"><span data-stu-id="dca96-104">Represents an Azure Active Directory user in a [chat](chat.md) or [channel](channel.md).</span></span> <span data-ttu-id="dca96-105">此类型继承自 [conversationMember](conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="dca96-105">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dca96-106">方法</span><span class="sxs-lookup"><span data-stu-id="dca96-106">Methods</span></span>

| <span data-ttu-id="dca96-107">方法</span><span class="sxs-lookup"><span data-stu-id="dca96-107">Method</span></span>       | <span data-ttu-id="dca96-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="dca96-108">Return Type</span></span>  |<span data-ttu-id="dca96-109">说明</span><span class="sxs-lookup"><span data-stu-id="dca96-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dca96-110">列出成员</span><span class="sxs-lookup"><span data-stu-id="dca96-110">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="dca96-111">[conversationmember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dca96-111">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="dca96-112">获取包含聊天或频道中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="dca96-112">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="dca96-113">获取成员</span><span class="sxs-lookup"><span data-stu-id="dca96-113">Get member groups</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="dca96-114">conversationmember</span><span class="sxs-lookup"><span data-stu-id="dca96-114">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="dca96-115">获取聊天或频道中的一位用户。</span><span class="sxs-lookup"><span data-stu-id="dca96-115">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="dca96-116">添加成员</span><span class="sxs-lookup"><span data-stu-id="dca96-116">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="dca96-117">conversationMember</span><span class="sxs-lookup"><span data-stu-id="dca96-117">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="dca96-118">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="dca96-118">Add a member to a class.</span></span>|
|[<span data-ttu-id="dca96-119">更新成员</span><span class="sxs-lookup"><span data-stu-id="dca96-119">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="dca96-120">conversationMember</span><span class="sxs-lookup"><span data-stu-id="dca96-120">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="dca96-121">更新频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="dca96-121">Update a member in the channel.</span></span>|
|[<span data-ttu-id="dca96-122">删除成员</span><span class="sxs-lookup"><span data-stu-id="dca96-122">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="dca96-123">conversationMember</span><span class="sxs-lookup"><span data-stu-id="dca96-123">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="dca96-124">删除频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="dca96-124">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="dca96-125">属性</span><span class="sxs-lookup"><span data-stu-id="dca96-125">Properties</span></span>

| <span data-ttu-id="dca96-126">属性</span><span class="sxs-lookup"><span data-stu-id="dca96-126">Property</span></span>   | <span data-ttu-id="dca96-127">类型</span><span class="sxs-lookup"><span data-stu-id="dca96-127">Type</span></span> |<span data-ttu-id="dca96-128">说明</span><span class="sxs-lookup"><span data-stu-id="dca96-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dca96-129">id</span><span class="sxs-lookup"><span data-stu-id="dca96-129">id</span></span>|<span data-ttu-id="dca96-130">String</span><span class="sxs-lookup"><span data-stu-id="dca96-130">String</span></span>| <span data-ttu-id="dca96-131">只读。</span><span class="sxs-lookup"><span data-stu-id="dca96-131">Read-only.</span></span> <span data-ttu-id="dca96-132">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="dca96-132">Unique ID of the message.</span></span>|
|<span data-ttu-id="dca96-133">displayName</span><span class="sxs-lookup"><span data-stu-id="dca96-133">displayName</span></span>| <span data-ttu-id="dca96-134">string</span><span class="sxs-lookup"><span data-stu-id="dca96-134">string</span></span> | <span data-ttu-id="dca96-135">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dca96-135">The display name of the user.</span></span> |
|<span data-ttu-id="dca96-136">角色</span><span class="sxs-lookup"><span data-stu-id="dca96-136">roles</span></span>| <span data-ttu-id="dca96-137">string 集合</span><span class="sxs-lookup"><span data-stu-id="dca96-137">string collection</span></span> | <span data-ttu-id="dca96-138">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="dca96-138">The roles for that user.</span></span> |
|<span data-ttu-id="dca96-139">userId</span><span class="sxs-lookup"><span data-stu-id="dca96-139">userId</span></span>| <span data-ttu-id="dca96-140">string</span><span class="sxs-lookup"><span data-stu-id="dca96-140">string</span></span> | <span data-ttu-id="dca96-141">用户的 GUID。</span><span class="sxs-lookup"><span data-stu-id="dca96-141">The guid of the user.</span></span> |
|<span data-ttu-id="dca96-142">email</span><span class="sxs-lookup"><span data-stu-id="dca96-142">email</span></span>| <span data-ttu-id="dca96-143">string</span><span class="sxs-lookup"><span data-stu-id="dca96-143">string</span></span>  | <span data-ttu-id="dca96-144">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="dca96-144">The e-mail address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dca96-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dca96-145">JSON representation</span></span>

<span data-ttu-id="dca96-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dca96-146">The following is a JSON representation of the resource.</span></span>

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
