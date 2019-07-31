---
title: 参与者资源类型
description: 参与者类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a903eb34191401100d9b19aa17eba6fb9f5c6617
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009214"
---
# <a name="participant-resource-type"></a><span data-ttu-id="2dc99-103">参与者资源类型</span><span class="sxs-lookup"><span data-stu-id="2dc99-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dc99-104">参与者类型。</span><span class="sxs-lookup"><span data-stu-id="2dc99-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="2dc99-105">方法</span><span class="sxs-lookup"><span data-stu-id="2dc99-105">Methods</span></span>

| <span data-ttu-id="2dc99-106">方法</span><span class="sxs-lookup"><span data-stu-id="2dc99-106">Method</span></span>                                                          | <span data-ttu-id="2dc99-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="2dc99-107">Return Type</span></span>                              | <span data-ttu-id="2dc99-108">说明</span><span class="sxs-lookup"><span data-stu-id="2dc99-108">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="2dc99-109">获取参与者</span><span class="sxs-lookup"><span data-stu-id="2dc99-109">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="2dc99-110">参与者</span><span class="sxs-lookup"><span data-stu-id="2dc99-110">participant</span></span>](participant.md)            | <span data-ttu-id="2dc99-111">读取**参与者**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2dc99-111">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="2dc99-112">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="2dc99-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="2dc99-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="2dc99-113">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="2dc99-114">配置参与者音频混合器。</span><span class="sxs-lookup"><span data-stu-id="2dc99-114">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="2dc99-115">邀请</span><span class="sxs-lookup"><span data-stu-id="2dc99-115">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="2dc99-116">commsOperation</span><span class="sxs-lookup"><span data-stu-id="2dc99-116">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="2dc99-117">邀请参与者加入呼叫。</span><span class="sxs-lookup"><span data-stu-id="2dc99-117">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="2dc99-118">参与者静音</span><span class="sxs-lookup"><span data-stu-id="2dc99-118">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="2dc99-119">commsOperation</span><span class="sxs-lookup"><span data-stu-id="2dc99-119">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="2dc99-120">将呼叫中的参与者静音。</span><span class="sxs-lookup"><span data-stu-id="2dc99-120">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="2dc99-121">为所有参与者静音</span><span class="sxs-lookup"><span data-stu-id="2dc99-121">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="2dc99-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="2dc99-122">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="2dc99-123">将会议中的所有参与者设为静音。</span><span class="sxs-lookup"><span data-stu-id="2dc99-123">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="2dc99-124">属性</span><span class="sxs-lookup"><span data-stu-id="2dc99-124">Properties</span></span>

| <span data-ttu-id="2dc99-125">属性</span><span class="sxs-lookup"><span data-stu-id="2dc99-125">Property</span></span>             | <span data-ttu-id="2dc99-126">类型</span><span class="sxs-lookup"><span data-stu-id="2dc99-126">Type</span></span>                                     | <span data-ttu-id="2dc99-127">说明</span><span class="sxs-lookup"><span data-stu-id="2dc99-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="2dc99-128">id</span><span class="sxs-lookup"><span data-stu-id="2dc99-128">id</span></span>                   | <span data-ttu-id="2dc99-129">String</span><span class="sxs-lookup"><span data-stu-id="2dc99-129">String</span></span>                                   | <span data-ttu-id="2dc99-130">参与者 id。</span><span class="sxs-lookup"><span data-stu-id="2dc99-130">The participant id.</span></span>                                          |
| <span data-ttu-id="2dc99-131">info</span><span class="sxs-lookup"><span data-stu-id="2dc99-131">info</span></span>                 | [<span data-ttu-id="2dc99-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="2dc99-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="2dc99-133">参与者的参与者。</span><span class="sxs-lookup"><span data-stu-id="2dc99-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="2dc99-134">isInLobby</span><span class="sxs-lookup"><span data-stu-id="2dc99-134">isInLobby</span></span>            | <span data-ttu-id="2dc99-135">boolean</span><span class="sxs-lookup"><span data-stu-id="2dc99-135">boolean</span></span>                                  | <span data-ttu-id="2dc99-136">如果参与者在会议厅中, 则为 true</span><span class="sxs-lookup"><span data-stu-id="2dc99-136">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="2dc99-137">isMuted</span><span class="sxs-lookup"><span data-stu-id="2dc99-137">isMuted</span></span>              | <span data-ttu-id="2dc99-138">boolean</span><span class="sxs-lookup"><span data-stu-id="2dc99-138">boolean</span></span>                                  | <span data-ttu-id="2dc99-139">如果参与者处于静音 (客户端或服务器为静音)</span><span class="sxs-lookup"><span data-stu-id="2dc99-139">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="2dc99-140">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="2dc99-140">mediaStreams</span></span>         | <span data-ttu-id="2dc99-141">[mediaStream](mediastream.md)集合</span><span class="sxs-lookup"><span data-stu-id="2dc99-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="2dc99-142">媒体流的列表。</span><span class="sxs-lookup"><span data-stu-id="2dc99-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="2dc99-143">metadata</span><span class="sxs-lookup"><span data-stu-id="2dc99-143">metadata</span></span>             | <span data-ttu-id="2dc99-144">String</span><span class="sxs-lookup"><span data-stu-id="2dc99-144">String</span></span>                                   | <span data-ttu-id="2dc99-145">名单中的参与者提供的数据 blob</span><span class="sxs-lookup"><span data-stu-id="2dc99-145">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="2dc99-146">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="2dc99-146">recordingInfo</span></span>        | [<span data-ttu-id="2dc99-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="2dc99-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="2dc99-148">有关参与者是否有录制功能的信息。</span><span class="sxs-lookup"><span data-stu-id="2dc99-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2dc99-149">关系</span><span class="sxs-lookup"><span data-stu-id="2dc99-149">Relationships</span></span>
<span data-ttu-id="2dc99-150">无</span><span class="sxs-lookup"><span data-stu-id="2dc99-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2dc99-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2dc99-151">JSON representation</span></span>

<span data-ttu-id="2dc99-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2dc99-152">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="2dc99-153">示例</span><span class="sxs-lookup"><span data-stu-id="2dc99-153">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus"
  },
  "isInLobby": false,
  "isMuted": false,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "status": "recordingCapable"
  }
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
