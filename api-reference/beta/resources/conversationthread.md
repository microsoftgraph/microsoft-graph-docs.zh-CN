---
title: conversationThread 资源类型
description: conversationThread 是 帖子 集合。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b9e06ddb7a4a92905612d0975d719700c4cc90b6
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721661"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="67a1d-103">conversationThread 资源类型</span><span class="sxs-lookup"><span data-stu-id="67a1d-103">conversationThread resource type</span></span>

<span data-ttu-id="67a1d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67a1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67a1d-105">conversationThread 是 [帖子](post.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="67a1d-105">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="67a1d-p101">最后一个帖子收件人集合聚合了整个线程的收件人。线程的收件人集合可以不断扩大。从线程中移除某个收件人时将创建一个新的线程。</span><span class="sxs-lookup"><span data-stu-id="67a1d-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="67a1d-109">方法</span><span class="sxs-lookup"><span data-stu-id="67a1d-109">Methods</span></span>

| <span data-ttu-id="67a1d-110">方法</span><span class="sxs-lookup"><span data-stu-id="67a1d-110">Method</span></span>       | <span data-ttu-id="67a1d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="67a1d-111">Return Type</span></span>  |<span data-ttu-id="67a1d-112">说明</span><span class="sxs-lookup"><span data-stu-id="67a1d-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="67a1d-113">列出线程</span><span class="sxs-lookup"><span data-stu-id="67a1d-113">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="67a1d-114">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67a1d-114">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="67a1d-115">获取组的所有线程。</span><span class="sxs-lookup"><span data-stu-id="67a1d-115">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="67a1d-116">创建线程</span><span class="sxs-lookup"><span data-stu-id="67a1d-116">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="67a1d-117">conversationThread</span><span class="sxs-lookup"><span data-stu-id="67a1d-117">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="67a1d-p102">通过首先创建一个线程，启动一个新对话。在组中创建新对话、对话线程和帖子。</span><span class="sxs-lookup"><span data-stu-id="67a1d-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="67a1d-120">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="67a1d-120">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="67a1d-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="67a1d-121">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="67a1d-122">获取属于某个组的特定线程。</span><span class="sxs-lookup"><span data-stu-id="67a1d-122">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="67a1d-123">更新</span><span class="sxs-lookup"><span data-stu-id="67a1d-123">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="67a1d-124">conversationThread</span><span class="sxs-lookup"><span data-stu-id="67a1d-124">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="67a1d-125">更新 conversationThread 对象</span><span class="sxs-lookup"><span data-stu-id="67a1d-125">Update conversationThread object.</span></span> |
|[<span data-ttu-id="67a1d-126">删除</span><span class="sxs-lookup"><span data-stu-id="67a1d-126">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="67a1d-127">无</span><span class="sxs-lookup"><span data-stu-id="67a1d-127">None</span></span> |<span data-ttu-id="67a1d-128">删除 conversationThread 对象</span><span class="sxs-lookup"><span data-stu-id="67a1d-128">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="67a1d-129">回复</span><span class="sxs-lookup"><span data-stu-id="67a1d-129">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="67a1d-130">无</span><span class="sxs-lookup"><span data-stu-id="67a1d-130">None</span></span>|<span data-ttu-id="67a1d-131">通过新建 Post 实体答复此线程。</span><span class="sxs-lookup"><span data-stu-id="67a1d-131">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="67a1d-132">列出帖子</span><span class="sxs-lookup"><span data-stu-id="67a1d-132">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="67a1d-133">[帖子](post.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67a1d-133">[post](post.md) collection</span></span>| <span data-ttu-id="67a1d-134">获取指定线程的帖子。</span><span class="sxs-lookup"><span data-stu-id="67a1d-134">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="67a1d-135">属性</span><span class="sxs-lookup"><span data-stu-id="67a1d-135">Properties</span></span>
| <span data-ttu-id="67a1d-136">属性</span><span class="sxs-lookup"><span data-stu-id="67a1d-136">Property</span></span>              | <span data-ttu-id="67a1d-137">类型</span><span class="sxs-lookup"><span data-stu-id="67a1d-137">Type</span></span>                                 | <span data-ttu-id="67a1d-138">说明</span><span class="sxs-lookup"><span data-stu-id="67a1d-138">Description</span></span>                                                                                                                                                                                      |
|:----------------------|:-------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="67a1d-139">id</span><span class="sxs-lookup"><span data-stu-id="67a1d-139">id</span></span>                    | <span data-ttu-id="67a1d-140">String</span><span class="sxs-lookup"><span data-stu-id="67a1d-140">String</span></span>                               | <span data-ttu-id="67a1d-141">只读。</span><span class="sxs-lookup"><span data-stu-id="67a1d-141">Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="67a1d-142">toRecipients</span><span class="sxs-lookup"><span data-stu-id="67a1d-142">toRecipients</span></span>          | <span data-ttu-id="67a1d-143">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="67a1d-143">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="67a1d-144">收件人：线程的收件人。</span><span class="sxs-lookup"><span data-stu-id="67a1d-144">The To: recipients for the thread.</span></span>                                                                                                                                                               |
| <span data-ttu-id="67a1d-145">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="67a1d-145">ccRecipients</span></span>          | <span data-ttu-id="67a1d-146">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="67a1d-146">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="67a1d-147">抄送：线程的收件人。</span><span class="sxs-lookup"><span data-stu-id="67a1d-147">The Cc: recipients for the thread.</span></span>                                                                                                                                                               |
| <span data-ttu-id="67a1d-148">topic</span><span class="sxs-lookup"><span data-stu-id="67a1d-148">topic</span></span>                 | <span data-ttu-id="67a1d-149">String</span><span class="sxs-lookup"><span data-stu-id="67a1d-149">String</span></span>                               | <span data-ttu-id="67a1d-p103">对话的主题。在创建对话时可设置此属性，但无法对其进行更新。</span><span class="sxs-lookup"><span data-stu-id="67a1d-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>                                                                              |
| <span data-ttu-id="67a1d-152">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="67a1d-152">hasAttachments</span></span>        | <span data-ttu-id="67a1d-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a1d-153">Boolean</span></span>                              | <span data-ttu-id="67a1d-154">指示此线程中的任意帖子是否至少具有一个附件。</span><span class="sxs-lookup"><span data-stu-id="67a1d-154">Indicates whether any of the posts within this thread has at least one attachment.</span></span>                                                                                                               |
| <span data-ttu-id="67a1d-155">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="67a1d-155">lastDeliveredDateTime</span></span> | <span data-ttu-id="67a1d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67a1d-156">DateTimeOffset</span></span>                       | <span data-ttu-id="67a1d-157">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="67a1d-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="67a1d-158">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="67a1d-158">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span> |
| <span data-ttu-id="67a1d-159">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="67a1d-159">uniqueSenders</span></span>         | <span data-ttu-id="67a1d-160">String collection</span><span class="sxs-lookup"><span data-stu-id="67a1d-160">String collection</span></span>                    | <span data-ttu-id="67a1d-161">向此线程发送邮件的所有用户。</span><span class="sxs-lookup"><span data-stu-id="67a1d-161">All the users that sent a message to this thread.</span></span>                                                                                                                                                |
| <span data-ttu-id="67a1d-162">preview</span><span class="sxs-lookup"><span data-stu-id="67a1d-162">preview</span></span>               | <span data-ttu-id="67a1d-163">String</span><span class="sxs-lookup"><span data-stu-id="67a1d-163">String</span></span>                               | <span data-ttu-id="67a1d-164">此对话中最新文章正文的简短摘要。</span><span class="sxs-lookup"><span data-stu-id="67a1d-164">A short summary from the body of the latest post in this conversation.</span></span>                                                                                                                           |
| <span data-ttu-id="67a1d-165">isLocked</span><span class="sxs-lookup"><span data-stu-id="67a1d-165">isLocked</span></span>              | <span data-ttu-id="67a1d-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a1d-166">Boolean</span></span>                              | <span data-ttu-id="67a1d-167">指示线程是否已锁定。</span><span class="sxs-lookup"><span data-stu-id="67a1d-167">Indicates if the thread is locked.</span></span>                                                                                                                                                               |

## <a name="relationships"></a><span data-ttu-id="67a1d-168">关系</span><span class="sxs-lookup"><span data-stu-id="67a1d-168">Relationships</span></span>
| <span data-ttu-id="67a1d-169">关系</span><span class="sxs-lookup"><span data-stu-id="67a1d-169">Relationship</span></span> | <span data-ttu-id="67a1d-170">类型</span><span class="sxs-lookup"><span data-stu-id="67a1d-170">Type</span></span>   |<span data-ttu-id="67a1d-171">说明</span><span class="sxs-lookup"><span data-stu-id="67a1d-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67a1d-172">posts</span><span class="sxs-lookup"><span data-stu-id="67a1d-172">posts</span></span>|<span data-ttu-id="67a1d-173">[帖子](post.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67a1d-173">[post](post.md) collection</span></span>| <span data-ttu-id="67a1d-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="67a1d-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67a1d-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67a1d-176">JSON representation</span></span>

<span data-ttu-id="67a1d-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67a1d-177">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationThread"
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
<!--
{
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


