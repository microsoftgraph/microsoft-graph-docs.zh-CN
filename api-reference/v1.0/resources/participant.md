---
title: 参与者资源类型
description: 代表参与者类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 82a8cdd51cc7dd8c3be1e06c24ff61b19a9b86ac
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962336"
---
# <a name="participant-resource-type"></a><span data-ttu-id="a3e7e-103">参与者资源类型</span><span class="sxs-lookup"><span data-stu-id="a3e7e-103">participant resource type</span></span>

<span data-ttu-id="a3e7e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3e7e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a3e7e-105">代表参与者类型。</span><span class="sxs-lookup"><span data-stu-id="a3e7e-105">Represents the participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="a3e7e-106">方法</span><span class="sxs-lookup"><span data-stu-id="a3e7e-106">Methods</span></span>

| <span data-ttu-id="a3e7e-107">方法</span><span class="sxs-lookup"><span data-stu-id="a3e7e-107">Method</span></span>                                                 | <span data-ttu-id="a3e7e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a3e7e-108">Return Type</span></span>                                                 | <span data-ttu-id="a3e7e-109">说明</span><span class="sxs-lookup"><span data-stu-id="a3e7e-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="a3e7e-110">获取参与者</span><span class="sxs-lookup"><span data-stu-id="a3e7e-110">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="a3e7e-111">参与者</span><span class="sxs-lookup"><span data-stu-id="a3e7e-111">participant</span></span>](participant.md)                               | <span data-ttu-id="a3e7e-112">读取**参与者**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a3e7e-112">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="a3e7e-113">邀请</span><span class="sxs-lookup"><span data-stu-id="a3e7e-113">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="a3e7e-114">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="a3e7e-114">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                        | <span data-ttu-id="a3e7e-115">邀请参与者加入呼叫。</span><span class="sxs-lookup"><span data-stu-id="a3e7e-115">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="a3e7e-116">参与者静音</span><span class="sxs-lookup"><span data-stu-id="a3e7e-116">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="a3e7e-117">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="a3e7e-117">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="a3e7e-118">将呼叫中的参与者静音。</span><span class="sxs-lookup"><span data-stu-id="a3e7e-118">Mute a participant in a call.</span></span>                  |

## <a name="properties"></a><span data-ttu-id="a3e7e-119">属性</span><span class="sxs-lookup"><span data-stu-id="a3e7e-119">Properties</span></span>

| <span data-ttu-id="a3e7e-120">属性</span><span class="sxs-lookup"><span data-stu-id="a3e7e-120">Property</span></span>             | <span data-ttu-id="a3e7e-121">类型</span><span class="sxs-lookup"><span data-stu-id="a3e7e-121">Type</span></span>                                     | <span data-ttu-id="a3e7e-122">说明</span><span class="sxs-lookup"><span data-stu-id="a3e7e-122">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="a3e7e-123">id</span><span class="sxs-lookup"><span data-stu-id="a3e7e-123">id</span></span>                   | <span data-ttu-id="a3e7e-124">String</span><span class="sxs-lookup"><span data-stu-id="a3e7e-124">String</span></span>                                   | <span data-ttu-id="a3e7e-125">参与者 ID。</span><span class="sxs-lookup"><span data-stu-id="a3e7e-125">The participant ID.</span></span>                                          |
| <span data-ttu-id="a3e7e-126">info</span><span class="sxs-lookup"><span data-stu-id="a3e7e-126">info</span></span>                 | [<span data-ttu-id="a3e7e-127">participantInfo</span><span class="sxs-lookup"><span data-stu-id="a3e7e-127">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="a3e7e-128">参与者的参与者。</span><span class="sxs-lookup"><span data-stu-id="a3e7e-128">The participant of the participant.</span></span>                          |
| <span data-ttu-id="a3e7e-129">isInLobby</span><span class="sxs-lookup"><span data-stu-id="a3e7e-129">isInLobby</span></span>            | <span data-ttu-id="a3e7e-130">布尔</span><span class="sxs-lookup"><span data-stu-id="a3e7e-130">Boolean</span></span>                                  | <span data-ttu-id="a3e7e-131">`true`如果参与者处于会议厅中。</span><span class="sxs-lookup"><span data-stu-id="a3e7e-131">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="a3e7e-132">isMuted</span><span class="sxs-lookup"><span data-stu-id="a3e7e-132">isMuted</span></span>              | <span data-ttu-id="a3e7e-133">布尔</span><span class="sxs-lookup"><span data-stu-id="a3e7e-133">Boolean</span></span>                                  | <span data-ttu-id="a3e7e-134">`true`如果参与者处于静音（客户端或服务器为静音）。</span><span class="sxs-lookup"><span data-stu-id="a3e7e-134">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="a3e7e-135">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="a3e7e-135">mediaStreams</span></span>         | <span data-ttu-id="a3e7e-136">[mediaStream](mediastream.md)集合</span><span class="sxs-lookup"><span data-stu-id="a3e7e-136">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="a3e7e-137">媒体流的列表。</span><span class="sxs-lookup"><span data-stu-id="a3e7e-137">The list of media streams.</span></span>                                   |
| <span data-ttu-id="a3e7e-138">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="a3e7e-138">recordingInfo</span></span>        | [<span data-ttu-id="a3e7e-139">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="a3e7e-139">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="a3e7e-140">有关参与者是否有录制功能的信息。</span><span class="sxs-lookup"><span data-stu-id="a3e7e-140">Information about whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a3e7e-141">关系</span><span class="sxs-lookup"><span data-stu-id="a3e7e-141">Relationships</span></span>
<span data-ttu-id="a3e7e-142">无。</span><span class="sxs-lookup"><span data-stu-id="a3e7e-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3e7e-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3e7e-143">JSON representation</span></span>

<span data-ttu-id="a3e7e-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3e7e-144">The following is a JSON representation of the resource.</span></span>

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
