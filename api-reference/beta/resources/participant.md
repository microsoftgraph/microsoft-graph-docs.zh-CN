---
title: 参与者资源类型
description: 参与者类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dc1038e80566cab0ce37eaa40b4f5c391a625824
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943722"
---
# <a name="participant-resource-type"></a><span data-ttu-id="9be6a-103">参与者资源类型</span><span class="sxs-lookup"><span data-stu-id="9be6a-103">participant resource type</span></span>

<span data-ttu-id="9be6a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9be6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9be6a-105">代表通话中的参与者。</span><span class="sxs-lookup"><span data-stu-id="9be6a-105">Represents a participant in a call.</span></span>

## <a name="methods"></a><span data-ttu-id="9be6a-106">方法</span><span class="sxs-lookup"><span data-stu-id="9be6a-106">Methods</span></span>

| <span data-ttu-id="9be6a-107">方法</span><span class="sxs-lookup"><span data-stu-id="9be6a-107">Method</span></span>                                                 | <span data-ttu-id="9be6a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9be6a-108">Return Type</span></span>                                                 | <span data-ttu-id="9be6a-109">说明</span><span class="sxs-lookup"><span data-stu-id="9be6a-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="9be6a-110">列出参与者</span><span class="sxs-lookup"><span data-stu-id="9be6a-110">List participant</span></span>](../api/participant-get.md)         | [<span data-ttu-id="9be6a-111">参与者</span><span class="sxs-lookup"><span data-stu-id="9be6a-111">participant</span></span>](participant.md)                               | <span data-ttu-id="9be6a-112">检索呼叫 **中的参与者** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="9be6a-112">Retrieve a list of **participant** objects in the call.</span></span> |
| [<span data-ttu-id="9be6a-113">获取参与者</span><span class="sxs-lookup"><span data-stu-id="9be6a-113">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="9be6a-114">参与者</span><span class="sxs-lookup"><span data-stu-id="9be6a-114">participant</span></span>](participant.md)                               | <span data-ttu-id="9be6a-115">读取参与者 **对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="9be6a-115">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="9be6a-116">删除参与者</span><span class="sxs-lookup"><span data-stu-id="9be6a-116">Delete participant</span></span>](../api/participant-delete.md)     | <span data-ttu-id="9be6a-117">无</span><span class="sxs-lookup"><span data-stu-id="9be6a-117">None</span></span>   | <span data-ttu-id="9be6a-118">删除通话中的参与者。</span><span class="sxs-lookup"><span data-stu-id="9be6a-118">Delete a participant in a call.</span></span>                  |
| [<span data-ttu-id="9be6a-119">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="9be6a-119">ConfigureMixer</span></span>](../api/participant-configuremixer.md) | [<span data-ttu-id="9be6a-120">commsOperation</span><span class="sxs-lookup"><span data-stu-id="9be6a-120">commsOperation</span></span>](commsoperation.md)                         | <span data-ttu-id="9be6a-121">配置参与者音频混合器。</span><span class="sxs-lookup"><span data-stu-id="9be6a-121">Configure the participant audio mixer.</span></span>         |
| [<span data-ttu-id="9be6a-122">邀请</span><span class="sxs-lookup"><span data-stu-id="9be6a-122">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="9be6a-123">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="9be6a-123">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                         | <span data-ttu-id="9be6a-124">邀请参与者加入通话。</span><span class="sxs-lookup"><span data-stu-id="9be6a-124">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="9be6a-125">参与者静音</span><span class="sxs-lookup"><span data-stu-id="9be6a-125">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="9be6a-126">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="9be6a-126">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="9be6a-127">将呼叫中的参与者静音。</span><span class="sxs-lookup"><span data-stu-id="9be6a-127">Mute a participant in a call.</span></span>                  |
| [<span data-ttu-id="9be6a-128">所有参与者静音</span><span class="sxs-lookup"><span data-stu-id="9be6a-128">Mute all participants</span></span>](../api/participant-muteall.md) | [<span data-ttu-id="9be6a-129">commsOperation</span><span class="sxs-lookup"><span data-stu-id="9be6a-129">commsOperation</span></span>](commsoperation.md) | <span data-ttu-id="9be6a-130">将会议的所有参与者静音。</span><span class="sxs-lookup"><span data-stu-id="9be6a-130">Mute all the participants in the meeting.</span></span>      |

## <a name="properties"></a><span data-ttu-id="9be6a-131">属性</span><span class="sxs-lookup"><span data-stu-id="9be6a-131">Properties</span></span>

| <span data-ttu-id="9be6a-132">属性</span><span class="sxs-lookup"><span data-stu-id="9be6a-132">Property</span></span>             | <span data-ttu-id="9be6a-133">类型</span><span class="sxs-lookup"><span data-stu-id="9be6a-133">Type</span></span>                                     | <span data-ttu-id="9be6a-134">说明</span><span class="sxs-lookup"><span data-stu-id="9be6a-134">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="9be6a-135">id</span><span class="sxs-lookup"><span data-stu-id="9be6a-135">id</span></span>                   | <span data-ttu-id="9be6a-136">String</span><span class="sxs-lookup"><span data-stu-id="9be6a-136">String</span></span>                                   | <span data-ttu-id="9be6a-137">参与者 ID。</span><span class="sxs-lookup"><span data-stu-id="9be6a-137">The participant ID.</span></span>                                          |
| <span data-ttu-id="9be6a-138">info</span><span class="sxs-lookup"><span data-stu-id="9be6a-138">info</span></span>                 | [<span data-ttu-id="9be6a-139">participantInfo</span><span class="sxs-lookup"><span data-stu-id="9be6a-139">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="9be6a-140">有关参与者的信息。</span><span class="sxs-lookup"><span data-stu-id="9be6a-140">Information about the participant.</span></span>                          |
| <span data-ttu-id="9be6a-141">isInLobby</span><span class="sxs-lookup"><span data-stu-id="9be6a-141">isInLobby</span></span>            | <span data-ttu-id="9be6a-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be6a-142">Boolean</span></span>                                  | <span data-ttu-id="9be6a-143">`true` 如果参与者在大厅中。</span><span class="sxs-lookup"><span data-stu-id="9be6a-143">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="9be6a-144">isMuted</span><span class="sxs-lookup"><span data-stu-id="9be6a-144">isMuted</span></span>              | <span data-ttu-id="9be6a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be6a-145">Boolean</span></span>                                  | <span data-ttu-id="9be6a-146">`true` 如果参与者在客户端或服务器 (静音，则) 。</span><span class="sxs-lookup"><span data-stu-id="9be6a-146">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="9be6a-147">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="9be6a-147">mediaStreams</span></span>         | <span data-ttu-id="9be6a-148">[mediaStream](mediastream.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9be6a-148">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="9be6a-149">媒体流的列表。</span><span class="sxs-lookup"><span data-stu-id="9be6a-149">The list of media streams.</span></span>                                   |
| <span data-ttu-id="9be6a-150">metadata</span><span class="sxs-lookup"><span data-stu-id="9be6a-150">metadata</span></span>             | <span data-ttu-id="9be6a-151">String</span><span class="sxs-lookup"><span data-stu-id="9be6a-151">String</span></span>                                   | <span data-ttu-id="9be6a-152">名单中的参与者提供的数据 blob。</span><span class="sxs-lookup"><span data-stu-id="9be6a-152">A blob of data provided by the participant in the roster.</span></span>     |
| <span data-ttu-id="9be6a-153">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="9be6a-153">recordingInfo</span></span>        | [<span data-ttu-id="9be6a-154">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="9be6a-154">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="9be6a-155">有关参与者是否具有录制功能的信息。</span><span class="sxs-lookup"><span data-stu-id="9be6a-155">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9be6a-156">关系</span><span class="sxs-lookup"><span data-stu-id="9be6a-156">Relationships</span></span>
<span data-ttu-id="9be6a-157">无。</span><span class="sxs-lookup"><span data-stu-id="9be6a-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9be6a-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9be6a-158">JSON representation</span></span>

<span data-ttu-id="9be6a-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9be6a-159">The following is a JSON representation of the resource.</span></span>

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


