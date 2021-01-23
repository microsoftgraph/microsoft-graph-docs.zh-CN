---
title: 参与者资源类型
description: 表示参与者类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 99f165f2f3e99ab424a318b053a060ccda8fdc1c
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943715"
---
# <a name="participant-resource-type"></a><span data-ttu-id="5aea6-103">参与者资源类型</span><span class="sxs-lookup"><span data-stu-id="5aea6-103">participant resource type</span></span>

<span data-ttu-id="5aea6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aea6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5aea6-105">代表通话中的参与者。</span><span class="sxs-lookup"><span data-stu-id="5aea6-105">Represents a participant in a call.</span></span>

## <a name="methods"></a><span data-ttu-id="5aea6-106">方法</span><span class="sxs-lookup"><span data-stu-id="5aea6-106">Methods</span></span>

| <span data-ttu-id="5aea6-107">方法</span><span class="sxs-lookup"><span data-stu-id="5aea6-107">Method</span></span>                                                 | <span data-ttu-id="5aea6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="5aea6-108">Return Type</span></span>                                                 | <span data-ttu-id="5aea6-109">说明</span><span class="sxs-lookup"><span data-stu-id="5aea6-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="5aea6-110">列出参与者</span><span class="sxs-lookup"><span data-stu-id="5aea6-110">List participant</span></span>](../api/participant-get.md)          | [<span data-ttu-id="5aea6-111">参与者</span><span class="sxs-lookup"><span data-stu-id="5aea6-111">participant</span></span>](participant.md)                               | <span data-ttu-id="5aea6-112">检索呼叫 **中的参与者** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="5aea6-112">Retrieve a list of **participant** objects in the call.</span></span> |
| [<span data-ttu-id="5aea6-113">获取参与者</span><span class="sxs-lookup"><span data-stu-id="5aea6-113">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="5aea6-114">参与者</span><span class="sxs-lookup"><span data-stu-id="5aea6-114">participant</span></span>](participant.md)                               | <span data-ttu-id="5aea6-115">读取参与者 **对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="5aea6-115">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="5aea6-116">删除参与者</span><span class="sxs-lookup"><span data-stu-id="5aea6-116">Delete participant</span></span>](../api/participant-delete.md)         | <span data-ttu-id="5aea6-117">无</span><span class="sxs-lookup"><span data-stu-id="5aea6-117">None</span></span>   | <span data-ttu-id="5aea6-118">删除通话中的参与者。</span><span class="sxs-lookup"><span data-stu-id="5aea6-118">Delete a participant in a call.</span></span>                  |
| [<span data-ttu-id="5aea6-119">邀请</span><span class="sxs-lookup"><span data-stu-id="5aea6-119">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="5aea6-120">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="5aea6-120">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                        | <span data-ttu-id="5aea6-121">邀请参与者加入通话。</span><span class="sxs-lookup"><span data-stu-id="5aea6-121">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="5aea6-122">参与者静音</span><span class="sxs-lookup"><span data-stu-id="5aea6-122">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="5aea6-123">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="5aea6-123">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="5aea6-124">将呼叫中的参与者静音。</span><span class="sxs-lookup"><span data-stu-id="5aea6-124">Mute a participant in a call.</span></span>                  |

## <a name="properties"></a><span data-ttu-id="5aea6-125">属性</span><span class="sxs-lookup"><span data-stu-id="5aea6-125">Properties</span></span>

| <span data-ttu-id="5aea6-126">属性</span><span class="sxs-lookup"><span data-stu-id="5aea6-126">Property</span></span>             | <span data-ttu-id="5aea6-127">类型</span><span class="sxs-lookup"><span data-stu-id="5aea6-127">Type</span></span>                                     | <span data-ttu-id="5aea6-128">说明</span><span class="sxs-lookup"><span data-stu-id="5aea6-128">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="5aea6-129">id</span><span class="sxs-lookup"><span data-stu-id="5aea6-129">id</span></span>                   | <span data-ttu-id="5aea6-130">String</span><span class="sxs-lookup"><span data-stu-id="5aea6-130">String</span></span>                                   | <span data-ttu-id="5aea6-131">参与者 ID。</span><span class="sxs-lookup"><span data-stu-id="5aea6-131">The participant ID.</span></span>                                          |
| <span data-ttu-id="5aea6-132">info</span><span class="sxs-lookup"><span data-stu-id="5aea6-132">info</span></span>                 | [<span data-ttu-id="5aea6-133">participantInfo</span><span class="sxs-lookup"><span data-stu-id="5aea6-133">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="5aea6-134">有关参与者的信息。</span><span class="sxs-lookup"><span data-stu-id="5aea6-134">Information about the participant.</span></span>                          |
| <span data-ttu-id="5aea6-135">isInLobby</span><span class="sxs-lookup"><span data-stu-id="5aea6-135">isInLobby</span></span>            | <span data-ttu-id="5aea6-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="5aea6-136">Boolean</span></span>                                  | <span data-ttu-id="5aea6-137">`true` 如果参与者在大厅中。</span><span class="sxs-lookup"><span data-stu-id="5aea6-137">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="5aea6-138">isMuted</span><span class="sxs-lookup"><span data-stu-id="5aea6-138">isMuted</span></span>              | <span data-ttu-id="5aea6-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="5aea6-139">Boolean</span></span>                                  | <span data-ttu-id="5aea6-140">`true` 如果参与者在客户端或服务器 (静音，则) 。</span><span class="sxs-lookup"><span data-stu-id="5aea6-140">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="5aea6-141">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="5aea6-141">mediaStreams</span></span>         | <span data-ttu-id="5aea6-142">[mediaStream](mediastream.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5aea6-142">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="5aea6-143">媒体流的列表。</span><span class="sxs-lookup"><span data-stu-id="5aea6-143">The list of media streams.</span></span>                                   |
| <span data-ttu-id="5aea6-144">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="5aea6-144">recordingInfo</span></span>        | [<span data-ttu-id="5aea6-145">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="5aea6-145">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="5aea6-146">有关参与者是否具有录制功能的信息。</span><span class="sxs-lookup"><span data-stu-id="5aea6-146">Information about whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5aea6-147">关系</span><span class="sxs-lookup"><span data-stu-id="5aea6-147">Relationships</span></span>
<span data-ttu-id="5aea6-148">无。</span><span class="sxs-lookup"><span data-stu-id="5aea6-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5aea6-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5aea6-149">JSON representation</span></span>

<span data-ttu-id="5aea6-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5aea6-150">The following is a JSON representation of the resource.</span></span>

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

