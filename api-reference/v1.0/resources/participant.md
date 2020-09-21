---
title: 参与者资源类型
description: 代表参与者类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0c5004ea45cf44818c30ffe02dc48a1f6851e64a
ms.sourcegitcommit: d12bd5435c198bcd096e1f7f6a2716f4a04631cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2020
ms.locfileid: "48137112"
---
# <a name="participant-resource-type"></a><span data-ttu-id="14acd-103">参与者资源类型</span><span class="sxs-lookup"><span data-stu-id="14acd-103">participant resource type</span></span>

<span data-ttu-id="14acd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14acd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14acd-105">表示呼叫中的参与者。</span><span class="sxs-lookup"><span data-stu-id="14acd-105">Represents a participant in a call.</span></span>

## <a name="methods"></a><span data-ttu-id="14acd-106">方法</span><span class="sxs-lookup"><span data-stu-id="14acd-106">Methods</span></span>

| <span data-ttu-id="14acd-107">方法</span><span class="sxs-lookup"><span data-stu-id="14acd-107">Method</span></span>                                                 | <span data-ttu-id="14acd-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="14acd-108">Return Type</span></span>                                                 | <span data-ttu-id="14acd-109">说明</span><span class="sxs-lookup"><span data-stu-id="14acd-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="14acd-110">列出参与者</span><span class="sxs-lookup"><span data-stu-id="14acd-110">List participant</span></span>](../api/participant-get.md)          | [<span data-ttu-id="14acd-111">参与者</span><span class="sxs-lookup"><span data-stu-id="14acd-111">participant</span></span>](participant.md)                               | <span data-ttu-id="14acd-112">在呼叫中检索 **参与者** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="14acd-112">Retrieve a list of **participant** objects in the call.</span></span> |
| [<span data-ttu-id="14acd-113">获取参与者</span><span class="sxs-lookup"><span data-stu-id="14acd-113">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="14acd-114">参与者</span><span class="sxs-lookup"><span data-stu-id="14acd-114">participant</span></span>](participant.md)                               | <span data-ttu-id="14acd-115">读取 **参与者** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="14acd-115">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="14acd-116">删除参与者</span><span class="sxs-lookup"><span data-stu-id="14acd-116">Delete participant</span></span>](../api/participant-delete.md)         | <span data-ttu-id="14acd-117">无</span><span class="sxs-lookup"><span data-stu-id="14acd-117">None</span></span>   | <span data-ttu-id="14acd-118">删除呼叫中的参与者。</span><span class="sxs-lookup"><span data-stu-id="14acd-118">Delete a participant in a call.</span></span>                  |
| [<span data-ttu-id="14acd-119">邀请</span><span class="sxs-lookup"><span data-stu-id="14acd-119">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="14acd-120">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="14acd-120">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                        | <span data-ttu-id="14acd-121">邀请参与者加入呼叫。</span><span class="sxs-lookup"><span data-stu-id="14acd-121">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="14acd-122">参与者静音</span><span class="sxs-lookup"><span data-stu-id="14acd-122">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="14acd-123">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="14acd-123">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="14acd-124">将呼叫中的参与者静音。</span><span class="sxs-lookup"><span data-stu-id="14acd-124">Mute a participant in a call.</span></span>                  |

## <a name="properties"></a><span data-ttu-id="14acd-125">属性</span><span class="sxs-lookup"><span data-stu-id="14acd-125">Properties</span></span>

| <span data-ttu-id="14acd-126">属性</span><span class="sxs-lookup"><span data-stu-id="14acd-126">Property</span></span>             | <span data-ttu-id="14acd-127">类型</span><span class="sxs-lookup"><span data-stu-id="14acd-127">Type</span></span>                                     | <span data-ttu-id="14acd-128">说明</span><span class="sxs-lookup"><span data-stu-id="14acd-128">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="14acd-129">id</span><span class="sxs-lookup"><span data-stu-id="14acd-129">id</span></span>                   | <span data-ttu-id="14acd-130">String</span><span class="sxs-lookup"><span data-stu-id="14acd-130">String</span></span>                                   | <span data-ttu-id="14acd-131">参与者 ID。</span><span class="sxs-lookup"><span data-stu-id="14acd-131">The participant ID.</span></span>                                          |
| <span data-ttu-id="14acd-132">info</span><span class="sxs-lookup"><span data-stu-id="14acd-132">info</span></span>                 | [<span data-ttu-id="14acd-133">participantInfo</span><span class="sxs-lookup"><span data-stu-id="14acd-133">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="14acd-134">参与者的参与者。</span><span class="sxs-lookup"><span data-stu-id="14acd-134">The participant of the participant.</span></span>                          |
| <span data-ttu-id="14acd-135">isInLobby</span><span class="sxs-lookup"><span data-stu-id="14acd-135">isInLobby</span></span>            | <span data-ttu-id="14acd-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="14acd-136">Boolean</span></span>                                  | <span data-ttu-id="14acd-137">`true` 如果参与者处于会议厅中。</span><span class="sxs-lookup"><span data-stu-id="14acd-137">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="14acd-138">isMuted</span><span class="sxs-lookup"><span data-stu-id="14acd-138">isMuted</span></span>              | <span data-ttu-id="14acd-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="14acd-139">Boolean</span></span>                                  | <span data-ttu-id="14acd-140">`true` 如果与会者已静音 (客户端或服务器) 。</span><span class="sxs-lookup"><span data-stu-id="14acd-140">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="14acd-141">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="14acd-141">mediaStreams</span></span>         | <span data-ttu-id="14acd-142">[mediaStream](mediastream.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14acd-142">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="14acd-143">媒体流的列表。</span><span class="sxs-lookup"><span data-stu-id="14acd-143">The list of media streams.</span></span>                                   |
| <span data-ttu-id="14acd-144">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="14acd-144">recordingInfo</span></span>        | [<span data-ttu-id="14acd-145">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="14acd-145">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="14acd-146">有关参与者是否有录制功能的信息。</span><span class="sxs-lookup"><span data-stu-id="14acd-146">Information about whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="14acd-147">关系</span><span class="sxs-lookup"><span data-stu-id="14acd-147">Relationships</span></span>
<span data-ttu-id="14acd-148">无。</span><span class="sxs-lookup"><span data-stu-id="14acd-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14acd-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14acd-149">JSON representation</span></span>

<span data-ttu-id="14acd-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14acd-150">The following is a JSON representation of the resource.</span></span>

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

