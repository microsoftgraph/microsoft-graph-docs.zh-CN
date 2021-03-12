---
title: 对话资源类型
description: 对话是 线程 集合，而线程包含相应线程拥有的帖子。 对话中的所有线程和帖子共享相同的主题。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 666dd7e287e8bb460b039b58fe99b39febf581d0
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720639"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="2b0b3-104">对话资源类型</span><span class="sxs-lookup"><span data-stu-id="2b0b3-104">conversation resource type</span></span>

<span data-ttu-id="2b0b3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b0b3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b0b3-p102">对话是 [线程](conversationthread.md) 集合，而线程包含相应线程拥有的帖子。对话中的所有线程和帖子共享相同的主题。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-p102">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="2b0b3-108">此资源支持订阅 [更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-108">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="2b0b3-109">Methods</span><span class="sxs-lookup"><span data-stu-id="2b0b3-109">Methods</span></span>

| <span data-ttu-id="2b0b3-110">方法</span><span class="sxs-lookup"><span data-stu-id="2b0b3-110">Method</span></span>       | <span data-ttu-id="2b0b3-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="2b0b3-111">Return Type</span></span>  |<span data-ttu-id="2b0b3-112">说明</span><span class="sxs-lookup"><span data-stu-id="2b0b3-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b0b3-113">列出对话</span><span class="sxs-lookup"><span data-stu-id="2b0b3-113">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="2b0b3-114">[conversation](conversation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2b0b3-114">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="2b0b3-115">获取此组中的对话列表。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-115">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="2b0b3-116">创建</span><span class="sxs-lookup"><span data-stu-id="2b0b3-116">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="2b0b3-117">对话</span><span class="sxs-lookup"><span data-stu-id="2b0b3-117">conversation</span></span>](conversation.md)| <span data-ttu-id="2b0b3-118">通过包括线程和帖子创建新对话。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-118">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="2b0b3-119">获取对话</span><span class="sxs-lookup"><span data-stu-id="2b0b3-119">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="2b0b3-120">conversation</span><span class="sxs-lookup"><span data-stu-id="2b0b3-120">conversation</span></span>](conversation.md) |<span data-ttu-id="2b0b3-121">读取 conversation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-121">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="2b0b3-122">删除</span><span class="sxs-lookup"><span data-stu-id="2b0b3-122">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="2b0b3-123">无</span><span class="sxs-lookup"><span data-stu-id="2b0b3-123">None</span></span> |<span data-ttu-id="2b0b3-124">删除 conversation 对象。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-124">Delete conversation object.</span></span> |
|[<span data-ttu-id="2b0b3-125">列出对话线程</span><span class="sxs-lookup"><span data-stu-id="2b0b3-125">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="2b0b3-126">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2b0b3-126">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="2b0b3-127">获取组对话中的所有线程。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-127">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="2b0b3-128">创建对话线程</span><span class="sxs-lookup"><span data-stu-id="2b0b3-128">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="2b0b3-129">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2b0b3-129">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="2b0b3-130">在指定会话中创建线程。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-130">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="2b0b3-131">属性</span><span class="sxs-lookup"><span data-stu-id="2b0b3-131">Properties</span></span>
| <span data-ttu-id="2b0b3-132">属性</span><span class="sxs-lookup"><span data-stu-id="2b0b3-132">Property</span></span>     | <span data-ttu-id="2b0b3-133">类型</span><span class="sxs-lookup"><span data-stu-id="2b0b3-133">Type</span></span>   |<span data-ttu-id="2b0b3-134">说明</span><span class="sxs-lookup"><span data-stu-id="2b0b3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b0b3-135">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="2b0b3-135">hasAttachments</span></span>|<span data-ttu-id="2b0b3-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b0b3-136">Boolean</span></span>|<span data-ttu-id="2b0b3-137">指示此对话中的任意帖子是否至少有一个附件。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-137">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="2b0b3-138">id</span><span class="sxs-lookup"><span data-stu-id="2b0b3-138">id</span></span>|<span data-ttu-id="2b0b3-139">字符串</span><span class="sxs-lookup"><span data-stu-id="2b0b3-139">String</span></span>|<span data-ttu-id="2b0b3-p103">对话的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-p103">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="2b0b3-142">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="2b0b3-142">lastDeliveredDateTime</span></span>|<span data-ttu-id="2b0b3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b0b3-143">DateTimeOffset</span></span>|<span data-ttu-id="2b0b3-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2b0b3-145">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="2b0b3-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="2b0b3-146">preview</span><span class="sxs-lookup"><span data-stu-id="2b0b3-146">preview</span></span>|<span data-ttu-id="2b0b3-147">String</span><span class="sxs-lookup"><span data-stu-id="2b0b3-147">String</span></span>|<span data-ttu-id="2b0b3-148">来自此对话中最新帖子的正文的简短摘要。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-148">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="2b0b3-149">topic</span><span class="sxs-lookup"><span data-stu-id="2b0b3-149">topic</span></span>|<span data-ttu-id="2b0b3-150">String</span><span class="sxs-lookup"><span data-stu-id="2b0b3-150">String</span></span>|<span data-ttu-id="2b0b3-p105">对话的主题。在创建对话时可设置此属性，但无法对其进行更新。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-p105">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="2b0b3-153">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="2b0b3-153">uniqueSenders</span></span>|<span data-ttu-id="2b0b3-154">String collection</span><span class="sxs-lookup"><span data-stu-id="2b0b3-154">String collection</span></span>|<span data-ttu-id="2b0b3-155">发送消息到此对话的所有用户。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-155">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b0b3-156">关系</span><span class="sxs-lookup"><span data-stu-id="2b0b3-156">Relationships</span></span>
| <span data-ttu-id="2b0b3-157">关系</span><span class="sxs-lookup"><span data-stu-id="2b0b3-157">Relationship</span></span> | <span data-ttu-id="2b0b3-158">类型</span><span class="sxs-lookup"><span data-stu-id="2b0b3-158">Type</span></span>   |<span data-ttu-id="2b0b3-159">说明</span><span class="sxs-lookup"><span data-stu-id="2b0b3-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b0b3-160">threads</span><span class="sxs-lookup"><span data-stu-id="2b0b3-160">threads</span></span>|<span data-ttu-id="2b0b3-161">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2b0b3-161">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="2b0b3-p106">对话中所有对话线程的集合。一种导航属性。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-p106">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b0b3-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b0b3-166">JSON representation</span></span>

<span data-ttu-id="2b0b3-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b0b3-167">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversation",
  "@odata.annotations": [
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"],

  "threads": [{"@odata.type": "microsoft.graph.conversationThread"}]
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

