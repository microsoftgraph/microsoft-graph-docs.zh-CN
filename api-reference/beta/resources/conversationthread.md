---
title: conversationThread 资源类型
description: conversationThread 是 帖子 集合。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 504b8b8d4e47f892da72ea7ef9588491d0642f21
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508172"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="524bc-103">conversationThread 资源类型</span><span class="sxs-lookup"><span data-stu-id="524bc-103">conversationThread resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="524bc-104">conversationThread 是 [帖子](post.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="524bc-104">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="524bc-p101">最后一个帖子收件人集合聚合了整个线程的收件人。线程的收件人集合可以不断扩大。从线程中移除某个收件人时将创建一个新的线程。</span><span class="sxs-lookup"><span data-stu-id="524bc-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="524bc-108">方法</span><span class="sxs-lookup"><span data-stu-id="524bc-108">Methods</span></span>

| <span data-ttu-id="524bc-109">方法</span><span class="sxs-lookup"><span data-stu-id="524bc-109">Method</span></span>       | <span data-ttu-id="524bc-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="524bc-110">Return Type</span></span>  |<span data-ttu-id="524bc-111">说明</span><span class="sxs-lookup"><span data-stu-id="524bc-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="524bc-112">列出线程</span><span class="sxs-lookup"><span data-stu-id="524bc-112">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="524bc-113">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="524bc-113">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="524bc-114">获取某个组的所有线程。</span><span class="sxs-lookup"><span data-stu-id="524bc-114">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="524bc-115">创建线程</span><span class="sxs-lookup"><span data-stu-id="524bc-115">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="524bc-116">conversationThread</span><span class="sxs-lookup"><span data-stu-id="524bc-116">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="524bc-p102">通过首先创建一个线程，启动一个新对话。在组中创建新对话、对话线程和帖子。</span><span class="sxs-lookup"><span data-stu-id="524bc-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="524bc-119">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="524bc-119">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="524bc-120">conversationThread</span><span class="sxs-lookup"><span data-stu-id="524bc-120">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="524bc-121">获取属于某个组的特定线程。</span><span class="sxs-lookup"><span data-stu-id="524bc-121">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="524bc-122">更新</span><span class="sxs-lookup"><span data-stu-id="524bc-122">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="524bc-123">conversationThread</span><span class="sxs-lookup"><span data-stu-id="524bc-123">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="524bc-124">更新 conversationThread 对象</span><span class="sxs-lookup"><span data-stu-id="524bc-124">Update conversationThread object.</span></span> |
|[<span data-ttu-id="524bc-125">删除</span><span class="sxs-lookup"><span data-stu-id="524bc-125">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="524bc-126">None</span><span class="sxs-lookup"><span data-stu-id="524bc-126">None</span></span> |<span data-ttu-id="524bc-127">删除 conversationThread 对象</span><span class="sxs-lookup"><span data-stu-id="524bc-127">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="524bc-128">回复</span><span class="sxs-lookup"><span data-stu-id="524bc-128">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="524bc-129">无</span><span class="sxs-lookup"><span data-stu-id="524bc-129">None</span></span>|<span data-ttu-id="524bc-130">通过新建 Post 实体答复此线程。</span><span class="sxs-lookup"><span data-stu-id="524bc-130">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="524bc-131">列出帖子</span><span class="sxs-lookup"><span data-stu-id="524bc-131">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="524bc-132">[帖子](post.md) 集合</span><span class="sxs-lookup"><span data-stu-id="524bc-132">[post](post.md) collection</span></span>| <span data-ttu-id="524bc-133">获取指定线程的帖子。</span><span class="sxs-lookup"><span data-stu-id="524bc-133">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="524bc-134">属性</span><span class="sxs-lookup"><span data-stu-id="524bc-134">Properties</span></span>
| <span data-ttu-id="524bc-135">属性</span><span class="sxs-lookup"><span data-stu-id="524bc-135">Property</span></span>     | <span data-ttu-id="524bc-136">类型</span><span class="sxs-lookup"><span data-stu-id="524bc-136">Type</span></span>   |<span data-ttu-id="524bc-137">说明</span><span class="sxs-lookup"><span data-stu-id="524bc-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="524bc-138">id</span><span class="sxs-lookup"><span data-stu-id="524bc-138">id</span></span>|<span data-ttu-id="524bc-139">String</span><span class="sxs-lookup"><span data-stu-id="524bc-139">String</span></span>| <span data-ttu-id="524bc-140">只读。</span><span class="sxs-lookup"><span data-stu-id="524bc-140">Read-only.</span></span>|
|<span data-ttu-id="524bc-141">toRecipients</span><span class="sxs-lookup"><span data-stu-id="524bc-141">toRecipients</span></span>|<span data-ttu-id="524bc-142">[收件人](recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="524bc-142">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="524bc-143">收件人：线程的收件人。</span><span class="sxs-lookup"><span data-stu-id="524bc-143">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="524bc-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="524bc-144">ccRecipients</span></span>|<span data-ttu-id="524bc-145">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="524bc-145">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="524bc-146">抄送：线程的收件人。</span><span class="sxs-lookup"><span data-stu-id="524bc-146">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="524bc-147">topic</span><span class="sxs-lookup"><span data-stu-id="524bc-147">topic</span></span>|<span data-ttu-id="524bc-148">String</span><span class="sxs-lookup"><span data-stu-id="524bc-148">String</span></span>|<span data-ttu-id="524bc-p103">对话的主题。在创建对话时可设置此属性，但无法对其进行更新。</span><span class="sxs-lookup"><span data-stu-id="524bc-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="524bc-151">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="524bc-151">hasAttachments</span></span>|<span data-ttu-id="524bc-152">布尔</span><span class="sxs-lookup"><span data-stu-id="524bc-152">Boolean</span></span>|<span data-ttu-id="524bc-153">指示此线程中的任意帖子是否至少具有一个附件。</span><span class="sxs-lookup"><span data-stu-id="524bc-153">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="524bc-154">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="524bc-154">lastDeliveredDateTime</span></span>|<span data-ttu-id="524bc-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="524bc-155">DateTimeOffset</span></span>|<span data-ttu-id="524bc-p104">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="524bc-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="524bc-158">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="524bc-158">uniqueSenders</span></span>|<span data-ttu-id="524bc-159">String collection</span><span class="sxs-lookup"><span data-stu-id="524bc-159">String collection</span></span>|<span data-ttu-id="524bc-160">向此线程发送邮件的所有用户。</span><span class="sxs-lookup"><span data-stu-id="524bc-160">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="524bc-161">preview</span><span class="sxs-lookup"><span data-stu-id="524bc-161">preview</span></span>|<span data-ttu-id="524bc-162">String</span><span class="sxs-lookup"><span data-stu-id="524bc-162">String</span></span>|<span data-ttu-id="524bc-163">来自此对话中最新帖子的正文的简短摘要。</span><span class="sxs-lookup"><span data-stu-id="524bc-163">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="524bc-164">isLocked</span><span class="sxs-lookup"><span data-stu-id="524bc-164">isLocked</span></span>|<span data-ttu-id="524bc-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="524bc-165">Boolean</span></span>|<span data-ttu-id="524bc-166">指示线程是否已锁定。</span><span class="sxs-lookup"><span data-stu-id="524bc-166">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="524bc-167">关系</span><span class="sxs-lookup"><span data-stu-id="524bc-167">Relationships</span></span>
| <span data-ttu-id="524bc-168">关系</span><span class="sxs-lookup"><span data-stu-id="524bc-168">Relationship</span></span> | <span data-ttu-id="524bc-169">类型</span><span class="sxs-lookup"><span data-stu-id="524bc-169">Type</span></span>   |<span data-ttu-id="524bc-170">说明</span><span class="sxs-lookup"><span data-stu-id="524bc-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="524bc-171">posts</span><span class="sxs-lookup"><span data-stu-id="524bc-171">posts</span></span>|<span data-ttu-id="524bc-172">[帖子](post.md) 集合</span><span class="sxs-lookup"><span data-stu-id="524bc-172">[post](post.md) collection</span></span>| <span data-ttu-id="524bc-p105">只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="524bc-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="524bc-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="524bc-175">JSON representation</span></span>

<span data-ttu-id="524bc-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="524bc-176">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/conversationthread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
