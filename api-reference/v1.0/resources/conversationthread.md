---
title: conversationThread 资源类型
description: conversationThread 是 帖子 集合。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a8ac7efb08e498b45247119e995aae4c5b1fcb8e
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2020
ms.locfileid: "43511041"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="e4646-103">conversationThread 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4646-103">conversationThread resource type</span></span>

<span data-ttu-id="e4646-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4646-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4646-105">conversationThread 是 [帖子](post.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="e4646-105">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="e4646-p101">最后一个帖子收件人集合聚合了整个线程的收件人。线程的收件人集合可以不断扩大。从线程中移除某个收件人时将创建一个新的线程。</span><span class="sxs-lookup"><span data-stu-id="e4646-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="e4646-109">方法</span><span class="sxs-lookup"><span data-stu-id="e4646-109">Methods</span></span>

| <span data-ttu-id="e4646-110">方法</span><span class="sxs-lookup"><span data-stu-id="e4646-110">Method</span></span>       | <span data-ttu-id="e4646-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="e4646-111">Return Type</span></span>  |<span data-ttu-id="e4646-112">说明</span><span class="sxs-lookup"><span data-stu-id="e4646-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e4646-113">列出线程</span><span class="sxs-lookup"><span data-stu-id="e4646-113">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="e4646-114">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e4646-114">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="e4646-115">获取组的所有线程。</span><span class="sxs-lookup"><span data-stu-id="e4646-115">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="e4646-116">创建线程</span><span class="sxs-lookup"><span data-stu-id="e4646-116">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="e4646-117">conversationThread</span><span class="sxs-lookup"><span data-stu-id="e4646-117">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="e4646-p102">通过首先创建一个线程，启动一个新对话。在组中创建新对话、对话线程和帖子。</span><span class="sxs-lookup"><span data-stu-id="e4646-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="e4646-120">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="e4646-120">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="e4646-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="e4646-121">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="e4646-122">获取属于某个组的特定线程。</span><span class="sxs-lookup"><span data-stu-id="e4646-122">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="e4646-123">更新</span><span class="sxs-lookup"><span data-stu-id="e4646-123">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="e4646-124">conversationThread</span><span class="sxs-lookup"><span data-stu-id="e4646-124">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="e4646-125">更新 conversationThread 对象</span><span class="sxs-lookup"><span data-stu-id="e4646-125">Update conversationThread object.</span></span> |
|[<span data-ttu-id="e4646-126">删除</span><span class="sxs-lookup"><span data-stu-id="e4646-126">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="e4646-127">无</span><span class="sxs-lookup"><span data-stu-id="e4646-127">None</span></span> |<span data-ttu-id="e4646-128">删除 conversationThread 对象</span><span class="sxs-lookup"><span data-stu-id="e4646-128">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="e4646-129">答复</span><span class="sxs-lookup"><span data-stu-id="e4646-129">Reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="e4646-130">无</span><span class="sxs-lookup"><span data-stu-id="e4646-130">None</span></span>|<span data-ttu-id="e4646-131">通过新建 Post 实体答复此线程。</span><span class="sxs-lookup"><span data-stu-id="e4646-131">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="e4646-132">列出帖子</span><span class="sxs-lookup"><span data-stu-id="e4646-132">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="e4646-133">[帖子](post.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e4646-133">[post](post.md) collection</span></span>| <span data-ttu-id="e4646-134">获取指定线程的帖子。</span><span class="sxs-lookup"><span data-stu-id="e4646-134">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="e4646-135">属性</span><span class="sxs-lookup"><span data-stu-id="e4646-135">Properties</span></span>
| <span data-ttu-id="e4646-136">属性</span><span class="sxs-lookup"><span data-stu-id="e4646-136">Property</span></span>     | <span data-ttu-id="e4646-137">类型</span><span class="sxs-lookup"><span data-stu-id="e4646-137">Type</span></span>   |<span data-ttu-id="e4646-138">说明</span><span class="sxs-lookup"><span data-stu-id="e4646-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4646-139">id</span><span class="sxs-lookup"><span data-stu-id="e4646-139">id</span></span>|<span data-ttu-id="e4646-140">String</span><span class="sxs-lookup"><span data-stu-id="e4646-140">String</span></span>| <span data-ttu-id="e4646-141">只读。</span><span class="sxs-lookup"><span data-stu-id="e4646-141">Read-only.</span></span>|
|<span data-ttu-id="e4646-142">toRecipients</span><span class="sxs-lookup"><span data-stu-id="e4646-142">toRecipients</span></span>|<span data-ttu-id="e4646-143">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="e4646-143">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="e4646-144">收件人：线程的收件人。</span><span class="sxs-lookup"><span data-stu-id="e4646-144">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="e4646-145">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="e4646-145">ccRecipients</span></span>|<span data-ttu-id="e4646-146">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="e4646-146">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="e4646-147">抄送：线程的收件人。</span><span class="sxs-lookup"><span data-stu-id="e4646-147">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="e4646-148">topic</span><span class="sxs-lookup"><span data-stu-id="e4646-148">topic</span></span>|<span data-ttu-id="e4646-149">String</span><span class="sxs-lookup"><span data-stu-id="e4646-149">String</span></span>|<span data-ttu-id="e4646-p103">对话的主题。在创建对话时可设置此属性，但无法对其进行更新。</span><span class="sxs-lookup"><span data-stu-id="e4646-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="e4646-152">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="e4646-152">hasAttachments</span></span>|<span data-ttu-id="e4646-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4646-153">Boolean</span></span>|<span data-ttu-id="e4646-154">指示此线程中的任意帖子是否至少具有一个附件。</span><span class="sxs-lookup"><span data-stu-id="e4646-154">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="e4646-155">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="e4646-155">lastDeliveredDateTime</span></span>|<span data-ttu-id="e4646-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4646-156">DateTimeOffset</span></span>|<span data-ttu-id="e4646-p104">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e4646-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e4646-159">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="e4646-159">uniqueSenders</span></span>|<span data-ttu-id="e4646-160">String collection</span><span class="sxs-lookup"><span data-stu-id="e4646-160">String collection</span></span>|<span data-ttu-id="e4646-161">向此线程发送邮件的所有用户。</span><span class="sxs-lookup"><span data-stu-id="e4646-161">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="e4646-162">preview</span><span class="sxs-lookup"><span data-stu-id="e4646-162">preview</span></span>|<span data-ttu-id="e4646-163">String</span><span class="sxs-lookup"><span data-stu-id="e4646-163">String</span></span>|<span data-ttu-id="e4646-164">来自此对话中最新帖子的正文的简短摘要。</span><span class="sxs-lookup"><span data-stu-id="e4646-164">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="e4646-165">Resource.islocked</span><span class="sxs-lookup"><span data-stu-id="e4646-165">isLocked</span></span>|<span data-ttu-id="e4646-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4646-166">Boolean</span></span>|<span data-ttu-id="e4646-167">指示线程是否已锁定。</span><span class="sxs-lookup"><span data-stu-id="e4646-167">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4646-168">关系</span><span class="sxs-lookup"><span data-stu-id="e4646-168">Relationships</span></span>
| <span data-ttu-id="e4646-169">关系</span><span class="sxs-lookup"><span data-stu-id="e4646-169">Relationship</span></span> | <span data-ttu-id="e4646-170">类型</span><span class="sxs-lookup"><span data-stu-id="e4646-170">Type</span></span>   |<span data-ttu-id="e4646-171">说明</span><span class="sxs-lookup"><span data-stu-id="e4646-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4646-172">posts</span><span class="sxs-lookup"><span data-stu-id="e4646-172">posts</span></span>|<span data-ttu-id="e4646-173">[帖子](post.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e4646-173">[post](post.md) collection</span></span>| <span data-ttu-id="e4646-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="e4646-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4646-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4646-176">JSON representation</span></span>

<span data-ttu-id="e4646-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4646-177">Here is a JSON representation of the resource</span></span>

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
