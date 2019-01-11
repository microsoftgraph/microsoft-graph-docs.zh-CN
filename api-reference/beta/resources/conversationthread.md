---
title: conversationThread 资源类型
description: conversationThread 是 帖子 集合。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 1101bb56e69b6418cfd57e719cf1633fa76b161c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845267"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="eac1e-103">conversationThread 资源类型</span><span class="sxs-lookup"><span data-stu-id="eac1e-103">conversationThread resource type</span></span>

> <span data-ttu-id="eac1e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eac1e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eac1e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eac1e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eac1e-106">conversationThread 是 [帖子](post.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="eac1e-106">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="eac1e-p102">最后一个帖子收件人集合聚合了整个线程的收件人。线程的收件人集合可以不断扩大。从线程中移除某个收件人时将创建一个新的线程。</span><span class="sxs-lookup"><span data-stu-id="eac1e-p102">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="eac1e-110">方法</span><span class="sxs-lookup"><span data-stu-id="eac1e-110">Methods</span></span>

| <span data-ttu-id="eac1e-111">方法</span><span class="sxs-lookup"><span data-stu-id="eac1e-111">Method</span></span>       | <span data-ttu-id="eac1e-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="eac1e-112">Return Type</span></span>  |<span data-ttu-id="eac1e-113">说明</span><span class="sxs-lookup"><span data-stu-id="eac1e-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eac1e-114">列出线程</span><span class="sxs-lookup"><span data-stu-id="eac1e-114">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="eac1e-115">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eac1e-115">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="eac1e-116">获取某个组的所有线程。</span><span class="sxs-lookup"><span data-stu-id="eac1e-116">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="eac1e-117">创建线程</span><span class="sxs-lookup"><span data-stu-id="eac1e-117">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="eac1e-118">conversationThread</span><span class="sxs-lookup"><span data-stu-id="eac1e-118">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="eac1e-p103">通过首先创建一个线程，启动一个新对话。在组中创建新对话、对话线程和帖子。</span><span class="sxs-lookup"><span data-stu-id="eac1e-p103">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="eac1e-121">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="eac1e-121">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="eac1e-122">conversationThread</span><span class="sxs-lookup"><span data-stu-id="eac1e-122">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="eac1e-123">获取属于某个组的特定线程。</span><span class="sxs-lookup"><span data-stu-id="eac1e-123">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="eac1e-124">更新</span><span class="sxs-lookup"><span data-stu-id="eac1e-124">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="eac1e-125">conversationThread</span><span class="sxs-lookup"><span data-stu-id="eac1e-125">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="eac1e-126">更新 conversationThread 对象</span><span class="sxs-lookup"><span data-stu-id="eac1e-126">Update conversationThread object.</span></span> |
|[<span data-ttu-id="eac1e-127">删除</span><span class="sxs-lookup"><span data-stu-id="eac1e-127">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="eac1e-128">无</span><span class="sxs-lookup"><span data-stu-id="eac1e-128">None</span></span> |<span data-ttu-id="eac1e-129">删除 conversationThread 对象</span><span class="sxs-lookup"><span data-stu-id="eac1e-129">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="eac1e-130">回复</span><span class="sxs-lookup"><span data-stu-id="eac1e-130">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="eac1e-131">无</span><span class="sxs-lookup"><span data-stu-id="eac1e-131">None</span></span>|<span data-ttu-id="eac1e-132">通过新建 Post 实体答复此线程。</span><span class="sxs-lookup"><span data-stu-id="eac1e-132">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="eac1e-133">列出帖子</span><span class="sxs-lookup"><span data-stu-id="eac1e-133">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="eac1e-134">[帖子](post.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eac1e-134">[post](post.md) collection</span></span>| <span data-ttu-id="eac1e-135">获取指定线程的帖子。</span><span class="sxs-lookup"><span data-stu-id="eac1e-135">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="eac1e-136">属性</span><span class="sxs-lookup"><span data-stu-id="eac1e-136">Properties</span></span>
| <span data-ttu-id="eac1e-137">属性</span><span class="sxs-lookup"><span data-stu-id="eac1e-137">Property</span></span>     | <span data-ttu-id="eac1e-138">类型</span><span class="sxs-lookup"><span data-stu-id="eac1e-138">Type</span></span>   |<span data-ttu-id="eac1e-139">说明</span><span class="sxs-lookup"><span data-stu-id="eac1e-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eac1e-140">id</span><span class="sxs-lookup"><span data-stu-id="eac1e-140">id</span></span>|<span data-ttu-id="eac1e-141">String</span><span class="sxs-lookup"><span data-stu-id="eac1e-141">String</span></span>| <span data-ttu-id="eac1e-142">只读。</span><span class="sxs-lookup"><span data-stu-id="eac1e-142">Read-only.</span></span>|
|<span data-ttu-id="eac1e-143">toRecipients</span><span class="sxs-lookup"><span data-stu-id="eac1e-143">toRecipients</span></span>|<span data-ttu-id="eac1e-144">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="eac1e-144">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="eac1e-145">收件人：线程的收件人。</span><span class="sxs-lookup"><span data-stu-id="eac1e-145">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="eac1e-146">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="eac1e-146">ccRecipients</span></span>|<span data-ttu-id="eac1e-147">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="eac1e-147">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="eac1e-148">抄送：线程的收件人。</span><span class="sxs-lookup"><span data-stu-id="eac1e-148">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="eac1e-149">topic</span><span class="sxs-lookup"><span data-stu-id="eac1e-149">topic</span></span>|<span data-ttu-id="eac1e-150">String</span><span class="sxs-lookup"><span data-stu-id="eac1e-150">String</span></span>|<span data-ttu-id="eac1e-p104">对话的主题。在创建对话时可设置此属性，但无法对其进行更新。</span><span class="sxs-lookup"><span data-stu-id="eac1e-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="eac1e-153">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="eac1e-153">hasAttachments</span></span>|<span data-ttu-id="eac1e-154">布尔</span><span class="sxs-lookup"><span data-stu-id="eac1e-154">Boolean</span></span>|<span data-ttu-id="eac1e-155">指示此线程中的任意帖子是否至少具有一个附件。</span><span class="sxs-lookup"><span data-stu-id="eac1e-155">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="eac1e-156">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="eac1e-156">lastDeliveredDateTime</span></span>|<span data-ttu-id="eac1e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eac1e-157">DateTimeOffset</span></span>|<span data-ttu-id="eac1e-p105">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="eac1e-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="eac1e-160">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="eac1e-160">uniqueSenders</span></span>|<span data-ttu-id="eac1e-161">String collection</span><span class="sxs-lookup"><span data-stu-id="eac1e-161">String collection</span></span>|<span data-ttu-id="eac1e-162">向此线程发送邮件的所有用户。</span><span class="sxs-lookup"><span data-stu-id="eac1e-162">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="eac1e-163">preview</span><span class="sxs-lookup"><span data-stu-id="eac1e-163">preview</span></span>|<span data-ttu-id="eac1e-164">String</span><span class="sxs-lookup"><span data-stu-id="eac1e-164">String</span></span>|<span data-ttu-id="eac1e-165">来自此对话中最新帖子的正文的简短摘要。</span><span class="sxs-lookup"><span data-stu-id="eac1e-165">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="eac1e-166">isLocked</span><span class="sxs-lookup"><span data-stu-id="eac1e-166">isLocked</span></span>|<span data-ttu-id="eac1e-167">布尔</span><span class="sxs-lookup"><span data-stu-id="eac1e-167">Boolean</span></span>|<span data-ttu-id="eac1e-168">指示线程是否已锁定。</span><span class="sxs-lookup"><span data-stu-id="eac1e-168">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eac1e-169">Relationships</span><span class="sxs-lookup"><span data-stu-id="eac1e-169">Relationships</span></span>
| <span data-ttu-id="eac1e-170">关系</span><span class="sxs-lookup"><span data-stu-id="eac1e-170">Relationship</span></span> | <span data-ttu-id="eac1e-171">类型</span><span class="sxs-lookup"><span data-stu-id="eac1e-171">Type</span></span>   |<span data-ttu-id="eac1e-172">说明</span><span class="sxs-lookup"><span data-stu-id="eac1e-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eac1e-173">posts</span><span class="sxs-lookup"><span data-stu-id="eac1e-173">posts</span></span>|<span data-ttu-id="eac1e-174">[帖子](post.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eac1e-174">[post](post.md) collection</span></span>| <span data-ttu-id="eac1e-p106">只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="eac1e-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eac1e-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eac1e-177">JSON representation</span></span>

<span data-ttu-id="eac1e-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eac1e-178">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
