---
title: chatMessageReaction 资源类型
description: '表示对 chatMessage 实体的一种反应。 '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: bc7a3a5cbff2aee1191383ac18128e97075b4b99
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721619"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="92a0e-103">chatMessageReaction 资源类型</span><span class="sxs-lookup"><span data-stu-id="92a0e-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="92a0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92a0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92a0e-105">表示对 [chatMessage 实体](chatmessage.md) 的一种反应。</span><span class="sxs-lookup"><span data-stu-id="92a0e-105">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="92a0e-106">类型实体作为 `chatMessageReaction` [chatMessage](chatmessage.md)实体的一部分作为[获取](../api/channel-get-message.md)频道消息 API 的一部分返回。</span><span class="sxs-lookup"><span data-stu-id="92a0e-106">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/channel-get-message.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="92a0e-107">属性</span><span class="sxs-lookup"><span data-stu-id="92a0e-107">Properties</span></span>

| <span data-ttu-id="92a0e-108">属性</span><span class="sxs-lookup"><span data-stu-id="92a0e-108">Property</span></span>     | <span data-ttu-id="92a0e-109">类型</span><span class="sxs-lookup"><span data-stu-id="92a0e-109">Type</span></span>        | <span data-ttu-id="92a0e-110">说明</span><span class="sxs-lookup"><span data-stu-id="92a0e-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="92a0e-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92a0e-111">createdDateTime</span></span>|<span data-ttu-id="92a0e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92a0e-112">DateTimeOffset</span></span>|<span data-ttu-id="92a0e-113">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="92a0e-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="92a0e-114">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="92a0e-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="92a0e-115">reactionType</span><span class="sxs-lookup"><span data-stu-id="92a0e-115">reactionType</span></span>|<span data-ttu-id="92a0e-116">String</span><span class="sxs-lookup"><span data-stu-id="92a0e-116">String</span></span>|<span data-ttu-id="92a0e-117">支持的值是 `like` ， ， ， ， `angry` `sad` `laugh` `heart` `surprised` 。</span><span class="sxs-lookup"><span data-stu-id="92a0e-117">Supported values are `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span></span> |
|<span data-ttu-id="92a0e-118">user</span><span class="sxs-lookup"><span data-stu-id="92a0e-118">user</span></span>|[<span data-ttu-id="92a0e-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="92a0e-119">identitySet</span></span>](identityset.md)|<span data-ttu-id="92a0e-120">对邮件做出响应的用户。</span><span class="sxs-lookup"><span data-stu-id="92a0e-120">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92a0e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92a0e-121">JSON representation</span></span>

<span data-ttu-id="92a0e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92a0e-122">The following is a JSON representation of the resource.</span></span>

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


