---
title: 对话资源类型
description: 对话是 线程 集合，而线程包含相应线程拥有的帖子。对话中的所有线程和帖子共享相同的主题。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 0066a636d2b36e74443380598c2ca6e8daf826c1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928155"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="418c2-104">对话资源类型</span><span class="sxs-lookup"><span data-stu-id="418c2-104">conversation resource type</span></span>

<span data-ttu-id="418c2-p102">对话是 [线程](conversationthread.md) 集合，而线程包含相应线程拥有的帖子。对话中的所有线程和帖子共享相同的主题。</span><span class="sxs-lookup"><span data-stu-id="418c2-p102">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="418c2-107">此资源支持订阅[更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="418c2-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="418c2-108">方法</span><span class="sxs-lookup"><span data-stu-id="418c2-108">Methods</span></span>

| <span data-ttu-id="418c2-109">方法</span><span class="sxs-lookup"><span data-stu-id="418c2-109">Method</span></span>       | <span data-ttu-id="418c2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="418c2-110">Return Type</span></span>  |<span data-ttu-id="418c2-111">说明</span><span class="sxs-lookup"><span data-stu-id="418c2-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="418c2-112">列出对话</span><span class="sxs-lookup"><span data-stu-id="418c2-112">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="418c2-113">[对话](conversation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="418c2-113">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="418c2-114">获取此组中的对话列表。</span><span class="sxs-lookup"><span data-stu-id="418c2-114">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="418c2-115">创建</span><span class="sxs-lookup"><span data-stu-id="418c2-115">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="418c2-116">对话</span><span class="sxs-lookup"><span data-stu-id="418c2-116">conversation</span></span>](conversation.md)| <span data-ttu-id="418c2-117">通过包括线程和帖子创建新对话。</span><span class="sxs-lookup"><span data-stu-id="418c2-117">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="418c2-118">获取对话</span><span class="sxs-lookup"><span data-stu-id="418c2-118">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="418c2-119">对话</span><span class="sxs-lookup"><span data-stu-id="418c2-119">conversation</span></span>](conversation.md) |<span data-ttu-id="418c2-120">读取 conversation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="418c2-120">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="418c2-121">删除</span><span class="sxs-lookup"><span data-stu-id="418c2-121">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="418c2-122">无</span><span class="sxs-lookup"><span data-stu-id="418c2-122">None</span></span> |<span data-ttu-id="418c2-123">删除 conversation 对象</span><span class="sxs-lookup"><span data-stu-id="418c2-123">Delete conversation object.</span></span> |
|[<span data-ttu-id="418c2-124">列出对话线程</span><span class="sxs-lookup"><span data-stu-id="418c2-124">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="418c2-125">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="418c2-125">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="418c2-126">获取组对话中的所有线程。</span><span class="sxs-lookup"><span data-stu-id="418c2-126">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="418c2-127">创建对话线程</span><span class="sxs-lookup"><span data-stu-id="418c2-127">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="418c2-128">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="418c2-128">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="418c2-129">在指定会话中创建线程。</span><span class="sxs-lookup"><span data-stu-id="418c2-129">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="418c2-130">属性</span><span class="sxs-lookup"><span data-stu-id="418c2-130">Properties</span></span>
| <span data-ttu-id="418c2-131">属性</span><span class="sxs-lookup"><span data-stu-id="418c2-131">Property</span></span>     | <span data-ttu-id="418c2-132">类型</span><span class="sxs-lookup"><span data-stu-id="418c2-132">Type</span></span>   |<span data-ttu-id="418c2-133">说明</span><span class="sxs-lookup"><span data-stu-id="418c2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="418c2-134">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="418c2-134">hasAttachments</span></span>|<span data-ttu-id="418c2-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="418c2-135">Boolean</span></span>|<span data-ttu-id="418c2-136">指示此对话中的任意帖子是否至少有一个附件。</span><span class="sxs-lookup"><span data-stu-id="418c2-136">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="418c2-137">id</span><span class="sxs-lookup"><span data-stu-id="418c2-137">id</span></span>|<span data-ttu-id="418c2-138">String</span><span class="sxs-lookup"><span data-stu-id="418c2-138">String</span></span>|<span data-ttu-id="418c2-p103">对话的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="418c2-p103">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="418c2-141">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="418c2-141">lastDeliveredDateTime</span></span>|<span data-ttu-id="418c2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="418c2-142">DateTimeOffset</span></span>|<span data-ttu-id="418c2-p104">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="418c2-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="418c2-145">preview</span><span class="sxs-lookup"><span data-stu-id="418c2-145">preview</span></span>|<span data-ttu-id="418c2-146">String</span><span class="sxs-lookup"><span data-stu-id="418c2-146">String</span></span>|<span data-ttu-id="418c2-147">来自此对话中最新帖子的正文的简短摘要。</span><span class="sxs-lookup"><span data-stu-id="418c2-147">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="418c2-148">topic</span><span class="sxs-lookup"><span data-stu-id="418c2-148">topic</span></span>|<span data-ttu-id="418c2-149">String</span><span class="sxs-lookup"><span data-stu-id="418c2-149">String</span></span>|<span data-ttu-id="418c2-p105">对话的主题。在创建对话时可设置此属性，但无法对其进行更新。</span><span class="sxs-lookup"><span data-stu-id="418c2-p105">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="418c2-152">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="418c2-152">uniqueSenders</span></span>|<span data-ttu-id="418c2-153">String collection</span><span class="sxs-lookup"><span data-stu-id="418c2-153">String collection</span></span>|<span data-ttu-id="418c2-154">发送消息到此对话的所有用户。</span><span class="sxs-lookup"><span data-stu-id="418c2-154">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="418c2-155">Relationships</span><span class="sxs-lookup"><span data-stu-id="418c2-155">Relationships</span></span>
| <span data-ttu-id="418c2-156">关系</span><span class="sxs-lookup"><span data-stu-id="418c2-156">Relationship</span></span> | <span data-ttu-id="418c2-157">类型</span><span class="sxs-lookup"><span data-stu-id="418c2-157">Type</span></span>   |<span data-ttu-id="418c2-158">说明</span><span class="sxs-lookup"><span data-stu-id="418c2-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="418c2-159">线程</span><span class="sxs-lookup"><span data-stu-id="418c2-159">threads</span></span>|<span data-ttu-id="418c2-160">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="418c2-160">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="418c2-p106">对话中所有对话线程的集合。一种导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="418c2-p106">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="418c2-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="418c2-165">JSON representation</span></span>

<span data-ttu-id="418c2-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="418c2-166">Here is a JSON representation of the resource</span></span>

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
