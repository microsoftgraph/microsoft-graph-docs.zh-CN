---
title: 参与者资源类型
description: 参与者类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d76dd0643d76d5899c5f46dceee6a5ecca21f389
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866656"
---
# <a name="participant-resource-type"></a><span data-ttu-id="10ba5-103">参与者资源类型</span><span class="sxs-lookup"><span data-stu-id="10ba5-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10ba5-104">参与者类型。</span><span class="sxs-lookup"><span data-stu-id="10ba5-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="10ba5-105">方法</span><span class="sxs-lookup"><span data-stu-id="10ba5-105">Methods</span></span>

| <span data-ttu-id="10ba5-106">方法</span><span class="sxs-lookup"><span data-stu-id="10ba5-106">Method</span></span>                                                 | <span data-ttu-id="10ba5-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="10ba5-107">Return Type</span></span>                                                 | <span data-ttu-id="10ba5-108">说明</span><span class="sxs-lookup"><span data-stu-id="10ba5-108">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="10ba5-109">获取参与者</span><span class="sxs-lookup"><span data-stu-id="10ba5-109">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="10ba5-110">参与者</span><span class="sxs-lookup"><span data-stu-id="10ba5-110">participant</span></span>](participant.md)                               | <span data-ttu-id="10ba5-111">读取**参与者**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="10ba5-111">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="10ba5-112">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="10ba5-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md) | [<span data-ttu-id="10ba5-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="10ba5-113">commsOperation</span></span>](commsoperation.md)                         | <span data-ttu-id="10ba5-114">配置参与者音频混合器。</span><span class="sxs-lookup"><span data-stu-id="10ba5-114">Configure the participant audio mixer.</span></span>         |
| [<span data-ttu-id="10ba5-115">邀请</span><span class="sxs-lookup"><span data-stu-id="10ba5-115">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="10ba5-116">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="10ba5-116">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                         | <span data-ttu-id="10ba5-117">邀请参与者加入呼叫。</span><span class="sxs-lookup"><span data-stu-id="10ba5-117">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="10ba5-118">参与者静音</span><span class="sxs-lookup"><span data-stu-id="10ba5-118">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="10ba5-119">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="10ba5-119">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="10ba5-120">将呼叫中的参与者静音。</span><span class="sxs-lookup"><span data-stu-id="10ba5-120">Mute a participant in a call.</span></span>                  |
| [<span data-ttu-id="10ba5-121">所有参与者静音</span><span class="sxs-lookup"><span data-stu-id="10ba5-121">Mute all participants</span></span>](../api/participant-muteall.md) | [<span data-ttu-id="10ba5-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="10ba5-122">commsOperation</span></span>](commsoperation.md) | <span data-ttu-id="10ba5-123">将会议中的所有参与者设为静音。</span><span class="sxs-lookup"><span data-stu-id="10ba5-123">Mute all the participants in the meeting.</span></span>      |

## <a name="properties"></a><span data-ttu-id="10ba5-124">属性</span><span class="sxs-lookup"><span data-stu-id="10ba5-124">Properties</span></span>

| <span data-ttu-id="10ba5-125">属性</span><span class="sxs-lookup"><span data-stu-id="10ba5-125">Property</span></span>             | <span data-ttu-id="10ba5-126">类型</span><span class="sxs-lookup"><span data-stu-id="10ba5-126">Type</span></span>                                     | <span data-ttu-id="10ba5-127">说明</span><span class="sxs-lookup"><span data-stu-id="10ba5-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="10ba5-128">id</span><span class="sxs-lookup"><span data-stu-id="10ba5-128">id</span></span>                   | <span data-ttu-id="10ba5-129">String</span><span class="sxs-lookup"><span data-stu-id="10ba5-129">String</span></span>                                   | <span data-ttu-id="10ba5-130">参与者 ID。</span><span class="sxs-lookup"><span data-stu-id="10ba5-130">The participant ID.</span></span>                                          |
| <span data-ttu-id="10ba5-131">info</span><span class="sxs-lookup"><span data-stu-id="10ba5-131">info</span></span>                 | [<span data-ttu-id="10ba5-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="10ba5-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="10ba5-133">参与者的参与者。</span><span class="sxs-lookup"><span data-stu-id="10ba5-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="10ba5-134">isInLobby</span><span class="sxs-lookup"><span data-stu-id="10ba5-134">isInLobby</span></span>            | <span data-ttu-id="10ba5-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="10ba5-135">Boolean</span></span>                                  | <span data-ttu-id="10ba5-136">`true`如果参与者处于会议厅中。</span><span class="sxs-lookup"><span data-stu-id="10ba5-136">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="10ba5-137">isMuted</span><span class="sxs-lookup"><span data-stu-id="10ba5-137">isMuted</span></span>              | <span data-ttu-id="10ba5-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="10ba5-138">Boolean</span></span>                                  | <span data-ttu-id="10ba5-139">`true`如果参与者处于静音（客户端或服务器为静音）。</span><span class="sxs-lookup"><span data-stu-id="10ba5-139">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="10ba5-140">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="10ba5-140">mediaStreams</span></span>         | <span data-ttu-id="10ba5-141">[mediaStream](mediastream.md)集合</span><span class="sxs-lookup"><span data-stu-id="10ba5-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="10ba5-142">媒体流的列表。</span><span class="sxs-lookup"><span data-stu-id="10ba5-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="10ba5-143">metadata</span><span class="sxs-lookup"><span data-stu-id="10ba5-143">metadata</span></span>             | <span data-ttu-id="10ba5-144">String</span><span class="sxs-lookup"><span data-stu-id="10ba5-144">String</span></span>                                   | <span data-ttu-id="10ba5-145">名单中参与者提供的数据的 blob。</span><span class="sxs-lookup"><span data-stu-id="10ba5-145">A blob of data provided by the participant in the roster.</span></span>     |
| <span data-ttu-id="10ba5-146">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="10ba5-146">recordingInfo</span></span>        | [<span data-ttu-id="10ba5-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="10ba5-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="10ba5-148">有关参与者是否有录制功能的信息。</span><span class="sxs-lookup"><span data-stu-id="10ba5-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="10ba5-149">关系</span><span class="sxs-lookup"><span data-stu-id="10ba5-149">Relationships</span></span>
<span data-ttu-id="10ba5-150">无。</span><span class="sxs-lookup"><span data-stu-id="10ba5-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10ba5-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10ba5-151">JSON representation</span></span>

<span data-ttu-id="10ba5-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10ba5-152">The following is a JSON representation of the resource.</span></span>

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
