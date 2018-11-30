---
title: chatMessageReaction 资源类型
description: '代表 chatMessage 实体的反应。 '
ms.openlocfilehash: 1ad1f7948405a8891ec9aa13065b71108e9c47c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049183"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="c2f45-103">chatMessageReaction 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2f45-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="c2f45-104">代表[chatMessage](chatmessage.md)实体的反应。</span><span class="sxs-lookup"><span data-stu-id="c2f45-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="c2f45-105">实体类型的`chatMessageReaction`返回作为一部分[获取通道消息](../api/channel-get-message.md)API，作为[chatMessage](chatmessage.md)实体的一部分。</span><span class="sxs-lookup"><span data-stu-id="c2f45-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel messages](../api/channel-get-message.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="c2f45-106">属性</span><span class="sxs-lookup"><span data-stu-id="c2f45-106">Properties</span></span>
| <span data-ttu-id="c2f45-107">属性</span><span class="sxs-lookup"><span data-stu-id="c2f45-107">Property</span></span>     | <span data-ttu-id="c2f45-108">类型</span><span class="sxs-lookup"><span data-stu-id="c2f45-108">Type</span></span>   |<span data-ttu-id="c2f45-109">说明</span><span class="sxs-lookup"><span data-stu-id="c2f45-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2f45-110">reactionType</span><span class="sxs-lookup"><span data-stu-id="c2f45-110">reactionType</span></span>|<span data-ttu-id="c2f45-111">string</span><span class="sxs-lookup"><span data-stu-id="c2f45-111">string</span></span>| <span data-ttu-id="c2f45-112">反应的类型。</span><span class="sxs-lookup"><span data-stu-id="c2f45-112">The type of reaction.</span></span> <span data-ttu-id="c2f45-113">计划的值包括：</span><span class="sxs-lookup"><span data-stu-id="c2f45-113">Planned values include:</span></span> <br><ul><li><span data-ttu-id="c2f45-114">像-像一条消息，内容为空在这种情况下。</span><span class="sxs-lookup"><span data-stu-id="c2f45-114">Like - Like a message, content is blank in this case.</span></span></li><li><span data-ttu-id="c2f45-115">Emoji-Emoji 反应。</span><span class="sxs-lookup"><span data-stu-id="c2f45-115">Emoji - Emoji reaction.</span></span> <span data-ttu-id="c2f45-116">内容设置为 unicode 值的 emoji。</span><span class="sxs-lookup"><span data-stu-id="c2f45-116">Content is set to unicode value of the emoji.</span></span></li><li><span data-ttu-id="c2f45-117">标签-内容设置为中标签的字符串。</span><span class="sxs-lookup"><span data-stu-id="c2f45-117">Label - Content is set to the string in the label.</span></span></li></ul>|
|<span data-ttu-id="c2f45-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2f45-118">createdDateTime</span></span>|<span data-ttu-id="c2f45-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2f45-119">dateTimeOffset</span></span>|<span data-ttu-id="c2f45-120">ISO-8601 格式中的根消息的 UTC 时间戳。</span><span class="sxs-lookup"><span data-stu-id="c2f45-120">UTC timestamp of the root message in ISO-8601 format.</span></span>|
|<span data-ttu-id="c2f45-121">user</span><span class="sxs-lookup"><span data-stu-id="c2f45-121">user</span></span>|<span data-ttu-id="c2f45-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="c2f45-122">identitySet</span></span>|<span data-ttu-id="c2f45-123">反应到邮件用户。</span><span class="sxs-lookup"><span data-stu-id="c2f45-123">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2f45-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2f45-124">JSON representation</span></span>

<span data-ttu-id="c2f45-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2f45-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "content"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageReaction"
}-->

```json
{
  "reactionType": "string ",
  "createdDateTime": "string (timestamp)",
  "user": {"@odata.type": "microsoft.graph.identitySet"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message reaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
