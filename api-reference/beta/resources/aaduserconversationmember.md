---
title: aadUserConversationMember 资源类型
description: 表示聊天或频道中的 Azure Active Directory 用户。
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: caf8336d58ee40fcc1bf51b569cf334ba99294fc
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228350"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="ea80c-103">aadUserConversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea80c-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="ea80c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea80c-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="ea80c-105">表示[聊天](chat.md)或[频道](channel.md)中的 Azure Active Directory 用户。</span><span class="sxs-lookup"><span data-stu-id="ea80c-105">Represents an Azure Active Directory user in a [chat](chat.md) or [channel](channel.md).</span></span> <span data-ttu-id="ea80c-106">此类型继承自 [conversationMember](conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="ea80c-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ea80c-107">方法</span><span class="sxs-lookup"><span data-stu-id="ea80c-107">Methods</span></span>

| <span data-ttu-id="ea80c-108">方法</span><span class="sxs-lookup"><span data-stu-id="ea80c-108">Method</span></span>       | <span data-ttu-id="ea80c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ea80c-109">Return Type</span></span>  |<span data-ttu-id="ea80c-110">说明</span><span class="sxs-lookup"><span data-stu-id="ea80c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ea80c-111">列出成员</span><span class="sxs-lookup"><span data-stu-id="ea80c-111">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="ea80c-112">[conversationmember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ea80c-112">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="ea80c-113">获取包含聊天或频道中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="ea80c-113">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="ea80c-114">获取成员</span><span class="sxs-lookup"><span data-stu-id="ea80c-114">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="ea80c-115">conversationmember</span><span class="sxs-lookup"><span data-stu-id="ea80c-115">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="ea80c-116">获取聊天或频道中的一位用户。</span><span class="sxs-lookup"><span data-stu-id="ea80c-116">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="ea80c-117">添加成员</span><span class="sxs-lookup"><span data-stu-id="ea80c-117">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="ea80c-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ea80c-118">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="ea80c-119">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="ea80c-119">Add a member to a channel.</span></span>|
|[<span data-ttu-id="ea80c-120">更新成员</span><span class="sxs-lookup"><span data-stu-id="ea80c-120">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="ea80c-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ea80c-121">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="ea80c-122">更新频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="ea80c-122">Update a member in the channel.</span></span>|
|[<span data-ttu-id="ea80c-123">删除成员</span><span class="sxs-lookup"><span data-stu-id="ea80c-123">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="ea80c-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ea80c-124">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="ea80c-125">删除频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="ea80c-125">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea80c-126">属性</span><span class="sxs-lookup"><span data-stu-id="ea80c-126">Properties</span></span>

| <span data-ttu-id="ea80c-127">属性</span><span class="sxs-lookup"><span data-stu-id="ea80c-127">Property</span></span>   | <span data-ttu-id="ea80c-128">类型</span><span class="sxs-lookup"><span data-stu-id="ea80c-128">Type</span></span> |<span data-ttu-id="ea80c-129">说明</span><span class="sxs-lookup"><span data-stu-id="ea80c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea80c-130">id</span><span class="sxs-lookup"><span data-stu-id="ea80c-130">id</span></span>|<span data-ttu-id="ea80c-131">String</span><span class="sxs-lookup"><span data-stu-id="ea80c-131">String</span></span>| <span data-ttu-id="ea80c-132">只读。</span><span class="sxs-lookup"><span data-stu-id="ea80c-132">Read-only.</span></span> <span data-ttu-id="ea80c-133">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="ea80c-133">Unique ID of the user.</span></span>|
|<span data-ttu-id="ea80c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ea80c-134">displayName</span></span>| <span data-ttu-id="ea80c-135">string</span><span class="sxs-lookup"><span data-stu-id="ea80c-135">string</span></span> | <span data-ttu-id="ea80c-136">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ea80c-136">The display name of the user.</span></span> |
|<span data-ttu-id="ea80c-137">角色</span><span class="sxs-lookup"><span data-stu-id="ea80c-137">roles</span></span>| <span data-ttu-id="ea80c-138">string 集合</span><span class="sxs-lookup"><span data-stu-id="ea80c-138">string collection</span></span> | <span data-ttu-id="ea80c-139">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="ea80c-139">The roles for that user.</span></span> |
|<span data-ttu-id="ea80c-140">userId</span><span class="sxs-lookup"><span data-stu-id="ea80c-140">userId</span></span>| <span data-ttu-id="ea80c-141">string</span><span class="sxs-lookup"><span data-stu-id="ea80c-141">string</span></span> | <span data-ttu-id="ea80c-142">用户的 GUID。</span><span class="sxs-lookup"><span data-stu-id="ea80c-142">The guid of the user.</span></span> |
|<span data-ttu-id="ea80c-143">email</span><span class="sxs-lookup"><span data-stu-id="ea80c-143">email</span></span>| <span data-ttu-id="ea80c-144">string</span><span class="sxs-lookup"><span data-stu-id="ea80c-144">string</span></span>  | <span data-ttu-id="ea80c-145">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="ea80c-145">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ea80c-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea80c-146">JSON representation</span></span>

<span data-ttu-id="ea80c-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea80c-147">The following is a JSON representation of the resource.</span></span>

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
