---
title: chatMessageReaction 资源类型
description: '表示对了 chatmessage 实体的反应。 '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: 9dac85d7b177f1b3622129e1187f3a3dca51ba50
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044233"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="8077d-103">chatMessageReaction 资源类型</span><span class="sxs-lookup"><span data-stu-id="8077d-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="8077d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8077d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8077d-105">表示对 [了 chatmessage](chatmessage.md) 实体的反应。</span><span class="sxs-lookup"><span data-stu-id="8077d-105">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="8077d-106">`chatMessageReaction`作为[了 chatmessage](chatmessage.md)实体的一部分，类型的实体作为[Get 信道消息](../api/channel-get-message.md)API 的一部分返回。</span><span class="sxs-lookup"><span data-stu-id="8077d-106">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/channel-get-message.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="8077d-107">属性</span><span class="sxs-lookup"><span data-stu-id="8077d-107">Properties</span></span>

| <span data-ttu-id="8077d-108">属性</span><span class="sxs-lookup"><span data-stu-id="8077d-108">Property</span></span>     | <span data-ttu-id="8077d-109">类型</span><span class="sxs-lookup"><span data-stu-id="8077d-109">Type</span></span>        | <span data-ttu-id="8077d-110">说明</span><span class="sxs-lookup"><span data-stu-id="8077d-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8077d-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8077d-111">createdDateTime</span></span>|<span data-ttu-id="8077d-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8077d-112">DateTimeOffset</span></span>|<span data-ttu-id="8077d-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8077d-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8077d-115">reactionType</span><span class="sxs-lookup"><span data-stu-id="8077d-115">reactionType</span></span>|<span data-ttu-id="8077d-116">String</span><span class="sxs-lookup"><span data-stu-id="8077d-116">String</span></span>|<span data-ttu-id="8077d-117">受支持的值为、、、、 `like` `angry` `sad` `laugh` `heart` 、 `surprised` 。</span><span class="sxs-lookup"><span data-stu-id="8077d-117">Supported values are `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span></span> |
|<span data-ttu-id="8077d-118">user</span><span class="sxs-lookup"><span data-stu-id="8077d-118">user</span></span>|[<span data-ttu-id="8077d-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="8077d-119">identitySet</span></span>](identityset.md)|<span data-ttu-id="8077d-120">Reacted 邮件的用户。</span><span class="sxs-lookup"><span data-stu-id="8077d-120">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8077d-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8077d-121">JSON representation</span></span>

<span data-ttu-id="8077d-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8077d-122">The following is a JSON representation of the resource.</span></span>

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


