---
title: audioRoutingGroup 资源类型
description: 音频路由组在多方对话中的参与者之间存储专用音频路由。 源是参与者本身, 而接收器是多方对话中的其他参与者的子集。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c5139b9f1f0c56b93848868c0d76ebf3051a148c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328249"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="83d43-104">audioRoutingGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="83d43-104">audioRoutingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83d43-105">音频路由组在多方对话中的参与者之间存储专用音频路由。</span><span class="sxs-lookup"><span data-stu-id="83d43-105">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="83d43-106">源是参与者本身, 而接收器是多方对话中的其他参与者的子集。</span><span class="sxs-lookup"><span data-stu-id="83d43-106">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="83d43-107">**注意:**[ConfigureMixer](../api/participant-configuremixer.md)不涉及任何路由, 而是用于设置源接收器组合的音量级别的整个调用。</span><span class="sxs-lookup"><span data-stu-id="83d43-107">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="83d43-108">方法</span><span class="sxs-lookup"><span data-stu-id="83d43-108">Methods</span></span>

| <span data-ttu-id="83d43-109">方法</span><span class="sxs-lookup"><span data-stu-id="83d43-109">Method</span></span>                                                  | <span data-ttu-id="83d43-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="83d43-110">Return Type</span></span>                               | <span data-ttu-id="83d43-111">说明</span><span class="sxs-lookup"><span data-stu-id="83d43-111">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="83d43-112">获取 audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="83d43-112">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="83d43-113">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="83d43-113">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="83d43-114">读取 audioRoutingGroup 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="83d43-114">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="83d43-115">更新</span><span class="sxs-lookup"><span data-stu-id="83d43-115">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="83d43-116">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="83d43-116">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="83d43-117">更新接收器列表。</span><span class="sxs-lookup"><span data-stu-id="83d43-117">Update receivers list.</span></span>                       |
| [<span data-ttu-id="83d43-118">删除</span><span class="sxs-lookup"><span data-stu-id="83d43-118">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="83d43-119">无</span><span class="sxs-lookup"><span data-stu-id="83d43-119">None</span></span>                                      | <span data-ttu-id="83d43-120">删除音频路由组。</span><span class="sxs-lookup"><span data-stu-id="83d43-120">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="83d43-121">属性</span><span class="sxs-lookup"><span data-stu-id="83d43-121">Properties</span></span>

| <span data-ttu-id="83d43-122">属性</span><span class="sxs-lookup"><span data-stu-id="83d43-122">Property</span></span>      | <span data-ttu-id="83d43-123">类型</span><span class="sxs-lookup"><span data-stu-id="83d43-123">Type</span></span>              | <span data-ttu-id="83d43-124">说明</span><span class="sxs-lookup"><span data-stu-id="83d43-124">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="83d43-125">id</span><span class="sxs-lookup"><span data-stu-id="83d43-125">id</span></span>            | <span data-ttu-id="83d43-126">string</span><span class="sxs-lookup"><span data-stu-id="83d43-126">string</span></span>            | <span data-ttu-id="83d43-127">只读。</span><span class="sxs-lookup"><span data-stu-id="83d43-127">Read-only.</span></span> <span data-ttu-id="83d43-128">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="83d43-128">Server generated.</span></span>                                         |
| <span data-ttu-id="83d43-129">接收器</span><span class="sxs-lookup"><span data-stu-id="83d43-129">receivers</span></span>     | <span data-ttu-id="83d43-130">collection(string)</span><span class="sxs-lookup"><span data-stu-id="83d43-130">collection(string)</span></span> | <span data-ttu-id="83d43-131">接收参与者 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="83d43-131">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="83d43-132">routingMode</span><span class="sxs-lookup"><span data-stu-id="83d43-132">routingMode</span></span>   | <span data-ttu-id="83d43-133">string</span><span class="sxs-lookup"><span data-stu-id="83d43-133">string</span></span>            | <span data-ttu-id="83d43-134">路由组模式。</span><span class="sxs-lookup"><span data-stu-id="83d43-134">Routing group mode.</span></span>  <span data-ttu-id="83d43-135">可取值为：`oneToOne`、`multicast`。</span><span class="sxs-lookup"><span data-stu-id="83d43-135">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="83d43-136">源</span><span class="sxs-lookup"><span data-stu-id="83d43-136">sources</span></span>       | <span data-ttu-id="83d43-137">collection(string)</span><span class="sxs-lookup"><span data-stu-id="83d43-137">collection(string)</span></span> | <span data-ttu-id="83d43-138">源参与者 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="83d43-138">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="83d43-139">**注意:** 路由模式确定对源和接收器的限制。</span><span class="sxs-lookup"><span data-stu-id="83d43-139">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="83d43-140">仅支持以下路由组。</span><span class="sxs-lookup"><span data-stu-id="83d43-140">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="83d43-141">`oneToOne`-源和接收器每个只有一个参与者。</span><span class="sxs-lookup"><span data-stu-id="83d43-141">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="83d43-142">`multicast`-源具有一个参与者, 但有多个接收器。</span><span class="sxs-lookup"><span data-stu-id="83d43-142">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="83d43-143">收件人列表可能会更新。</span><span class="sxs-lookup"><span data-stu-id="83d43-143">Receivers list may be updated.</span></span>

> <span data-ttu-id="83d43-144">**注意:** 如果创建了多个音频路由组 (例如, 每个参与者的 bot), 则仅转发前4个主扬声器的音频。</span><span class="sxs-lookup"><span data-stu-id="83d43-144">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="83d43-145">除了自定义的音频路由组, 如果扬声器在主混音器中的音量不足, 他/她也不会听到此扬声器和机器人的专用音频组, 即使在主混音器中没有太大的声音。</span><span class="sxs-lookup"><span data-stu-id="83d43-145">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="83d43-146">关系</span><span class="sxs-lookup"><span data-stu-id="83d43-146">Relationships</span></span>
<span data-ttu-id="83d43-147">无</span><span class="sxs-lookup"><span data-stu-id="83d43-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83d43-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83d43-148">JSON representation</span></span>

<span data-ttu-id="83d43-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83d43-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "string (identifier)",
  "receivers": [ "string" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "string" ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
