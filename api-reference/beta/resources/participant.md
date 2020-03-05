---
title: 参与者资源类型
description: 参与者类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6ae920e35c3ba7c2b31c5947f15b3e9d6585a21c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522037"
---
# <a name="participant-resource-type"></a><span data-ttu-id="eb5a1-103">参与者资源类型</span><span class="sxs-lookup"><span data-stu-id="eb5a1-103">participant resource type</span></span>

<span data-ttu-id="eb5a1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="eb5a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb5a1-105">参与者类型。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-105">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="eb5a1-106">方法</span><span class="sxs-lookup"><span data-stu-id="eb5a1-106">Methods</span></span>

| <span data-ttu-id="eb5a1-107">方法</span><span class="sxs-lookup"><span data-stu-id="eb5a1-107">Method</span></span>                                                 | <span data-ttu-id="eb5a1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="eb5a1-108">Return Type</span></span>                                                 | <span data-ttu-id="eb5a1-109">说明</span><span class="sxs-lookup"><span data-stu-id="eb5a1-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="eb5a1-110">获取参与者</span><span class="sxs-lookup"><span data-stu-id="eb5a1-110">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="eb5a1-111">参与者</span><span class="sxs-lookup"><span data-stu-id="eb5a1-111">participant</span></span>](participant.md)                               | <span data-ttu-id="eb5a1-112">读取**参与者**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-112">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="eb5a1-113">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="eb5a1-113">ConfigureMixer</span></span>](../api/participant-configuremixer.md) | [<span data-ttu-id="eb5a1-114">commsOperation</span><span class="sxs-lookup"><span data-stu-id="eb5a1-114">commsOperation</span></span>](commsoperation.md)                         | <span data-ttu-id="eb5a1-115">配置参与者音频混合器。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-115">Configure the participant audio mixer.</span></span>         |
| [<span data-ttu-id="eb5a1-116">邀请</span><span class="sxs-lookup"><span data-stu-id="eb5a1-116">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="eb5a1-117">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="eb5a1-117">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                         | <span data-ttu-id="eb5a1-118">邀请参与者加入呼叫。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-118">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="eb5a1-119">参与者静音</span><span class="sxs-lookup"><span data-stu-id="eb5a1-119">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="eb5a1-120">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="eb5a1-120">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="eb5a1-121">将呼叫中的参与者静音。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-121">Mute a participant in a call.</span></span>                  |
| [<span data-ttu-id="eb5a1-122">所有参与者静音</span><span class="sxs-lookup"><span data-stu-id="eb5a1-122">Mute all participants</span></span>](../api/participant-muteall.md) | [<span data-ttu-id="eb5a1-123">commsOperation</span><span class="sxs-lookup"><span data-stu-id="eb5a1-123">commsOperation</span></span>](commsoperation.md) | <span data-ttu-id="eb5a1-124">将会议中的所有参与者设为静音。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-124">Mute all the participants in the meeting.</span></span>      |

## <a name="properties"></a><span data-ttu-id="eb5a1-125">属性</span><span class="sxs-lookup"><span data-stu-id="eb5a1-125">Properties</span></span>

| <span data-ttu-id="eb5a1-126">属性</span><span class="sxs-lookup"><span data-stu-id="eb5a1-126">Property</span></span>             | <span data-ttu-id="eb5a1-127">类型</span><span class="sxs-lookup"><span data-stu-id="eb5a1-127">Type</span></span>                                     | <span data-ttu-id="eb5a1-128">说明</span><span class="sxs-lookup"><span data-stu-id="eb5a1-128">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="eb5a1-129">id</span><span class="sxs-lookup"><span data-stu-id="eb5a1-129">id</span></span>                   | <span data-ttu-id="eb5a1-130">String</span><span class="sxs-lookup"><span data-stu-id="eb5a1-130">String</span></span>                                   | <span data-ttu-id="eb5a1-131">参与者 ID。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-131">The participant ID.</span></span>                                          |
| <span data-ttu-id="eb5a1-132">info</span><span class="sxs-lookup"><span data-stu-id="eb5a1-132">info</span></span>                 | [<span data-ttu-id="eb5a1-133">participantInfo</span><span class="sxs-lookup"><span data-stu-id="eb5a1-133">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="eb5a1-134">参与者的参与者。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-134">The participant of the participant.</span></span>                          |
| <span data-ttu-id="eb5a1-135">isInLobby</span><span class="sxs-lookup"><span data-stu-id="eb5a1-135">isInLobby</span></span>            | <span data-ttu-id="eb5a1-136">布尔</span><span class="sxs-lookup"><span data-stu-id="eb5a1-136">Boolean</span></span>                                  | <span data-ttu-id="eb5a1-137">`true`如果参与者处于会议厅中。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-137">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="eb5a1-138">isMuted</span><span class="sxs-lookup"><span data-stu-id="eb5a1-138">isMuted</span></span>              | <span data-ttu-id="eb5a1-139">布尔</span><span class="sxs-lookup"><span data-stu-id="eb5a1-139">Boolean</span></span>                                  | <span data-ttu-id="eb5a1-140">`true`如果参与者处于静音（客户端或服务器为静音）。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-140">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="eb5a1-141">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="eb5a1-141">mediaStreams</span></span>         | <span data-ttu-id="eb5a1-142">[mediaStream](mediastream.md)集合</span><span class="sxs-lookup"><span data-stu-id="eb5a1-142">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="eb5a1-143">媒体流的列表。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-143">The list of media streams.</span></span>                                   |
| <span data-ttu-id="eb5a1-144">metadata</span><span class="sxs-lookup"><span data-stu-id="eb5a1-144">metadata</span></span>             | <span data-ttu-id="eb5a1-145">String</span><span class="sxs-lookup"><span data-stu-id="eb5a1-145">String</span></span>                                   | <span data-ttu-id="eb5a1-146">名单中参与者提供的数据的 blob。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-146">A blob of data provided by the participant in the roster.</span></span>     |
| <span data-ttu-id="eb5a1-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="eb5a1-147">recordingInfo</span></span>        | [<span data-ttu-id="eb5a1-148">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="eb5a1-148">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="eb5a1-149">有关参与者是否有录制功能的信息。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-149">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="eb5a1-150">关系</span><span class="sxs-lookup"><span data-stu-id="eb5a1-150">Relationships</span></span>
<span data-ttu-id="eb5a1-151">无。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb5a1-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb5a1-152">JSON representation</span></span>

<span data-ttu-id="eb5a1-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb5a1-153">The following is a JSON representation of the resource.</span></span>

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
