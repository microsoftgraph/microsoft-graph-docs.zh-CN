---
title: chatThread 资源类型
description: chatThread 是 Microsoft Teams 中的 chatMessages 集合。
localization_priority: Priority
ms.openlocfilehash: 19365109c2008d52d3597b3d23fc1baefa5cfd1c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399603"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="1af8c-103">chatThread 资源类型</span><span class="sxs-lookup"><span data-stu-id="1af8c-103">chatThread resource type</span></span>

> <span data-ttu-id="1af8c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1af8c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1af8c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1af8c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1af8c-106">chatThread 是 Microsoft Teams 中的 [chatMessages](chatmessage.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="1af8c-106">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="1af8c-107">目前，可以[在频道内创建](../api/channel-post-chatthreads.md) chatThread。</span><span class="sxs-lookup"><span data-stu-id="1af8c-107">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="1af8c-108">将来的 API 版本将支持读取现有的 chatThread，以及读取/写入与团队或频道范围外的用户之间的直接聊天。</span><span class="sxs-lookup"><span data-stu-id="1af8c-108">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="1af8c-109">方法</span><span class="sxs-lookup"><span data-stu-id="1af8c-109">Methods</span></span>

| <span data-ttu-id="1af8c-110">方法</span><span class="sxs-lookup"><span data-stu-id="1af8c-110">Method</span></span>       | <span data-ttu-id="1af8c-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="1af8c-111">Return Type</span></span>  |<span data-ttu-id="1af8c-112">说明</span><span class="sxs-lookup"><span data-stu-id="1af8c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1af8c-113">创建线程</span><span class="sxs-lookup"><span data-stu-id="1af8c-113">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="1af8c-114">chatThread</span><span class="sxs-lookup"><span data-stu-id="1af8c-114">chatThread</span></span>](chatthread.md) |<span data-ttu-id="1af8c-115">在指定的频道中启动新线程，提供第一条消息。</span><span class="sxs-lookup"><span data-stu-id="1af8c-115">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="1af8c-116">属性</span><span class="sxs-lookup"><span data-stu-id="1af8c-116">Properties</span></span>
| <span data-ttu-id="1af8c-117">属性</span><span class="sxs-lookup"><span data-stu-id="1af8c-117">Property</span></span>     | <span data-ttu-id="1af8c-118">类型</span><span class="sxs-lookup"><span data-stu-id="1af8c-118">Type</span></span>   |<span data-ttu-id="1af8c-119">说明</span><span class="sxs-lookup"><span data-stu-id="1af8c-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1af8c-120">id</span><span class="sxs-lookup"><span data-stu-id="1af8c-120">id</span></span>|<span data-ttu-id="1af8c-121">String</span><span class="sxs-lookup"><span data-stu-id="1af8c-121">String</span></span>| <span data-ttu-id="1af8c-122">只读。</span><span class="sxs-lookup"><span data-stu-id="1af8c-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1af8c-123">关系</span><span class="sxs-lookup"><span data-stu-id="1af8c-123">Relationships</span></span>
| <span data-ttu-id="1af8c-124">关系</span><span class="sxs-lookup"><span data-stu-id="1af8c-124">Relationship</span></span> | <span data-ttu-id="1af8c-125">类型</span><span class="sxs-lookup"><span data-stu-id="1af8c-125">Type</span></span>   |<span data-ttu-id="1af8c-126">说明</span><span class="sxs-lookup"><span data-stu-id="1af8c-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1af8c-127">rootMessage</span><span class="sxs-lookup"><span data-stu-id="1af8c-127">rootMessage</span></span>|[<span data-ttu-id="1af8c-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="1af8c-128">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="1af8c-129">可为空。</span><span class="sxs-lookup"><span data-stu-id="1af8c-129">Nullable.</span></span>|
|<span data-ttu-id="1af8c-130">chatMessages</span><span class="sxs-lookup"><span data-stu-id="1af8c-130">chatMessages</span></span>|<span data-ttu-id="1af8c-131">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1af8c-131">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="1af8c-132">可为空。</span><span class="sxs-lookup"><span data-stu-id="1af8c-132">Nullable.</span></span>|

> <span data-ttu-id="1af8c-133">目前这些关系是隐式存在的，但不能读取或写入。</span><span class="sxs-lookup"><span data-stu-id="1af8c-133">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="1af8c-134">将来的 beta API 版本将支持此功能。</span><span class="sxs-lookup"><span data-stu-id="1af8c-134">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1af8c-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1af8c-135">JSON representation</span></span>

<span data-ttu-id="1af8c-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1af8c-136">Here is a JSON representation of the resource</span></span>

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
  "id": "string (identifier)"
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
