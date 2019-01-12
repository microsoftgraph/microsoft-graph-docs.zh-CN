---
title: 参与者的资源类型
description: 参与者类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d6a4474525086fb1e8aefe00ad37acaf6511e9f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938328"
---
# <a name="participant-resource-type"></a><span data-ttu-id="85b50-103">参与者的资源类型</span><span class="sxs-lookup"><span data-stu-id="85b50-103">participant resource type</span></span>

> <span data-ttu-id="85b50-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="85b50-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85b50-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="85b50-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85b50-106">参与者类型。</span><span class="sxs-lookup"><span data-stu-id="85b50-106">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="85b50-107">方法</span><span class="sxs-lookup"><span data-stu-id="85b50-107">Methods</span></span>

| <span data-ttu-id="85b50-108">方法</span><span class="sxs-lookup"><span data-stu-id="85b50-108">Method</span></span>                                                          | <span data-ttu-id="85b50-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="85b50-109">Return Type</span></span>                              | <span data-ttu-id="85b50-110">说明</span><span class="sxs-lookup"><span data-stu-id="85b50-110">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="85b50-111">获取参与者</span><span class="sxs-lookup"><span data-stu-id="85b50-111">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="85b50-112">参与者</span><span class="sxs-lookup"><span data-stu-id="85b50-112">participant</span></span>](participant.md)            | <span data-ttu-id="85b50-113">阅读**参与者**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="85b50-113">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="85b50-114">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="85b50-114">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="85b50-115">commsOperation</span><span class="sxs-lookup"><span data-stu-id="85b50-115">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="85b50-116">配置参与者音频混音器。</span><span class="sxs-lookup"><span data-stu-id="85b50-116">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="85b50-117">邀请</span><span class="sxs-lookup"><span data-stu-id="85b50-117">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="85b50-118">commsOperation</span><span class="sxs-lookup"><span data-stu-id="85b50-118">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="85b50-119">邀请参与者加入呼叫。</span><span class="sxs-lookup"><span data-stu-id="85b50-119">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="85b50-120">设置为静音的参与者</span><span class="sxs-lookup"><span data-stu-id="85b50-120">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="85b50-121">commsOperation</span><span class="sxs-lookup"><span data-stu-id="85b50-121">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="85b50-122">将呼叫中的参与者设为静音。</span><span class="sxs-lookup"><span data-stu-id="85b50-122">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="85b50-123">将所有参与者设为都静音</span><span class="sxs-lookup"><span data-stu-id="85b50-123">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="85b50-124">commsOperation</span><span class="sxs-lookup"><span data-stu-id="85b50-124">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="85b50-125">将会议中的所有参与者设为都静音。</span><span class="sxs-lookup"><span data-stu-id="85b50-125">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="85b50-126">属性</span><span class="sxs-lookup"><span data-stu-id="85b50-126">Properties</span></span>

| <span data-ttu-id="85b50-127">属性</span><span class="sxs-lookup"><span data-stu-id="85b50-127">Property</span></span>             | <span data-ttu-id="85b50-128">类型</span><span class="sxs-lookup"><span data-stu-id="85b50-128">Type</span></span>                                     | <span data-ttu-id="85b50-129">说明</span><span class="sxs-lookup"><span data-stu-id="85b50-129">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="85b50-130">id</span><span class="sxs-lookup"><span data-stu-id="85b50-130">id</span></span>                   | <span data-ttu-id="85b50-131">字符串</span><span class="sxs-lookup"><span data-stu-id="85b50-131">String</span></span>                                   | <span data-ttu-id="85b50-132">参与者的 id。</span><span class="sxs-lookup"><span data-stu-id="85b50-132">The participant id.</span></span>                                          |
| <span data-ttu-id="85b50-133">信息</span><span class="sxs-lookup"><span data-stu-id="85b50-133">info</span></span>                 | [<span data-ttu-id="85b50-134">participantInfo</span><span class="sxs-lookup"><span data-stu-id="85b50-134">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="85b50-135">参与者的参与者。</span><span class="sxs-lookup"><span data-stu-id="85b50-135">The participant of the participant.</span></span>                          |
| <span data-ttu-id="85b50-136">isInLobby</span><span class="sxs-lookup"><span data-stu-id="85b50-136">isInLobby</span></span>            | <span data-ttu-id="85b50-137">boolean</span><span class="sxs-lookup"><span data-stu-id="85b50-137">boolean</span></span>                                  | <span data-ttu-id="85b50-138">true 如果参与者位于会议厅</span><span class="sxs-lookup"><span data-stu-id="85b50-138">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="85b50-139">isMuted</span><span class="sxs-lookup"><span data-stu-id="85b50-139">isMuted</span></span>              | <span data-ttu-id="85b50-140">boolean</span><span class="sxs-lookup"><span data-stu-id="85b50-140">boolean</span></span>                                  | <span data-ttu-id="85b50-141">如果参与者处于静音状态，则 true （客户端或服务器静音）</span><span class="sxs-lookup"><span data-stu-id="85b50-141">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="85b50-142">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="85b50-142">mediaStreams</span></span>         | <span data-ttu-id="85b50-143">[mediaStream](mediastream.md)集合</span><span class="sxs-lookup"><span data-stu-id="85b50-143">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="85b50-144">媒体流的列表。</span><span class="sxs-lookup"><span data-stu-id="85b50-144">The list of media streams.</span></span>                                   |
| <span data-ttu-id="85b50-145">元数据</span><span class="sxs-lookup"><span data-stu-id="85b50-145">metadata</span></span>             | <span data-ttu-id="85b50-146">字符串</span><span class="sxs-lookup"><span data-stu-id="85b50-146">String</span></span>                                   | <span data-ttu-id="85b50-147">提供在名单中的参与者的数据的 blob</span><span class="sxs-lookup"><span data-stu-id="85b50-147">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="85b50-148">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="85b50-148">recordingInfo</span></span>        | [<span data-ttu-id="85b50-149">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="85b50-149">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="85b50-150">参与者是否具有录制功能的信息。</span><span class="sxs-lookup"><span data-stu-id="85b50-150">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="85b50-151">Relationships</span><span class="sxs-lookup"><span data-stu-id="85b50-151">Relationships</span></span>
<span data-ttu-id="85b50-152">无</span><span class="sxs-lookup"><span data-stu-id="85b50-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85b50-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85b50-153">JSON representation</span></span>

<span data-ttu-id="85b50-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85b50-154">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="85b50-155">示例</span><span class="sxs-lookup"><span data-stu-id="85b50-155">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
