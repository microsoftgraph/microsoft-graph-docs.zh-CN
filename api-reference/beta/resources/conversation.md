---
title: 对话资源类型
description: 对话是 线程 集合，而线程包含相应线程拥有的帖子。对话中的所有线程和帖子共享相同的主题。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5cacad2b9539c398251ffd07899df7beb3c2f378
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991438"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="0d4ee-104">对话资源类型</span><span class="sxs-lookup"><span data-stu-id="0d4ee-104">conversation resource type</span></span>

> <span data-ttu-id="0d4ee-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d4ee-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d4ee-p103">对话是 [线程](conversationthread.md) 集合，而线程包含相应线程拥有的帖子。对话中的所有线程和帖子共享相同的主题。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-p103">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="0d4ee-109">此资源支持订阅[更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-109">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="0d4ee-110">方法</span><span class="sxs-lookup"><span data-stu-id="0d4ee-110">Methods</span></span>

| <span data-ttu-id="0d4ee-111">方法</span><span class="sxs-lookup"><span data-stu-id="0d4ee-111">Method</span></span>       | <span data-ttu-id="0d4ee-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="0d4ee-112">Return Type</span></span>  |<span data-ttu-id="0d4ee-113">说明</span><span class="sxs-lookup"><span data-stu-id="0d4ee-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d4ee-114">列出对话</span><span class="sxs-lookup"><span data-stu-id="0d4ee-114">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="0d4ee-115">[对话](conversation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d4ee-115">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="0d4ee-116">获取此组中的对话列表。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-116">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="0d4ee-117">创建</span><span class="sxs-lookup"><span data-stu-id="0d4ee-117">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="0d4ee-118">对话</span><span class="sxs-lookup"><span data-stu-id="0d4ee-118">conversation</span></span>](conversation.md)| <span data-ttu-id="0d4ee-119">通过包括线程和帖子创建新对话。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-119">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="0d4ee-120">获取对话</span><span class="sxs-lookup"><span data-stu-id="0d4ee-120">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="0d4ee-121">对话</span><span class="sxs-lookup"><span data-stu-id="0d4ee-121">conversation</span></span>](conversation.md) |<span data-ttu-id="0d4ee-122">读取 conversation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-122">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="0d4ee-123">删除</span><span class="sxs-lookup"><span data-stu-id="0d4ee-123">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="0d4ee-124">无</span><span class="sxs-lookup"><span data-stu-id="0d4ee-124">None</span></span> |<span data-ttu-id="0d4ee-125">删除 conversation 对象</span><span class="sxs-lookup"><span data-stu-id="0d4ee-125">Delete conversation object.</span></span> |
|[<span data-ttu-id="0d4ee-126">列出对话线程</span><span class="sxs-lookup"><span data-stu-id="0d4ee-126">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="0d4ee-127">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d4ee-127">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="0d4ee-128">获取组对话中的所有线程。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-128">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="0d4ee-129">创建对话线程</span><span class="sxs-lookup"><span data-stu-id="0d4ee-129">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="0d4ee-130">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d4ee-130">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="0d4ee-131">在指定会话中创建线程。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-131">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="0d4ee-132">属性</span><span class="sxs-lookup"><span data-stu-id="0d4ee-132">Properties</span></span>
| <span data-ttu-id="0d4ee-133">属性</span><span class="sxs-lookup"><span data-stu-id="0d4ee-133">Property</span></span>     | <span data-ttu-id="0d4ee-134">类型</span><span class="sxs-lookup"><span data-stu-id="0d4ee-134">Type</span></span>   |<span data-ttu-id="0d4ee-135">说明</span><span class="sxs-lookup"><span data-stu-id="0d4ee-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d4ee-136">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="0d4ee-136">hasAttachments</span></span>|<span data-ttu-id="0d4ee-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d4ee-137">Boolean</span></span>|<span data-ttu-id="0d4ee-138">指示此对话中的任意帖子是否至少有一个附件。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-138">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="0d4ee-139">id</span><span class="sxs-lookup"><span data-stu-id="0d4ee-139">id</span></span>|<span data-ttu-id="0d4ee-140">String</span><span class="sxs-lookup"><span data-stu-id="0d4ee-140">String</span></span>|<span data-ttu-id="0d4ee-p104">对话的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-p104">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="0d4ee-143">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="0d4ee-143">lastDeliveredDateTime</span></span>|<span data-ttu-id="0d4ee-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d4ee-144">DateTimeOffset</span></span>|<span data-ttu-id="0d4ee-p105">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0d4ee-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0d4ee-147">preview</span><span class="sxs-lookup"><span data-stu-id="0d4ee-147">preview</span></span>|<span data-ttu-id="0d4ee-148">String</span><span class="sxs-lookup"><span data-stu-id="0d4ee-148">String</span></span>|<span data-ttu-id="0d4ee-149">来自此对话中最新帖子的正文的简短摘要。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-149">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="0d4ee-150">topic</span><span class="sxs-lookup"><span data-stu-id="0d4ee-150">topic</span></span>|<span data-ttu-id="0d4ee-151">String</span><span class="sxs-lookup"><span data-stu-id="0d4ee-151">String</span></span>|<span data-ttu-id="0d4ee-p106">对话的主题。在创建对话时可设置此属性，但无法对其进行更新。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-p106">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="0d4ee-154">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="0d4ee-154">uniqueSenders</span></span>|<span data-ttu-id="0d4ee-155">String collection</span><span class="sxs-lookup"><span data-stu-id="0d4ee-155">String collection</span></span>|<span data-ttu-id="0d4ee-156">发送消息到此对话的所有用户。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-156">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d4ee-157">Relationships</span><span class="sxs-lookup"><span data-stu-id="0d4ee-157">Relationships</span></span>
| <span data-ttu-id="0d4ee-158">关系</span><span class="sxs-lookup"><span data-stu-id="0d4ee-158">Relationship</span></span> | <span data-ttu-id="0d4ee-159">类型</span><span class="sxs-lookup"><span data-stu-id="0d4ee-159">Type</span></span>   |<span data-ttu-id="0d4ee-160">说明</span><span class="sxs-lookup"><span data-stu-id="0d4ee-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d4ee-161">线程</span><span class="sxs-lookup"><span data-stu-id="0d4ee-161">threads</span></span>|<span data-ttu-id="0d4ee-162">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d4ee-162">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="0d4ee-p107">对话中所有对话线程的集合。一种导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-p107">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d4ee-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d4ee-167">JSON representation</span></span>

<span data-ttu-id="0d4ee-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d4ee-168">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversation"
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
