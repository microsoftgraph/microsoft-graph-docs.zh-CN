---
title: 参与者资源类型
description: 参与者类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3f9e861cc5427243b18ff920facab7544d6315ad
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913735"
---
# <a name="participant-resource-type"></a><span data-ttu-id="8cb3c-103">参与者资源类型</span><span class="sxs-lookup"><span data-stu-id="8cb3c-103">participant resource type</span></span>

<span data-ttu-id="8cb3c-104">参与者类型。</span><span class="sxs-lookup"><span data-stu-id="8cb3c-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="8cb3c-105">方法</span><span class="sxs-lookup"><span data-stu-id="8cb3c-105">Methods</span></span>

| <span data-ttu-id="8cb3c-106">方法</span><span class="sxs-lookup"><span data-stu-id="8cb3c-106">Method</span></span>                                                 | <span data-ttu-id="8cb3c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="8cb3c-107">Return Type</span></span>                                                 | <span data-ttu-id="8cb3c-108">说明</span><span class="sxs-lookup"><span data-stu-id="8cb3c-108">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="8cb3c-109">获取参与者</span><span class="sxs-lookup"><span data-stu-id="8cb3c-109">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="8cb3c-110">参与者</span><span class="sxs-lookup"><span data-stu-id="8cb3c-110">participant</span></span>](participant.md)                               | <span data-ttu-id="8cb3c-111">读取**参与者**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8cb3c-111">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="8cb3c-112">邀请</span><span class="sxs-lookup"><span data-stu-id="8cb3c-112">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="8cb3c-113">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="8cb3c-113">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                        | <span data-ttu-id="8cb3c-114">邀请参与者加入呼叫。</span><span class="sxs-lookup"><span data-stu-id="8cb3c-114">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="8cb3c-115">参与者静音</span><span class="sxs-lookup"><span data-stu-id="8cb3c-115">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="8cb3c-116">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="8cb3c-116">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="8cb3c-117">将呼叫中的参与者静音。</span><span class="sxs-lookup"><span data-stu-id="8cb3c-117">Mute a participant in a call.</span></span>                  |

## <a name="properties"></a><span data-ttu-id="8cb3c-118">属性</span><span class="sxs-lookup"><span data-stu-id="8cb3c-118">Properties</span></span>

| <span data-ttu-id="8cb3c-119">属性</span><span class="sxs-lookup"><span data-stu-id="8cb3c-119">Property</span></span>             | <span data-ttu-id="8cb3c-120">类型</span><span class="sxs-lookup"><span data-stu-id="8cb3c-120">Type</span></span>                                     | <span data-ttu-id="8cb3c-121">说明</span><span class="sxs-lookup"><span data-stu-id="8cb3c-121">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="8cb3c-122">id</span><span class="sxs-lookup"><span data-stu-id="8cb3c-122">id</span></span>                   | <span data-ttu-id="8cb3c-123">String</span><span class="sxs-lookup"><span data-stu-id="8cb3c-123">String</span></span>                                   | <span data-ttu-id="8cb3c-124">参与者 ID。</span><span class="sxs-lookup"><span data-stu-id="8cb3c-124">The participant ID.</span></span>                                          |
| <span data-ttu-id="8cb3c-125">info</span><span class="sxs-lookup"><span data-stu-id="8cb3c-125">info</span></span>                 | [<span data-ttu-id="8cb3c-126">participantInfo</span><span class="sxs-lookup"><span data-stu-id="8cb3c-126">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="8cb3c-127">参与者的参与者。</span><span class="sxs-lookup"><span data-stu-id="8cb3c-127">The participant of the participant.</span></span>                          |
| <span data-ttu-id="8cb3c-128">isInLobby</span><span class="sxs-lookup"><span data-stu-id="8cb3c-128">isInLobby</span></span>            | <span data-ttu-id="8cb3c-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cb3c-129">Boolean</span></span>                                  | <span data-ttu-id="8cb3c-130">`true`如果参与者处于会议厅中。</span><span class="sxs-lookup"><span data-stu-id="8cb3c-130">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="8cb3c-131">isMuted</span><span class="sxs-lookup"><span data-stu-id="8cb3c-131">isMuted</span></span>              | <span data-ttu-id="8cb3c-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cb3c-132">Boolean</span></span>                                  | <span data-ttu-id="8cb3c-133">`true`如果参与者处于静音（客户端或服务器为静音）。</span><span class="sxs-lookup"><span data-stu-id="8cb3c-133">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="8cb3c-134">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="8cb3c-134">mediaStreams</span></span>         | <span data-ttu-id="8cb3c-135">[mediaStream](mediastream.md)集合</span><span class="sxs-lookup"><span data-stu-id="8cb3c-135">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="8cb3c-136">媒体流的列表。</span><span class="sxs-lookup"><span data-stu-id="8cb3c-136">The list of media streams.</span></span>                                   |

## <a name="relationships"></a><span data-ttu-id="8cb3c-137">关系</span><span class="sxs-lookup"><span data-stu-id="8cb3c-137">Relationships</span></span>
<span data-ttu-id="8cb3c-138">无。</span><span class="sxs-lookup"><span data-stu-id="8cb3c-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cb3c-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8cb3c-139">JSON representation</span></span>

<span data-ttu-id="8cb3c-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cb3c-140">The following is a JSON representation of the resource.</span></span>

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
