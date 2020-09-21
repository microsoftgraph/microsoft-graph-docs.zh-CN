---
title: 参与者资源类型
description: 参与者类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7598171b4d706a639a11d425ffa409e25126dcf8
ms.sourcegitcommit: d12bd5435c198bcd096e1f7f6a2716f4a04631cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2020
ms.locfileid: "48137146"
---
# <a name="participant-resource-type"></a><span data-ttu-id="db51b-103">参与者资源类型</span><span class="sxs-lookup"><span data-stu-id="db51b-103">participant resource type</span></span>

<span data-ttu-id="db51b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db51b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db51b-105">表示呼叫中的参与者。</span><span class="sxs-lookup"><span data-stu-id="db51b-105">Represents a participant in a call.</span></span>

## <a name="methods"></a><span data-ttu-id="db51b-106">方法</span><span class="sxs-lookup"><span data-stu-id="db51b-106">Methods</span></span>

| <span data-ttu-id="db51b-107">方法</span><span class="sxs-lookup"><span data-stu-id="db51b-107">Method</span></span>                                                 | <span data-ttu-id="db51b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="db51b-108">Return Type</span></span>                                                 | <span data-ttu-id="db51b-109">说明</span><span class="sxs-lookup"><span data-stu-id="db51b-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="db51b-110">列出参与者</span><span class="sxs-lookup"><span data-stu-id="db51b-110">List participant</span></span>](../api/participant-get.md)         | [<span data-ttu-id="db51b-111">参与者</span><span class="sxs-lookup"><span data-stu-id="db51b-111">participant</span></span>](participant.md)                               | <span data-ttu-id="db51b-112">在呼叫中检索 **参与者** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="db51b-112">Retrieve a list of **participant** objects in the call.</span></span> |
| [<span data-ttu-id="db51b-113">获取参与者</span><span class="sxs-lookup"><span data-stu-id="db51b-113">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="db51b-114">参与者</span><span class="sxs-lookup"><span data-stu-id="db51b-114">participant</span></span>](participant.md)                               | <span data-ttu-id="db51b-115">读取 **参与者** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="db51b-115">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="db51b-116">删除参与者</span><span class="sxs-lookup"><span data-stu-id="db51b-116">Delete participant</span></span>](../api/participant-delete.md)     | <span data-ttu-id="db51b-117">无</span><span class="sxs-lookup"><span data-stu-id="db51b-117">None</span></span>   | <span data-ttu-id="db51b-118">删除呼叫中的参与者。</span><span class="sxs-lookup"><span data-stu-id="db51b-118">Delete a participant in a call.</span></span>                  |
| [<span data-ttu-id="db51b-119">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="db51b-119">ConfigureMixer</span></span>](../api/participant-configuremixer.md) | [<span data-ttu-id="db51b-120">commsOperation</span><span class="sxs-lookup"><span data-stu-id="db51b-120">commsOperation</span></span>](commsoperation.md)                         | <span data-ttu-id="db51b-121">配置参与者音频混合器。</span><span class="sxs-lookup"><span data-stu-id="db51b-121">Configure the participant audio mixer.</span></span>         |
| [<span data-ttu-id="db51b-122">邀请</span><span class="sxs-lookup"><span data-stu-id="db51b-122">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="db51b-123">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="db51b-123">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                         | <span data-ttu-id="db51b-124">邀请参与者加入呼叫。</span><span class="sxs-lookup"><span data-stu-id="db51b-124">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="db51b-125">参与者静音</span><span class="sxs-lookup"><span data-stu-id="db51b-125">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="db51b-126">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="db51b-126">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="db51b-127">将呼叫中的参与者静音。</span><span class="sxs-lookup"><span data-stu-id="db51b-127">Mute a participant in a call.</span></span>                  |
| [<span data-ttu-id="db51b-128">所有参与者静音</span><span class="sxs-lookup"><span data-stu-id="db51b-128">Mute all participants</span></span>](../api/participant-muteall.md) | [<span data-ttu-id="db51b-129">commsOperation</span><span class="sxs-lookup"><span data-stu-id="db51b-129">commsOperation</span></span>](commsoperation.md) | <span data-ttu-id="db51b-130">将会议中的所有参与者设为静音。</span><span class="sxs-lookup"><span data-stu-id="db51b-130">Mute all the participants in the meeting.</span></span>      |

## <a name="properties"></a><span data-ttu-id="db51b-131">属性</span><span class="sxs-lookup"><span data-stu-id="db51b-131">Properties</span></span>

| <span data-ttu-id="db51b-132">属性</span><span class="sxs-lookup"><span data-stu-id="db51b-132">Property</span></span>             | <span data-ttu-id="db51b-133">类型</span><span class="sxs-lookup"><span data-stu-id="db51b-133">Type</span></span>                                     | <span data-ttu-id="db51b-134">说明</span><span class="sxs-lookup"><span data-stu-id="db51b-134">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="db51b-135">id</span><span class="sxs-lookup"><span data-stu-id="db51b-135">id</span></span>                   | <span data-ttu-id="db51b-136">String</span><span class="sxs-lookup"><span data-stu-id="db51b-136">String</span></span>                                   | <span data-ttu-id="db51b-137">参与者 ID。</span><span class="sxs-lookup"><span data-stu-id="db51b-137">The participant ID.</span></span>                                          |
| <span data-ttu-id="db51b-138">info</span><span class="sxs-lookup"><span data-stu-id="db51b-138">info</span></span>                 | [<span data-ttu-id="db51b-139">participantInfo</span><span class="sxs-lookup"><span data-stu-id="db51b-139">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="db51b-140">参与者的参与者。</span><span class="sxs-lookup"><span data-stu-id="db51b-140">The participant of the participant.</span></span>                          |
| <span data-ttu-id="db51b-141">isInLobby</span><span class="sxs-lookup"><span data-stu-id="db51b-141">isInLobby</span></span>            | <span data-ttu-id="db51b-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="db51b-142">Boolean</span></span>                                  | <span data-ttu-id="db51b-143">`true` 如果参与者处于会议厅中。</span><span class="sxs-lookup"><span data-stu-id="db51b-143">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="db51b-144">isMuted</span><span class="sxs-lookup"><span data-stu-id="db51b-144">isMuted</span></span>              | <span data-ttu-id="db51b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="db51b-145">Boolean</span></span>                                  | <span data-ttu-id="db51b-146">`true` 如果与会者已静音 (客户端或服务器) 。</span><span class="sxs-lookup"><span data-stu-id="db51b-146">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="db51b-147">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="db51b-147">mediaStreams</span></span>         | <span data-ttu-id="db51b-148">[mediaStream](mediastream.md) 集合</span><span class="sxs-lookup"><span data-stu-id="db51b-148">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="db51b-149">媒体流的列表。</span><span class="sxs-lookup"><span data-stu-id="db51b-149">The list of media streams.</span></span>                                   |
| <span data-ttu-id="db51b-150">metadata</span><span class="sxs-lookup"><span data-stu-id="db51b-150">metadata</span></span>             | <span data-ttu-id="db51b-151">String</span><span class="sxs-lookup"><span data-stu-id="db51b-151">String</span></span>                                   | <span data-ttu-id="db51b-152">名单中参与者提供的数据的 blob。</span><span class="sxs-lookup"><span data-stu-id="db51b-152">A blob of data provided by the participant in the roster.</span></span>     |
| <span data-ttu-id="db51b-153">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="db51b-153">recordingInfo</span></span>        | [<span data-ttu-id="db51b-154">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="db51b-154">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="db51b-155">有关参与者是否有录制功能的信息。</span><span class="sxs-lookup"><span data-stu-id="db51b-155">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="db51b-156">关系</span><span class="sxs-lookup"><span data-stu-id="db51b-156">Relationships</span></span>
<span data-ttu-id="db51b-157">无。</span><span class="sxs-lookup"><span data-stu-id="db51b-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="db51b-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db51b-158">JSON representation</span></span>

<span data-ttu-id="db51b-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db51b-159">The following is a JSON representation of the resource.</span></span>

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
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ],
  "metadata": "String",
  "recordingInfo": { "@odata.type": "#microsoft.graph.recordingInfo" }
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


