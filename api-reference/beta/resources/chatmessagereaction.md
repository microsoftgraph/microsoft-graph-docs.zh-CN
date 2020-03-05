---
title: chatMessageReaction 资源类型
description: '表示对了 chatmessage 实体的反应。 '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: cb26a46a3669b721184399036fa80e4a6b291ec8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507689"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="09881-103">chatMessageReaction 资源类型</span><span class="sxs-lookup"><span data-stu-id="09881-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="09881-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="09881-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09881-105">表示对[了 chatmessage](chatmessage.md)实体的反应。</span><span class="sxs-lookup"><span data-stu-id="09881-105">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="09881-106">作为[了 chatmessage](chatmessage.md)实体的`chatMessageReaction`一部分，类型的实体作为[Get 信道消息](../api/channel-get-message.md)API 的一部分返回。</span><span class="sxs-lookup"><span data-stu-id="09881-106">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/channel-get-message.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="09881-107">属性</span><span class="sxs-lookup"><span data-stu-id="09881-107">Properties</span></span>

| <span data-ttu-id="09881-108">属性</span><span class="sxs-lookup"><span data-stu-id="09881-108">Property</span></span>     | <span data-ttu-id="09881-109">类型</span><span class="sxs-lookup"><span data-stu-id="09881-109">Type</span></span>        | <span data-ttu-id="09881-110">说明</span><span class="sxs-lookup"><span data-stu-id="09881-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="09881-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09881-111">createdDateTime</span></span>|<span data-ttu-id="09881-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09881-112">DateTimeOffset</span></span>|<span data-ttu-id="09881-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="09881-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="09881-115">reactionType</span><span class="sxs-lookup"><span data-stu-id="09881-115">reactionType</span></span>|<span data-ttu-id="09881-116">String</span><span class="sxs-lookup"><span data-stu-id="09881-116">String</span></span>|<span data-ttu-id="09881-117">受支持的`like`值`angry`为`sad`、 `laugh`、 `heart`、 `surprised`、、。</span><span class="sxs-lookup"><span data-stu-id="09881-117">Supported values are `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span></span> |
|<span data-ttu-id="09881-118">user</span><span class="sxs-lookup"><span data-stu-id="09881-118">user</span></span>|[<span data-ttu-id="09881-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="09881-119">identitySet</span></span>](identityset.md)|<span data-ttu-id="09881-120">Reacted 邮件的用户。</span><span class="sxs-lookup"><span data-stu-id="09881-120">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09881-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09881-121">JSON representation</span></span>

<span data-ttu-id="09881-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09881-122">The following is a JSON representation of the resource.</span></span>

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
