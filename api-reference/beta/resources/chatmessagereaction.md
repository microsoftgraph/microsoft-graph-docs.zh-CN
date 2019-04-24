---
title: chatMessageReaction 资源类型
description: '表示对了 chatmessage 实体的反应。 '
localization_priority: Normal
ms.openlocfilehash: 5020653ef02c1604aece46f3ff2c7ea1c82a75ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460637"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="15c1e-103">chatMessageReaction 资源类型</span><span class="sxs-lookup"><span data-stu-id="15c1e-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="15c1e-104">表示对[了 chatmessage](chatmessage.md)实体的反应。</span><span class="sxs-lookup"><span data-stu-id="15c1e-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="15c1e-105">类型`chatMessageReaction`的实体作为[Get 信道消息](../api/channel-get-message.md)API 的一部分返回, 作为[了 chatmessage](chatmessage.md)实体的一部分。</span><span class="sxs-lookup"><span data-stu-id="15c1e-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel messages](../api/channel-get-message.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="15c1e-106">属性</span><span class="sxs-lookup"><span data-stu-id="15c1e-106">Properties</span></span>
| <span data-ttu-id="15c1e-107">属性</span><span class="sxs-lookup"><span data-stu-id="15c1e-107">Property</span></span>     | <span data-ttu-id="15c1e-108">类型</span><span class="sxs-lookup"><span data-stu-id="15c1e-108">Type</span></span>   |<span data-ttu-id="15c1e-109">说明</span><span class="sxs-lookup"><span data-stu-id="15c1e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15c1e-110">reactionType</span><span class="sxs-lookup"><span data-stu-id="15c1e-110">reactionType</span></span>|<span data-ttu-id="15c1e-111">字符串</span><span class="sxs-lookup"><span data-stu-id="15c1e-111">string</span></span>| <span data-ttu-id="15c1e-112">反应的类型。</span><span class="sxs-lookup"><span data-stu-id="15c1e-112">The type of reaction.</span></span> <span data-ttu-id="15c1e-113">计划的值包括:</span><span class="sxs-lookup"><span data-stu-id="15c1e-113">Planned values include:</span></span> <br><ul><li><span data-ttu-id="15c1e-114">类似于邮件, 在这种情况下内容为空。</span><span class="sxs-lookup"><span data-stu-id="15c1e-114">Like - Like a message, content is blank in this case.</span></span></li><li><span data-ttu-id="15c1e-115">表情符号-表情符号反应。</span><span class="sxs-lookup"><span data-stu-id="15c1e-115">Emoji - Emoji reaction.</span></span> <span data-ttu-id="15c1e-116">将内容设置为表情符号的 unicode 值。</span><span class="sxs-lookup"><span data-stu-id="15c1e-116">Content is set to unicode value of the emoji.</span></span></li><li><span data-ttu-id="15c1e-117">标签-内容设置为标签中的字符串。</span><span class="sxs-lookup"><span data-stu-id="15c1e-117">Label - Content is set to the string in the label.</span></span></li></ul>|
|<span data-ttu-id="15c1e-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15c1e-118">createdDateTime</span></span>|<span data-ttu-id="15c1e-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15c1e-119">dateTimeOffset</span></span>|<span data-ttu-id="15c1e-120">以 ISO-8601 格式表示的根邮件的 UTC 时间戳。</span><span class="sxs-lookup"><span data-stu-id="15c1e-120">UTC timestamp of the root message in ISO-8601 format.</span></span>|
|<span data-ttu-id="15c1e-121">user</span><span class="sxs-lookup"><span data-stu-id="15c1e-121">user</span></span>|<span data-ttu-id="15c1e-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="15c1e-122">identitySet</span></span>|<span data-ttu-id="15c1e-123">reacted 邮件的用户。</span><span class="sxs-lookup"><span data-stu-id="15c1e-123">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15c1e-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15c1e-124">JSON representation</span></span>

<span data-ttu-id="15c1e-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15c1e-125">The following is a JSON representation of the resource.</span></span>

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
