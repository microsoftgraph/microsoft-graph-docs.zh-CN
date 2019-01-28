---
title: chatThread 资源类型
description: chatThread 是 Microsoft Teams 中的 chatMessages 集合。
localization_priority: Priority
ms.openlocfilehash: a85b6aea6c48c9295fe88a7412fa7e6b96ee1d3f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521339"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="b68c4-103">chatThread 资源类型</span><span class="sxs-lookup"><span data-stu-id="b68c4-103">chatThread resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b68c4-104">chatThread 是 Microsoft Teams 中的 [chatMessages](chatmessage.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="b68c4-104">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="b68c4-105">目前，可以[在频道内创建](../api/channel-post-chatthreads.md) chatThread。</span><span class="sxs-lookup"><span data-stu-id="b68c4-105">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="b68c4-106">将来的 API 版本将支持读取现有的 chatThread，以及读取/写入与团队或频道范围外的用户之间的直接聊天。</span><span class="sxs-lookup"><span data-stu-id="b68c4-106">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="b68c4-107">方法</span><span class="sxs-lookup"><span data-stu-id="b68c4-107">Methods</span></span>

| <span data-ttu-id="b68c4-108">方法</span><span class="sxs-lookup"><span data-stu-id="b68c4-108">Method</span></span>       | <span data-ttu-id="b68c4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b68c4-109">Return Type</span></span>  |<span data-ttu-id="b68c4-110">说明</span><span class="sxs-lookup"><span data-stu-id="b68c4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b68c4-111">创建线程</span><span class="sxs-lookup"><span data-stu-id="b68c4-111">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="b68c4-112">chatThread</span><span class="sxs-lookup"><span data-stu-id="b68c4-112">chatThread</span></span>](chatthread.md) |<span data-ttu-id="b68c4-113">在指定的频道中启动新线程，提供第一条消息。</span><span class="sxs-lookup"><span data-stu-id="b68c4-113">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="b68c4-114">属性</span><span class="sxs-lookup"><span data-stu-id="b68c4-114">Properties</span></span>
| <span data-ttu-id="b68c4-115">属性</span><span class="sxs-lookup"><span data-stu-id="b68c4-115">Property</span></span>     | <span data-ttu-id="b68c4-116">类型</span><span class="sxs-lookup"><span data-stu-id="b68c4-116">Type</span></span>   |<span data-ttu-id="b68c4-117">说明</span><span class="sxs-lookup"><span data-stu-id="b68c4-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b68c4-118">id</span><span class="sxs-lookup"><span data-stu-id="b68c4-118">id</span></span>|<span data-ttu-id="b68c4-119">String</span><span class="sxs-lookup"><span data-stu-id="b68c4-119">String</span></span>| <span data-ttu-id="b68c4-120">只读。</span><span class="sxs-lookup"><span data-stu-id="b68c4-120">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b68c4-121">关系</span><span class="sxs-lookup"><span data-stu-id="b68c4-121">Relationships</span></span>
| <span data-ttu-id="b68c4-122">关系</span><span class="sxs-lookup"><span data-stu-id="b68c4-122">Relationship</span></span> | <span data-ttu-id="b68c4-123">类型</span><span class="sxs-lookup"><span data-stu-id="b68c4-123">Type</span></span>   |<span data-ttu-id="b68c4-124">说明</span><span class="sxs-lookup"><span data-stu-id="b68c4-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b68c4-125">rootMessage</span><span class="sxs-lookup"><span data-stu-id="b68c4-125">rootMessage</span></span>|[<span data-ttu-id="b68c4-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b68c4-126">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="b68c4-127">可为空。</span><span class="sxs-lookup"><span data-stu-id="b68c4-127">Nullable.</span></span>|
|<span data-ttu-id="b68c4-128">chatMessages</span><span class="sxs-lookup"><span data-stu-id="b68c4-128">chatMessages</span></span>|<span data-ttu-id="b68c4-129">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b68c4-129">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="b68c4-130">可为空。</span><span class="sxs-lookup"><span data-stu-id="b68c4-130">Nullable.</span></span>|

> <span data-ttu-id="b68c4-131">目前这些关系是隐式存在的，但不能读取或写入。</span><span class="sxs-lookup"><span data-stu-id="b68c4-131">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="b68c4-132">将来的 beta API 版本将支持此功能。</span><span class="sxs-lookup"><span data-stu-id="b68c4-132">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b68c4-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b68c4-133">JSON representation</span></span>

<span data-ttu-id="b68c4-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b68c4-134">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatthread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
