---
title: 参与者资源类型
description: 参与者类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e6711a771d0c10112850f2d05943f4e8752ebbdf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534084"
---
# <a name="participant-resource-type"></a><span data-ttu-id="dfca3-103">参与者资源类型</span><span class="sxs-lookup"><span data-stu-id="dfca3-103">participant resource type</span></span>

<span data-ttu-id="dfca3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfca3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dfca3-105">参与者类型。</span><span class="sxs-lookup"><span data-stu-id="dfca3-105">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="dfca3-106">Methods</span><span class="sxs-lookup"><span data-stu-id="dfca3-106">Methods</span></span>

| <span data-ttu-id="dfca3-107">方法</span><span class="sxs-lookup"><span data-stu-id="dfca3-107">Method</span></span>                                                 | <span data-ttu-id="dfca3-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="dfca3-108">Return Type</span></span>                                                 | <span data-ttu-id="dfca3-109">说明</span><span class="sxs-lookup"><span data-stu-id="dfca3-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="dfca3-110">获取参与者</span><span class="sxs-lookup"><span data-stu-id="dfca3-110">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="dfca3-111">参与者</span><span class="sxs-lookup"><span data-stu-id="dfca3-111">participant</span></span>](participant.md)                               | <span data-ttu-id="dfca3-112">读取**参与者**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dfca3-112">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="dfca3-113">邀请</span><span class="sxs-lookup"><span data-stu-id="dfca3-113">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="dfca3-114">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="dfca3-114">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                        | <span data-ttu-id="dfca3-115">邀请参与者加入呼叫。</span><span class="sxs-lookup"><span data-stu-id="dfca3-115">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="dfca3-116">参与者静音</span><span class="sxs-lookup"><span data-stu-id="dfca3-116">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="dfca3-117">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="dfca3-117">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="dfca3-118">将呼叫中的参与者静音。</span><span class="sxs-lookup"><span data-stu-id="dfca3-118">Mute a participant in a call.</span></span>                  |

## <a name="properties"></a><span data-ttu-id="dfca3-119">属性</span><span class="sxs-lookup"><span data-stu-id="dfca3-119">Properties</span></span>

| <span data-ttu-id="dfca3-120">属性</span><span class="sxs-lookup"><span data-stu-id="dfca3-120">Property</span></span>             | <span data-ttu-id="dfca3-121">类型</span><span class="sxs-lookup"><span data-stu-id="dfca3-121">Type</span></span>                                     | <span data-ttu-id="dfca3-122">说明</span><span class="sxs-lookup"><span data-stu-id="dfca3-122">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="dfca3-123">id</span><span class="sxs-lookup"><span data-stu-id="dfca3-123">id</span></span>                   | <span data-ttu-id="dfca3-124">字符串</span><span class="sxs-lookup"><span data-stu-id="dfca3-124">String</span></span>                                   | <span data-ttu-id="dfca3-125">参与者 ID。</span><span class="sxs-lookup"><span data-stu-id="dfca3-125">The participant ID.</span></span>                                          |
| <span data-ttu-id="dfca3-126">info</span><span class="sxs-lookup"><span data-stu-id="dfca3-126">info</span></span>                 | [<span data-ttu-id="dfca3-127">participantInfo</span><span class="sxs-lookup"><span data-stu-id="dfca3-127">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="dfca3-128">参与者的参与者。</span><span class="sxs-lookup"><span data-stu-id="dfca3-128">The participant of the participant.</span></span>                          |
| <span data-ttu-id="dfca3-129">isInLobby</span><span class="sxs-lookup"><span data-stu-id="dfca3-129">isInLobby</span></span>            | <span data-ttu-id="dfca3-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfca3-130">Boolean</span></span>                                  | <span data-ttu-id="dfca3-131">`true`如果参与者处于会议厅中。</span><span class="sxs-lookup"><span data-stu-id="dfca3-131">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="dfca3-132">isMuted</span><span class="sxs-lookup"><span data-stu-id="dfca3-132">isMuted</span></span>              | <span data-ttu-id="dfca3-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfca3-133">Boolean</span></span>                                  | <span data-ttu-id="dfca3-134">`true`如果参与者处于静音（客户端或服务器为静音）。</span><span class="sxs-lookup"><span data-stu-id="dfca3-134">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="dfca3-135">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="dfca3-135">mediaStreams</span></span>         | <span data-ttu-id="dfca3-136">[mediaStream](mediastream.md)集合</span><span class="sxs-lookup"><span data-stu-id="dfca3-136">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="dfca3-137">媒体流的列表。</span><span class="sxs-lookup"><span data-stu-id="dfca3-137">The list of media streams.</span></span>                                   |

## <a name="relationships"></a><span data-ttu-id="dfca3-138">关系</span><span class="sxs-lookup"><span data-stu-id="dfca3-138">Relationships</span></span>
<span data-ttu-id="dfca3-139">无。</span><span class="sxs-lookup"><span data-stu-id="dfca3-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfca3-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfca3-140">JSON representation</span></span>

<span data-ttu-id="dfca3-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfca3-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "String (identifier)",
  "info": {"@odata.type": "#microsoft.graph.participantInfo"},
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
