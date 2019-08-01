---
title: 对话资源类型
description: 对话是 线程 集合，而线程包含相应线程拥有的帖子。 对话中的所有线程和帖子共享相同的主题。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 4c34f6f0d55cb27e5ce7f5f2ba6459cfbb4d5291
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029594"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="f750b-104">对话资源类型</span><span class="sxs-lookup"><span data-stu-id="f750b-104">conversation resource type</span></span>

<span data-ttu-id="f750b-p102">对话是 [线程](conversationthread.md) 集合，而线程包含相应线程拥有的帖子。对话中的所有线程和帖子共享相同的主题。</span><span class="sxs-lookup"><span data-stu-id="f750b-p102">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="f750b-107">此资源支持订阅[更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="f750b-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="f750b-108">方法</span><span class="sxs-lookup"><span data-stu-id="f750b-108">Methods</span></span>

| <span data-ttu-id="f750b-109">方法</span><span class="sxs-lookup"><span data-stu-id="f750b-109">Method</span></span>       | <span data-ttu-id="f750b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f750b-110">Return Type</span></span>  |<span data-ttu-id="f750b-111">说明</span><span class="sxs-lookup"><span data-stu-id="f750b-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f750b-112">列出对话</span><span class="sxs-lookup"><span data-stu-id="f750b-112">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="f750b-113">[conversation](conversation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f750b-113">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="f750b-114">获取此组中的对话列表。</span><span class="sxs-lookup"><span data-stu-id="f750b-114">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="f750b-115">创建</span><span class="sxs-lookup"><span data-stu-id="f750b-115">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="f750b-116">对话</span><span class="sxs-lookup"><span data-stu-id="f750b-116">conversation</span></span>](conversation.md)| <span data-ttu-id="f750b-117">通过包括线程和帖子创建新对话。</span><span class="sxs-lookup"><span data-stu-id="f750b-117">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="f750b-118">获取对话</span><span class="sxs-lookup"><span data-stu-id="f750b-118">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="f750b-119">conversation</span><span class="sxs-lookup"><span data-stu-id="f750b-119">conversation</span></span>](conversation.md) |<span data-ttu-id="f750b-120">读取 conversation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f750b-120">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="f750b-121">删除</span><span class="sxs-lookup"><span data-stu-id="f750b-121">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="f750b-122">无</span><span class="sxs-lookup"><span data-stu-id="f750b-122">None</span></span> |<span data-ttu-id="f750b-123">删除 conversation 对象。</span><span class="sxs-lookup"><span data-stu-id="f750b-123">Delete conversation object.</span></span> |
|[<span data-ttu-id="f750b-124">列出对话线程</span><span class="sxs-lookup"><span data-stu-id="f750b-124">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="f750b-125">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f750b-125">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="f750b-126">获取组对话中的所有线程。</span><span class="sxs-lookup"><span data-stu-id="f750b-126">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="f750b-127">创建对话线程</span><span class="sxs-lookup"><span data-stu-id="f750b-127">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="f750b-128">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f750b-128">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="f750b-129">在指定会话中创建线程。</span><span class="sxs-lookup"><span data-stu-id="f750b-129">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="f750b-130">属性</span><span class="sxs-lookup"><span data-stu-id="f750b-130">Properties</span></span>
| <span data-ttu-id="f750b-131">属性</span><span class="sxs-lookup"><span data-stu-id="f750b-131">Property</span></span>     | <span data-ttu-id="f750b-132">类型</span><span class="sxs-lookup"><span data-stu-id="f750b-132">Type</span></span>   |<span data-ttu-id="f750b-133">说明</span><span class="sxs-lookup"><span data-stu-id="f750b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f750b-134">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="f750b-134">hasAttachments</span></span>|<span data-ttu-id="f750b-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="f750b-135">Boolean</span></span>|<span data-ttu-id="f750b-136">指示此对话中的任意帖子是否至少有一个附件。</span><span class="sxs-lookup"><span data-stu-id="f750b-136">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="f750b-137">id</span><span class="sxs-lookup"><span data-stu-id="f750b-137">id</span></span>|<span data-ttu-id="f750b-138">String</span><span class="sxs-lookup"><span data-stu-id="f750b-138">String</span></span>|<span data-ttu-id="f750b-p103">对话的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="f750b-p103">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="f750b-141">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="f750b-141">lastDeliveredDateTime</span></span>|<span data-ttu-id="f750b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f750b-142">DateTimeOffset</span></span>|<span data-ttu-id="f750b-p104">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f750b-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f750b-145">preview</span><span class="sxs-lookup"><span data-stu-id="f750b-145">preview</span></span>|<span data-ttu-id="f750b-146">String</span><span class="sxs-lookup"><span data-stu-id="f750b-146">String</span></span>|<span data-ttu-id="f750b-147">来自此对话中最新帖子的正文的简短摘要。</span><span class="sxs-lookup"><span data-stu-id="f750b-147">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="f750b-148">topic</span><span class="sxs-lookup"><span data-stu-id="f750b-148">topic</span></span>|<span data-ttu-id="f750b-149">String</span><span class="sxs-lookup"><span data-stu-id="f750b-149">String</span></span>|<span data-ttu-id="f750b-p105">对话的主题。在创建对话时可设置此属性，但无法对其进行更新。</span><span class="sxs-lookup"><span data-stu-id="f750b-p105">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="f750b-152">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="f750b-152">uniqueSenders</span></span>|<span data-ttu-id="f750b-153">String collection</span><span class="sxs-lookup"><span data-stu-id="f750b-153">String collection</span></span>|<span data-ttu-id="f750b-154">发送消息到此对话的所有用户。</span><span class="sxs-lookup"><span data-stu-id="f750b-154">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f750b-155">关系</span><span class="sxs-lookup"><span data-stu-id="f750b-155">Relationships</span></span>
| <span data-ttu-id="f750b-156">关系</span><span class="sxs-lookup"><span data-stu-id="f750b-156">Relationship</span></span> | <span data-ttu-id="f750b-157">类型</span><span class="sxs-lookup"><span data-stu-id="f750b-157">Type</span></span>   |<span data-ttu-id="f750b-158">说明</span><span class="sxs-lookup"><span data-stu-id="f750b-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f750b-159">threads</span><span class="sxs-lookup"><span data-stu-id="f750b-159">threads</span></span>|<span data-ttu-id="f750b-160">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f750b-160">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="f750b-p106">对话中所有对话线程的集合。一种导航属性。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="f750b-p106">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f750b-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f750b-165">JSON representation</span></span>

<span data-ttu-id="f750b-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f750b-166">Here is a JSON representation of the resource</span></span>

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
