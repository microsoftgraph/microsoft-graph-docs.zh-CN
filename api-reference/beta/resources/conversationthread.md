---
title: conversationThread 资源类型
description: conversationThread 是 帖子 集合。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: d1b274aa84299ae66d6385133ed7371a377d01e6
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845937"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="4f374-103">conversationThread 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f374-103">conversationThread resource type</span></span>

<span data-ttu-id="4f374-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f374-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f374-105">conversationThread 是 [帖子](post.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="4f374-105">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="4f374-106">The last post's recipients collection is the aggregated recipients of the entire thread.</span><span class="sxs-lookup"><span data-stu-id="4f374-106">The last post's recipients collection is the aggregated recipients of the entire thread.</span></span> <span data-ttu-id="4f374-107">A thread can have a growing collection of recipients.</span><span class="sxs-lookup"><span data-stu-id="4f374-107">A thread can have a growing collection of recipients.</span></span>
<span data-ttu-id="4f374-108">A new thread is created when a recipient is removed from the thread.</span><span class="sxs-lookup"><span data-stu-id="4f374-108">A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="4f374-109">Methods</span><span class="sxs-lookup"><span data-stu-id="4f374-109">Methods</span></span>

| <span data-ttu-id="4f374-110">方法</span><span class="sxs-lookup"><span data-stu-id="4f374-110">Method</span></span>       | <span data-ttu-id="4f374-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f374-111">Return Type</span></span>  |<span data-ttu-id="4f374-112">说明</span><span class="sxs-lookup"><span data-stu-id="4f374-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4f374-113">列出线程</span><span class="sxs-lookup"><span data-stu-id="4f374-113">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="4f374-114">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f374-114">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="4f374-115">获取组的所有线程。</span><span class="sxs-lookup"><span data-stu-id="4f374-115">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="4f374-116">创建线程</span><span class="sxs-lookup"><span data-stu-id="4f374-116">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="4f374-117">conversationThread</span><span class="sxs-lookup"><span data-stu-id="4f374-117">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="4f374-118">Start a new conversation by first creating a thread.</span><span class="sxs-lookup"><span data-stu-id="4f374-118">Start a new conversation by first creating a thread.</span></span> <span data-ttu-id="4f374-119">A new conversation, conversation thread, and post are created in the group.</span><span class="sxs-lookup"><span data-stu-id="4f374-119">A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="4f374-120">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="4f374-120">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="4f374-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="4f374-121">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="4f374-122">获取属于某个组的特定线程。</span><span class="sxs-lookup"><span data-stu-id="4f374-122">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="4f374-123">更新</span><span class="sxs-lookup"><span data-stu-id="4f374-123">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="4f374-124">conversationThread</span><span class="sxs-lookup"><span data-stu-id="4f374-124">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="4f374-125">更新 conversationThread 对象</span><span class="sxs-lookup"><span data-stu-id="4f374-125">Update conversationThread object.</span></span> |
|[<span data-ttu-id="4f374-126">删除</span><span class="sxs-lookup"><span data-stu-id="4f374-126">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="4f374-127">None</span><span class="sxs-lookup"><span data-stu-id="4f374-127">None</span></span> |<span data-ttu-id="4f374-128">删除 conversationThread 对象</span><span class="sxs-lookup"><span data-stu-id="4f374-128">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="4f374-129">回复</span><span class="sxs-lookup"><span data-stu-id="4f374-129">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="4f374-130">无</span><span class="sxs-lookup"><span data-stu-id="4f374-130">None</span></span>|<span data-ttu-id="4f374-131">通过新建 Post 实体答复此线程。</span><span class="sxs-lookup"><span data-stu-id="4f374-131">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="4f374-132">列出帖子</span><span class="sxs-lookup"><span data-stu-id="4f374-132">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="4f374-133">[帖子](post.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f374-133">[post](post.md) collection</span></span>| <span data-ttu-id="4f374-134">获取指定线程的帖子。</span><span class="sxs-lookup"><span data-stu-id="4f374-134">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="4f374-135">属性</span><span class="sxs-lookup"><span data-stu-id="4f374-135">Properties</span></span>
| <span data-ttu-id="4f374-136">属性</span><span class="sxs-lookup"><span data-stu-id="4f374-136">Property</span></span>              | <span data-ttu-id="4f374-137">类型</span><span class="sxs-lookup"><span data-stu-id="4f374-137">Type</span></span>                                 | <span data-ttu-id="4f374-138">说明</span><span class="sxs-lookup"><span data-stu-id="4f374-138">Description</span></span>                                                                                                                                                                                      |
|:----------------------|:-------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4f374-139">id</span><span class="sxs-lookup"><span data-stu-id="4f374-139">id</span></span>                    | <span data-ttu-id="4f374-140">String</span><span class="sxs-lookup"><span data-stu-id="4f374-140">String</span></span>                               | <span data-ttu-id="4f374-141">只读。</span><span class="sxs-lookup"><span data-stu-id="4f374-141">Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="4f374-142">toRecipients</span><span class="sxs-lookup"><span data-stu-id="4f374-142">toRecipients</span></span>          | <span data-ttu-id="4f374-143">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="4f374-143">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="4f374-144">收件人：线程的收件人。</span><span class="sxs-lookup"><span data-stu-id="4f374-144">The To: recipients for the thread.</span></span>                                                                                                                                                               |
| <span data-ttu-id="4f374-145">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="4f374-145">ccRecipients</span></span>          | <span data-ttu-id="4f374-146">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="4f374-146">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="4f374-147">抄送：线程的收件人。</span><span class="sxs-lookup"><span data-stu-id="4f374-147">The Cc: recipients for the thread.</span></span>                                                                                                                                                               |
| <span data-ttu-id="4f374-148">topic</span><span class="sxs-lookup"><span data-stu-id="4f374-148">topic</span></span>                 | <span data-ttu-id="4f374-149">String</span><span class="sxs-lookup"><span data-stu-id="4f374-149">String</span></span>                               | <span data-ttu-id="4f374-150">The topic of the conversation.</span><span class="sxs-lookup"><span data-stu-id="4f374-150">The topic of the conversation.</span></span> <span data-ttu-id="4f374-151">This property can be set when the conversation is created, but it cannot be updated.</span><span class="sxs-lookup"><span data-stu-id="4f374-151">This property can be set when the conversation is created, but it cannot be updated.</span></span>                                                                              |
| <span data-ttu-id="4f374-152">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="4f374-152">hasAttachments</span></span>        | <span data-ttu-id="4f374-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f374-153">Boolean</span></span>                              | <span data-ttu-id="4f374-154">指示此线程中的任意帖子是否至少具有一个附件。</span><span class="sxs-lookup"><span data-stu-id="4f374-154">Indicates whether any of the posts within this thread has at least one attachment.</span></span>                                                                                                               |
| <span data-ttu-id="4f374-155">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="4f374-155">lastDeliveredDateTime</span></span> | <span data-ttu-id="4f374-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f374-156">DateTimeOffset</span></span>                       | <span data-ttu-id="4f374-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span><span class="sxs-lookup"><span data-stu-id="4f374-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4f374-158">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4f374-158">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="4f374-159">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="4f374-159">uniqueSenders</span></span>         | <span data-ttu-id="4f374-160">String collection</span><span class="sxs-lookup"><span data-stu-id="4f374-160">String collection</span></span>                    | <span data-ttu-id="4f374-161">向此线程发送邮件的所有用户。</span><span class="sxs-lookup"><span data-stu-id="4f374-161">All the users that sent a message to this thread.</span></span>                                                                                                                                                |
| <span data-ttu-id="4f374-162">preview</span><span class="sxs-lookup"><span data-stu-id="4f374-162">preview</span></span>               | <span data-ttu-id="4f374-163">String</span><span class="sxs-lookup"><span data-stu-id="4f374-163">String</span></span>                               | <span data-ttu-id="4f374-164">本对话中最新帖子的正文中的简短摘要。</span><span class="sxs-lookup"><span data-stu-id="4f374-164">A short summary from the body of the latest post in this conversation.</span></span>                                                                                                                           |
| <span data-ttu-id="4f374-165">Resource.islocked</span><span class="sxs-lookup"><span data-stu-id="4f374-165">isLocked</span></span>              | <span data-ttu-id="4f374-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f374-166">Boolean</span></span>                              | <span data-ttu-id="4f374-167">指示线程是否已锁定。</span><span class="sxs-lookup"><span data-stu-id="4f374-167">Indicates if the thread is locked.</span></span>                                                                                                                                                               |

## <a name="relationships"></a><span data-ttu-id="4f374-168">关系</span><span class="sxs-lookup"><span data-stu-id="4f374-168">Relationships</span></span>
| <span data-ttu-id="4f374-169">关系</span><span class="sxs-lookup"><span data-stu-id="4f374-169">Relationship</span></span> | <span data-ttu-id="4f374-170">类型</span><span class="sxs-lookup"><span data-stu-id="4f374-170">Type</span></span>   |<span data-ttu-id="4f374-171">Description</span><span class="sxs-lookup"><span data-stu-id="4f374-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f374-172">posts</span><span class="sxs-lookup"><span data-stu-id="4f374-172">posts</span></span>|<span data-ttu-id="4f374-173">[帖子](post.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f374-173">[post](post.md) collection</span></span>| <span data-ttu-id="4f374-174">Read-only.</span><span class="sxs-lookup"><span data-stu-id="4f374-174">Read-only.</span></span> <span data-ttu-id="4f374-175">Nullable.</span><span class="sxs-lookup"><span data-stu-id="4f374-175">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f374-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f374-176">JSON representation</span></span>

<span data-ttu-id="4f374-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f374-177">Here is a JSON representation of the resource</span></span>

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
