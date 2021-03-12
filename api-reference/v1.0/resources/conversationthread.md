---
title: conversationThread 资源类型
description: conversationThread 是 帖子 集合。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: fa9ce48f9b0dd0dd1869a1e31937b70cf4edb975
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720149"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="92a58-103">conversationThread 资源类型</span><span class="sxs-lookup"><span data-stu-id="92a58-103">conversationThread resource type</span></span>

<span data-ttu-id="92a58-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92a58-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92a58-105">conversationThread 是 [帖子](post.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="92a58-105">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="92a58-p101">最后一个帖子收件人集合聚合了整个线程的收件人。线程的收件人集合可以不断扩大。从线程中移除某个收件人时将创建一个新的线程。</span><span class="sxs-lookup"><span data-stu-id="92a58-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="92a58-109">Methods</span><span class="sxs-lookup"><span data-stu-id="92a58-109">Methods</span></span>

| <span data-ttu-id="92a58-110">方法</span><span class="sxs-lookup"><span data-stu-id="92a58-110">Method</span></span>       | <span data-ttu-id="92a58-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="92a58-111">Return Type</span></span>  |<span data-ttu-id="92a58-112">说明</span><span class="sxs-lookup"><span data-stu-id="92a58-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92a58-113">列出线程</span><span class="sxs-lookup"><span data-stu-id="92a58-113">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="92a58-114">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92a58-114">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="92a58-115">获取组的所有线程。</span><span class="sxs-lookup"><span data-stu-id="92a58-115">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="92a58-116">创建线程</span><span class="sxs-lookup"><span data-stu-id="92a58-116">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="92a58-117">conversationThread</span><span class="sxs-lookup"><span data-stu-id="92a58-117">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="92a58-p102">通过首先创建一个线程，启动一个新对话。在组中创建新对话、对话线程和帖子。</span><span class="sxs-lookup"><span data-stu-id="92a58-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="92a58-120">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="92a58-120">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="92a58-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="92a58-121">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="92a58-122">获取属于某个组的特定线程。</span><span class="sxs-lookup"><span data-stu-id="92a58-122">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="92a58-123">更新</span><span class="sxs-lookup"><span data-stu-id="92a58-123">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="92a58-124">conversationThread</span><span class="sxs-lookup"><span data-stu-id="92a58-124">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="92a58-125">更新 conversationThread 对象</span><span class="sxs-lookup"><span data-stu-id="92a58-125">Update conversationThread object.</span></span> |
|[<span data-ttu-id="92a58-126">删除</span><span class="sxs-lookup"><span data-stu-id="92a58-126">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="92a58-127">无</span><span class="sxs-lookup"><span data-stu-id="92a58-127">None</span></span> |<span data-ttu-id="92a58-128">删除 conversationThread 对象</span><span class="sxs-lookup"><span data-stu-id="92a58-128">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="92a58-129">答复</span><span class="sxs-lookup"><span data-stu-id="92a58-129">Reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="92a58-130">无</span><span class="sxs-lookup"><span data-stu-id="92a58-130">None</span></span>|<span data-ttu-id="92a58-131">通过新建 Post 实体答复此线程。</span><span class="sxs-lookup"><span data-stu-id="92a58-131">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="92a58-132">列出帖子</span><span class="sxs-lookup"><span data-stu-id="92a58-132">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="92a58-133">[帖子](post.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92a58-133">[post](post.md) collection</span></span>| <span data-ttu-id="92a58-134">获取指定线程的帖子。</span><span class="sxs-lookup"><span data-stu-id="92a58-134">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="92a58-135">属性</span><span class="sxs-lookup"><span data-stu-id="92a58-135">Properties</span></span>
| <span data-ttu-id="92a58-136">属性</span><span class="sxs-lookup"><span data-stu-id="92a58-136">Property</span></span>              | <span data-ttu-id="92a58-137">类型</span><span class="sxs-lookup"><span data-stu-id="92a58-137">Type</span></span>                                 | <span data-ttu-id="92a58-138">说明</span><span class="sxs-lookup"><span data-stu-id="92a58-138">Description</span></span>                                                                                                                                                                                      |
|:----------------------|:-------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="92a58-139">id</span><span class="sxs-lookup"><span data-stu-id="92a58-139">id</span></span>                    | <span data-ttu-id="92a58-140">字符串</span><span class="sxs-lookup"><span data-stu-id="92a58-140">String</span></span>                               | <span data-ttu-id="92a58-141">只读。</span><span class="sxs-lookup"><span data-stu-id="92a58-141">Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="92a58-142">toRecipients</span><span class="sxs-lookup"><span data-stu-id="92a58-142">toRecipients</span></span>          | <span data-ttu-id="92a58-143">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="92a58-143">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="92a58-144">收件人：线程的收件人。</span><span class="sxs-lookup"><span data-stu-id="92a58-144">The To: recipients for the thread.</span></span>                                                                                                                                                               |
| <span data-ttu-id="92a58-145">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="92a58-145">ccRecipients</span></span>          | <span data-ttu-id="92a58-146">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="92a58-146">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="92a58-147">抄送：线程的收件人。</span><span class="sxs-lookup"><span data-stu-id="92a58-147">The Cc: recipients for the thread.</span></span>                                                                                                                                                               |
| <span data-ttu-id="92a58-148">topic</span><span class="sxs-lookup"><span data-stu-id="92a58-148">topic</span></span>                 | <span data-ttu-id="92a58-149">String</span><span class="sxs-lookup"><span data-stu-id="92a58-149">String</span></span>                               | <span data-ttu-id="92a58-p103">对话的主题。在创建对话时可设置此属性，但无法对其进行更新。</span><span class="sxs-lookup"><span data-stu-id="92a58-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>                                                                              |
| <span data-ttu-id="92a58-152">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="92a58-152">hasAttachments</span></span>        | <span data-ttu-id="92a58-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="92a58-153">Boolean</span></span>                              | <span data-ttu-id="92a58-154">指示此线程中的任意帖子是否至少具有一个附件。</span><span class="sxs-lookup"><span data-stu-id="92a58-154">Indicates whether any of the posts within this thread has at least one attachment.</span></span>                                                                                                               |
| <span data-ttu-id="92a58-155">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="92a58-155">lastDeliveredDateTime</span></span> | <span data-ttu-id="92a58-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92a58-156">DateTimeOffset</span></span>                       | <span data-ttu-id="92a58-157">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="92a58-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="92a58-158">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="92a58-158">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span> |
| <span data-ttu-id="92a58-159">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="92a58-159">uniqueSenders</span></span>         | <span data-ttu-id="92a58-160">String collection</span><span class="sxs-lookup"><span data-stu-id="92a58-160">String collection</span></span>                    | <span data-ttu-id="92a58-161">向此线程发送邮件的所有用户。</span><span class="sxs-lookup"><span data-stu-id="92a58-161">All the users that sent a message to this thread.</span></span>                                                                                                                                                |
| <span data-ttu-id="92a58-162">preview</span><span class="sxs-lookup"><span data-stu-id="92a58-162">preview</span></span>               | <span data-ttu-id="92a58-163">String</span><span class="sxs-lookup"><span data-stu-id="92a58-163">String</span></span>                               | <span data-ttu-id="92a58-164">此对话中最新文章正文的简短摘要。</span><span class="sxs-lookup"><span data-stu-id="92a58-164">A short summary from the body of the latest post in this conversation.</span></span>                                                                                                                           |
| <span data-ttu-id="92a58-165">isLocked</span><span class="sxs-lookup"><span data-stu-id="92a58-165">isLocked</span></span>              | <span data-ttu-id="92a58-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="92a58-166">Boolean</span></span>                              | <span data-ttu-id="92a58-167">指示线程是否已锁定。</span><span class="sxs-lookup"><span data-stu-id="92a58-167">Indicates if the thread is locked.</span></span>                                                                                                                                                               |

## <a name="relationships"></a><span data-ttu-id="92a58-168">关系</span><span class="sxs-lookup"><span data-stu-id="92a58-168">Relationships</span></span>
| <span data-ttu-id="92a58-169">关系</span><span class="sxs-lookup"><span data-stu-id="92a58-169">Relationship</span></span> | <span data-ttu-id="92a58-170">类型</span><span class="sxs-lookup"><span data-stu-id="92a58-170">Type</span></span>   |<span data-ttu-id="92a58-171">说明</span><span class="sxs-lookup"><span data-stu-id="92a58-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92a58-172">posts</span><span class="sxs-lookup"><span data-stu-id="92a58-172">posts</span></span>|<span data-ttu-id="92a58-173">[帖子](post.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92a58-173">[post](post.md) collection</span></span>| <span data-ttu-id="92a58-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="92a58-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92a58-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92a58-176">JSON representation</span></span>

<span data-ttu-id="92a58-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92a58-177">Here is a JSON representation of the resource</span></span>

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

