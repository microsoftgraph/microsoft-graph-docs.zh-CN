---
title: chatMessageReaction 资源类型
description: '表示对了 chatmessage 实体的反应。 '
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dd1eac9a4630e097f06cf99f30d371de9e32eb5f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991490"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="16a76-103">chatMessageReaction 资源类型</span><span class="sxs-lookup"><span data-stu-id="16a76-103">chatMessageReaction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16a76-104">表示对[了 chatmessage](chatmessage.md)实体的反应。</span><span class="sxs-lookup"><span data-stu-id="16a76-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="16a76-105">作为[了 chatmessage](chatmessage.md)实体的`chatMessageReaction`一部分, 类型的实体作为[Get 信道消息](../api/channel-get-message.md)API 的一部分返回。</span><span class="sxs-lookup"><span data-stu-id="16a76-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/channel-get-message.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="16a76-106">属性</span><span class="sxs-lookup"><span data-stu-id="16a76-106">Properties</span></span>

| <span data-ttu-id="16a76-107">属性</span><span class="sxs-lookup"><span data-stu-id="16a76-107">Property</span></span>     | <span data-ttu-id="16a76-108">类型</span><span class="sxs-lookup"><span data-stu-id="16a76-108">Type</span></span>        | <span data-ttu-id="16a76-109">说明</span><span class="sxs-lookup"><span data-stu-id="16a76-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="16a76-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16a76-110">createdDateTime</span></span>|<span data-ttu-id="16a76-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16a76-111">DateTimeOffset</span></span>|<span data-ttu-id="16a76-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="16a76-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="16a76-114">reactionType</span><span class="sxs-lookup"><span data-stu-id="16a76-114">reactionType</span></span>|<span data-ttu-id="16a76-115">String</span><span class="sxs-lookup"><span data-stu-id="16a76-115">String</span></span>|<span data-ttu-id="16a76-116">受支持的`like`值`angry`为`sad`、 `laugh`、 `heart`、 `surprised`、、。</span><span class="sxs-lookup"><span data-stu-id="16a76-116">Supported values are `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span></span> |
|<span data-ttu-id="16a76-117">user</span><span class="sxs-lookup"><span data-stu-id="16a76-117">user</span></span>|[<span data-ttu-id="16a76-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="16a76-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="16a76-119">Reacted 邮件的用户。</span><span class="sxs-lookup"><span data-stu-id="16a76-119">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16a76-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16a76-120">JSON representation</span></span>

<span data-ttu-id="16a76-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16a76-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageReaction",
  "baseType": null
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "reactionType": "String",
  "user": {"@odata.type": "microsoft.graph.identitySet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageReaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
