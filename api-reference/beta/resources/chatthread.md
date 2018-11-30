---
title: chatThread 资源类型
description: ChatThread 是 chatMessages 中的 Microsoft 团队的集合。
ms.openlocfilehash: ef8f118ae4354a5e4197802708aecfa1fb6f8cb8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048298"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="3421e-103">chatThread 资源类型</span><span class="sxs-lookup"><span data-stu-id="3421e-103">chatThread resource type</span></span>

> <span data-ttu-id="3421e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3421e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3421e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3421e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3421e-106">ChatThread 是[chatMessages](chatmessage.md)中的 Microsoft 团队的集合。</span><span class="sxs-lookup"><span data-stu-id="3421e-106">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="3421e-107">目前，chatThreads 可以是[在通道中创建](../api/channel-post-chatthreads.md)。</span><span class="sxs-lookup"><span data-stu-id="3421e-107">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="3421e-108">未来 API 版本将支持读取现有 chatThreads，以及读取/写入直接聊天之间的团队或通道范围之外的用户。</span><span class="sxs-lookup"><span data-stu-id="3421e-108">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="3421e-109">方法</span><span class="sxs-lookup"><span data-stu-id="3421e-109">Methods</span></span>

| <span data-ttu-id="3421e-110">方法</span><span class="sxs-lookup"><span data-stu-id="3421e-110">Method</span></span>       | <span data-ttu-id="3421e-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3421e-111">Return Type</span></span>  |<span data-ttu-id="3421e-112">说明</span><span class="sxs-lookup"><span data-stu-id="3421e-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3421e-113">创建线程</span><span class="sxs-lookup"><span data-stu-id="3421e-113">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="3421e-114">chatThread</span><span class="sxs-lookup"><span data-stu-id="3421e-114">chatThread</span></span>](chatthread.md) |<span data-ttu-id="3421e-115">在指定的通道，提供第一条消息中启动一个新的线程。</span><span class="sxs-lookup"><span data-stu-id="3421e-115">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="3421e-116">属性</span><span class="sxs-lookup"><span data-stu-id="3421e-116">Properties</span></span>
| <span data-ttu-id="3421e-117">属性</span><span class="sxs-lookup"><span data-stu-id="3421e-117">Property</span></span>     | <span data-ttu-id="3421e-118">类型</span><span class="sxs-lookup"><span data-stu-id="3421e-118">Type</span></span>   |<span data-ttu-id="3421e-119">说明</span><span class="sxs-lookup"><span data-stu-id="3421e-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3421e-120">id</span><span class="sxs-lookup"><span data-stu-id="3421e-120">id</span></span>|<span data-ttu-id="3421e-121">String</span><span class="sxs-lookup"><span data-stu-id="3421e-121">String</span></span>| <span data-ttu-id="3421e-122">只读。</span><span class="sxs-lookup"><span data-stu-id="3421e-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3421e-123">Relationships</span><span class="sxs-lookup"><span data-stu-id="3421e-123">Relationships</span></span>
| <span data-ttu-id="3421e-124">关系</span><span class="sxs-lookup"><span data-stu-id="3421e-124">Relationship</span></span> | <span data-ttu-id="3421e-125">类型</span><span class="sxs-lookup"><span data-stu-id="3421e-125">Type</span></span>   |<span data-ttu-id="3421e-126">说明</span><span class="sxs-lookup"><span data-stu-id="3421e-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3421e-127">rootMessage</span><span class="sxs-lookup"><span data-stu-id="3421e-127">rootMessage</span></span>|[<span data-ttu-id="3421e-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="3421e-128">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="3421e-129">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3421e-129">Nullable.</span></span>|
|<span data-ttu-id="3421e-130">chatMessages</span><span class="sxs-lookup"><span data-stu-id="3421e-130">chatMessages</span></span>|<span data-ttu-id="3421e-131">[chatMessage](chatmessage.md)集合</span><span class="sxs-lookup"><span data-stu-id="3421e-131">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="3421e-132">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3421e-132">Nullable.</span></span>|

> <span data-ttu-id="3421e-133">当前这些关系存在隐式，但不能读取或写入。</span><span class="sxs-lookup"><span data-stu-id="3421e-133">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="3421e-134">将来 beta API 版本将支持此功能。</span><span class="sxs-lookup"><span data-stu-id="3421e-134">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3421e-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3421e-135">JSON representation</span></span>

<span data-ttu-id="3421e-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3421e-136">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatThread"
}-->

```json
{
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
