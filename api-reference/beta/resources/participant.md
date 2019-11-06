---
title: 参与者资源类型
description: 参与者类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e2fae206fb76ffe3c00b91d992c874e200eeae98
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006597"
---
# <a name="participant-resource-type"></a><span data-ttu-id="8978e-103">参与者资源类型</span><span class="sxs-lookup"><span data-stu-id="8978e-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8978e-104">参与者类型。</span><span class="sxs-lookup"><span data-stu-id="8978e-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="8978e-105">Methods</span><span class="sxs-lookup"><span data-stu-id="8978e-105">Methods</span></span>

| <span data-ttu-id="8978e-106">方法</span><span class="sxs-lookup"><span data-stu-id="8978e-106">Method</span></span>                                                          | <span data-ttu-id="8978e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="8978e-107">Return Type</span></span>                              | <span data-ttu-id="8978e-108">说明</span><span class="sxs-lookup"><span data-stu-id="8978e-108">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="8978e-109">获取参与者</span><span class="sxs-lookup"><span data-stu-id="8978e-109">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="8978e-110">参与者</span><span class="sxs-lookup"><span data-stu-id="8978e-110">participant</span></span>](participant.md)            | <span data-ttu-id="8978e-111">读取**参与者**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8978e-111">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="8978e-112">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="8978e-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="8978e-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8978e-113">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8978e-114">配置参与者音频混合器。</span><span class="sxs-lookup"><span data-stu-id="8978e-114">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="8978e-115">邀请</span><span class="sxs-lookup"><span data-stu-id="8978e-115">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="8978e-116">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8978e-116">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8978e-117">邀请参与者加入呼叫。</span><span class="sxs-lookup"><span data-stu-id="8978e-117">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="8978e-118">静音参与者</span><span class="sxs-lookup"><span data-stu-id="8978e-118">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="8978e-119">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8978e-119">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8978e-120">将呼叫中的参与者静音。</span><span class="sxs-lookup"><span data-stu-id="8978e-120">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="8978e-121">为所有参与者静音</span><span class="sxs-lookup"><span data-stu-id="8978e-121">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="8978e-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8978e-122">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8978e-123">将会议中的所有参与者设为静音。</span><span class="sxs-lookup"><span data-stu-id="8978e-123">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="8978e-124">属性</span><span class="sxs-lookup"><span data-stu-id="8978e-124">Properties</span></span>

| <span data-ttu-id="8978e-125">属性</span><span class="sxs-lookup"><span data-stu-id="8978e-125">Property</span></span>             | <span data-ttu-id="8978e-126">类型</span><span class="sxs-lookup"><span data-stu-id="8978e-126">Type</span></span>                                     | <span data-ttu-id="8978e-127">说明</span><span class="sxs-lookup"><span data-stu-id="8978e-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="8978e-128">id</span><span class="sxs-lookup"><span data-stu-id="8978e-128">id</span></span>                   | <span data-ttu-id="8978e-129">String</span><span class="sxs-lookup"><span data-stu-id="8978e-129">String</span></span>                                   | <span data-ttu-id="8978e-130">参与者 id。</span><span class="sxs-lookup"><span data-stu-id="8978e-130">The participant id.</span></span>                                          |
| <span data-ttu-id="8978e-131">info</span><span class="sxs-lookup"><span data-stu-id="8978e-131">info</span></span>                 | [<span data-ttu-id="8978e-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="8978e-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="8978e-133">参与者的参与者。</span><span class="sxs-lookup"><span data-stu-id="8978e-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="8978e-134">isInLobby</span><span class="sxs-lookup"><span data-stu-id="8978e-134">isInLobby</span></span>            | <span data-ttu-id="8978e-135">boolean</span><span class="sxs-lookup"><span data-stu-id="8978e-135">boolean</span></span>                                  | <span data-ttu-id="8978e-136">如果参与者在会议厅中，则为 true</span><span class="sxs-lookup"><span data-stu-id="8978e-136">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="8978e-137">isMuted</span><span class="sxs-lookup"><span data-stu-id="8978e-137">isMuted</span></span>              | <span data-ttu-id="8978e-138">boolean</span><span class="sxs-lookup"><span data-stu-id="8978e-138">boolean</span></span>                                  | <span data-ttu-id="8978e-139">如果参与者处于静音（客户端或服务器为静音）</span><span class="sxs-lookup"><span data-stu-id="8978e-139">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="8978e-140">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="8978e-140">mediaStreams</span></span>         | <span data-ttu-id="8978e-141">[mediaStream](mediastream.md)集合</span><span class="sxs-lookup"><span data-stu-id="8978e-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="8978e-142">媒体流的列表。</span><span class="sxs-lookup"><span data-stu-id="8978e-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="8978e-143">metadata</span><span class="sxs-lookup"><span data-stu-id="8978e-143">metadata</span></span>             | <span data-ttu-id="8978e-144">String</span><span class="sxs-lookup"><span data-stu-id="8978e-144">String</span></span>                                   | <span data-ttu-id="8978e-145">名单中的参与者提供的数据 blob</span><span class="sxs-lookup"><span data-stu-id="8978e-145">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="8978e-146">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="8978e-146">recordingInfo</span></span>        | [<span data-ttu-id="8978e-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="8978e-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="8978e-148">有关参与者是否有录制功能的信息。</span><span class="sxs-lookup"><span data-stu-id="8978e-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8978e-149">关系</span><span class="sxs-lookup"><span data-stu-id="8978e-149">Relationships</span></span>
<span data-ttu-id="8978e-150">无</span><span class="sxs-lookup"><span data-stu-id="8978e-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8978e-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8978e-151">JSON representation</span></span>

<span data-ttu-id="8978e-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8978e-152">The following is a JSON representation of the resource.</span></span>

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
