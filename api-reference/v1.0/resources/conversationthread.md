---
title: conversationThread 资源类型
description: conversationThread 是 帖子 集合。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a1a45f5ac6d26b58f1179616d3a6b9b76c6c1618
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912314"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="20e61-103">conversationThread 资源类型</span><span class="sxs-lookup"><span data-stu-id="20e61-103">conversationThread resource type</span></span>
<span data-ttu-id="20e61-104">conversationThread 是 [帖子](post.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="20e61-104">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="20e61-p101">最后一个帖子收件人集合聚合了整个线程的收件人。线程的收件人集合可以不断扩大。从线程中移除某个收件人时将创建一个新的线程。</span><span class="sxs-lookup"><span data-stu-id="20e61-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="20e61-108">方法</span><span class="sxs-lookup"><span data-stu-id="20e61-108">Methods</span></span>

| <span data-ttu-id="20e61-109">方法</span><span class="sxs-lookup"><span data-stu-id="20e61-109">Method</span></span>       | <span data-ttu-id="20e61-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="20e61-110">Return Type</span></span>  |<span data-ttu-id="20e61-111">说明</span><span class="sxs-lookup"><span data-stu-id="20e61-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="20e61-112">列出线程</span><span class="sxs-lookup"><span data-stu-id="20e61-112">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="20e61-113">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="20e61-113">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="20e61-114">获取某个组的所有线程。</span><span class="sxs-lookup"><span data-stu-id="20e61-114">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="20e61-115">创建线程</span><span class="sxs-lookup"><span data-stu-id="20e61-115">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="20e61-116">conversationThread</span><span class="sxs-lookup"><span data-stu-id="20e61-116">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="20e61-p102">通过首先创建一个线程，启动一个新对话。在组中创建新对话、对话线程和帖子。</span><span class="sxs-lookup"><span data-stu-id="20e61-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="20e61-119">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="20e61-119">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="20e61-120">conversationThread</span><span class="sxs-lookup"><span data-stu-id="20e61-120">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="20e61-121">获取属于某个组的特定线程。</span><span class="sxs-lookup"><span data-stu-id="20e61-121">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="20e61-122">更新</span><span class="sxs-lookup"><span data-stu-id="20e61-122">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="20e61-123">conversationThread</span><span class="sxs-lookup"><span data-stu-id="20e61-123">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="20e61-124">更新 conversationThread 对象</span><span class="sxs-lookup"><span data-stu-id="20e61-124">Update conversationThread object.</span></span> |
|[<span data-ttu-id="20e61-125">删除</span><span class="sxs-lookup"><span data-stu-id="20e61-125">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="20e61-126">无</span><span class="sxs-lookup"><span data-stu-id="20e61-126">None</span></span> |<span data-ttu-id="20e61-127">删除 conversationThread 对象</span><span class="sxs-lookup"><span data-stu-id="20e61-127">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="20e61-128">答复</span><span class="sxs-lookup"><span data-stu-id="20e61-128">Reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="20e61-129">无</span><span class="sxs-lookup"><span data-stu-id="20e61-129">None</span></span>|<span data-ttu-id="20e61-130">通过新建 Post 实体答复此线程。</span><span class="sxs-lookup"><span data-stu-id="20e61-130">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="20e61-131">列出帖子</span><span class="sxs-lookup"><span data-stu-id="20e61-131">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="20e61-132">[帖子](post.md) 集合</span><span class="sxs-lookup"><span data-stu-id="20e61-132">[post](post.md) collection</span></span>| <span data-ttu-id="20e61-133">获取指定线程的帖子。</span><span class="sxs-lookup"><span data-stu-id="20e61-133">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="20e61-134">属性</span><span class="sxs-lookup"><span data-stu-id="20e61-134">Properties</span></span>
| <span data-ttu-id="20e61-135">属性</span><span class="sxs-lookup"><span data-stu-id="20e61-135">Property</span></span>     | <span data-ttu-id="20e61-136">类型</span><span class="sxs-lookup"><span data-stu-id="20e61-136">Type</span></span>   |<span data-ttu-id="20e61-137">说明</span><span class="sxs-lookup"><span data-stu-id="20e61-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20e61-138">id</span><span class="sxs-lookup"><span data-stu-id="20e61-138">id</span></span>|<span data-ttu-id="20e61-139">String</span><span class="sxs-lookup"><span data-stu-id="20e61-139">String</span></span>| <span data-ttu-id="20e61-140">只读。</span><span class="sxs-lookup"><span data-stu-id="20e61-140">Read-only.</span></span>|
|<span data-ttu-id="20e61-141">toRecipients</span><span class="sxs-lookup"><span data-stu-id="20e61-141">toRecipients</span></span>|<span data-ttu-id="20e61-142">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="20e61-142">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="20e61-143">收件人：线程的收件人。</span><span class="sxs-lookup"><span data-stu-id="20e61-143">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="20e61-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="20e61-144">ccRecipients</span></span>|<span data-ttu-id="20e61-145">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="20e61-145">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="20e61-146">抄送：线程的收件人。</span><span class="sxs-lookup"><span data-stu-id="20e61-146">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="20e61-147">topic</span><span class="sxs-lookup"><span data-stu-id="20e61-147">topic</span></span>|<span data-ttu-id="20e61-148">String</span><span class="sxs-lookup"><span data-stu-id="20e61-148">String</span></span>|<span data-ttu-id="20e61-p103">对话的主题。在创建对话时可设置此属性，但无法对其进行更新。</span><span class="sxs-lookup"><span data-stu-id="20e61-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="20e61-151">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="20e61-151">hasAttachments</span></span>|<span data-ttu-id="20e61-152">布尔</span><span class="sxs-lookup"><span data-stu-id="20e61-152">Boolean</span></span>|<span data-ttu-id="20e61-153">指示此线程中的任意帖子是否至少具有一个附件。</span><span class="sxs-lookup"><span data-stu-id="20e61-153">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="20e61-154">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="20e61-154">lastDeliveredDateTime</span></span>|<span data-ttu-id="20e61-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20e61-155">DateTimeOffset</span></span>|<span data-ttu-id="20e61-p104">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="20e61-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="20e61-158">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="20e61-158">uniqueSenders</span></span>|<span data-ttu-id="20e61-159">String collection</span><span class="sxs-lookup"><span data-stu-id="20e61-159">String collection</span></span>|<span data-ttu-id="20e61-160">向此线程发送邮件的所有用户。</span><span class="sxs-lookup"><span data-stu-id="20e61-160">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="20e61-161">preview</span><span class="sxs-lookup"><span data-stu-id="20e61-161">preview</span></span>|<span data-ttu-id="20e61-162">String</span><span class="sxs-lookup"><span data-stu-id="20e61-162">String</span></span>|<span data-ttu-id="20e61-163">来自此对话中最新帖子的正文的简短摘要。</span><span class="sxs-lookup"><span data-stu-id="20e61-163">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="20e61-164">isLocked</span><span class="sxs-lookup"><span data-stu-id="20e61-164">isLocked</span></span>|<span data-ttu-id="20e61-165">布尔</span><span class="sxs-lookup"><span data-stu-id="20e61-165">Boolean</span></span>|<span data-ttu-id="20e61-166">指示线程是否已锁定。</span><span class="sxs-lookup"><span data-stu-id="20e61-166">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20e61-167">Relationships</span><span class="sxs-lookup"><span data-stu-id="20e61-167">Relationships</span></span>
| <span data-ttu-id="20e61-168">关系</span><span class="sxs-lookup"><span data-stu-id="20e61-168">Relationship</span></span> | <span data-ttu-id="20e61-169">类型</span><span class="sxs-lookup"><span data-stu-id="20e61-169">Type</span></span>   |<span data-ttu-id="20e61-170">说明</span><span class="sxs-lookup"><span data-stu-id="20e61-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20e61-171">posts</span><span class="sxs-lookup"><span data-stu-id="20e61-171">posts</span></span>|<span data-ttu-id="20e61-172">[帖子](post.md) 集合</span><span class="sxs-lookup"><span data-stu-id="20e61-172">[post](post.md) collection</span></span>| <span data-ttu-id="20e61-p105">只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="20e61-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20e61-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20e61-175">JSON representation</span></span>

<span data-ttu-id="20e61-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20e61-176">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationThread",
  "@odata.annotations": [
    {
      "property": "posts",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": true,
  "id": "string (identifier)",
  "isLocked": true,
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
