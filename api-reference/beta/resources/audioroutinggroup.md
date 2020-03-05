---
title: audioRoutingGroup 资源类型
description: 音频路由组在多方对话中的参与者之间存储专用音频路由。 源是参与者本身，而接收器是多方对话中的其他参与者的子集。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 44049ebaa431ac1c11e6581c82eab76a7406fb94
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508106"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="1f37e-104">audioRoutingGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f37e-104">audioRoutingGroup resource type</span></span>

<span data-ttu-id="1f37e-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1f37e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f37e-106">音频路由组在多方对话中的参与者之间存储专用音频路由。</span><span class="sxs-lookup"><span data-stu-id="1f37e-106">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="1f37e-107">源是参与者本身，而接收器是多方对话中的其他参与者的子集。</span><span class="sxs-lookup"><span data-stu-id="1f37e-107">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="1f37e-108">**注意：** [ConfigureMixer](../api/participant-configuremixer.md)不涉及任何路由，而是用于设置源接收器组合的音量级别的整个调用。</span><span class="sxs-lookup"><span data-stu-id="1f37e-108">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="1f37e-109">方法</span><span class="sxs-lookup"><span data-stu-id="1f37e-109">Methods</span></span>

| <span data-ttu-id="1f37e-110">方法</span><span class="sxs-lookup"><span data-stu-id="1f37e-110">Method</span></span>                                                  | <span data-ttu-id="1f37e-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="1f37e-111">Return Type</span></span>                               | <span data-ttu-id="1f37e-112">说明</span><span class="sxs-lookup"><span data-stu-id="1f37e-112">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="1f37e-113">获取 audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="1f37e-113">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="1f37e-114">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="1f37e-114">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="1f37e-115">读取 audioRoutingGroup 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1f37e-115">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="1f37e-116">更新</span><span class="sxs-lookup"><span data-stu-id="1f37e-116">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="1f37e-117">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="1f37e-117">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="1f37e-118">更新接收器列表。</span><span class="sxs-lookup"><span data-stu-id="1f37e-118">Update receivers list.</span></span>                       |
| [<span data-ttu-id="1f37e-119">删除</span><span class="sxs-lookup"><span data-stu-id="1f37e-119">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="1f37e-120">无</span><span class="sxs-lookup"><span data-stu-id="1f37e-120">None</span></span>                                      | <span data-ttu-id="1f37e-121">删除音频路由组。</span><span class="sxs-lookup"><span data-stu-id="1f37e-121">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="1f37e-122">属性</span><span class="sxs-lookup"><span data-stu-id="1f37e-122">Properties</span></span>

| <span data-ttu-id="1f37e-123">属性</span><span class="sxs-lookup"><span data-stu-id="1f37e-123">Property</span></span>      | <span data-ttu-id="1f37e-124">类型</span><span class="sxs-lookup"><span data-stu-id="1f37e-124">Type</span></span>              | <span data-ttu-id="1f37e-125">说明</span><span class="sxs-lookup"><span data-stu-id="1f37e-125">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="1f37e-126">id</span><span class="sxs-lookup"><span data-stu-id="1f37e-126">id</span></span>            | <span data-ttu-id="1f37e-127">string</span><span class="sxs-lookup"><span data-stu-id="1f37e-127">string</span></span>            | <span data-ttu-id="1f37e-128">只读。</span><span class="sxs-lookup"><span data-stu-id="1f37e-128">Read-only.</span></span>                                                           |
| <span data-ttu-id="1f37e-129">接收器</span><span class="sxs-lookup"><span data-stu-id="1f37e-129">receivers</span></span>     | <span data-ttu-id="1f37e-130">collection(string)</span><span class="sxs-lookup"><span data-stu-id="1f37e-130">collection(string)</span></span> | <span data-ttu-id="1f37e-131">接收参与者 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="1f37e-131">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="1f37e-132">routingMode</span><span class="sxs-lookup"><span data-stu-id="1f37e-132">routingMode</span></span>   | <span data-ttu-id="1f37e-133">string</span><span class="sxs-lookup"><span data-stu-id="1f37e-133">string</span></span>            | <span data-ttu-id="1f37e-134">路由组模式。</span><span class="sxs-lookup"><span data-stu-id="1f37e-134">Routing group mode.</span></span>  <span data-ttu-id="1f37e-135">可取值为：`oneToOne`、`multicast`。</span><span class="sxs-lookup"><span data-stu-id="1f37e-135">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="1f37e-136">源</span><span class="sxs-lookup"><span data-stu-id="1f37e-136">sources</span></span>       | <span data-ttu-id="1f37e-137">collection(string)</span><span class="sxs-lookup"><span data-stu-id="1f37e-137">collection(string)</span></span> | <span data-ttu-id="1f37e-138">源参与者 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="1f37e-138">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="1f37e-139">**注意：** 路由模式确定对源和接收器的限制。</span><span class="sxs-lookup"><span data-stu-id="1f37e-139">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="1f37e-140">仅支持以下路由组。</span><span class="sxs-lookup"><span data-stu-id="1f37e-140">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="1f37e-141">`oneToOne`-源和接收器每个只有一个参与者。</span><span class="sxs-lookup"><span data-stu-id="1f37e-141">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="1f37e-142">`multicast`-源具有一个参与者，但有多个接收器。</span><span class="sxs-lookup"><span data-stu-id="1f37e-142">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="1f37e-143">收件人列表可能会更新。</span><span class="sxs-lookup"><span data-stu-id="1f37e-143">Receivers list may be updated.</span></span>

> <span data-ttu-id="1f37e-144">**注意：** 如果创建了多个音频路由组（例如，每个参与者的 bot），则仅转发前4个主扬声器的音频。</span><span class="sxs-lookup"><span data-stu-id="1f37e-144">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="1f37e-145">除了自定义的音频路由组，如果扬声器在主混音器中的音量不足，他/她也不会听到此扬声器和机器人的专用音频组，即使在主混音器中没有太大的声音。</span><span class="sxs-lookup"><span data-stu-id="1f37e-145">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="1f37e-146">关系</span><span class="sxs-lookup"><span data-stu-id="1f37e-146">Relationships</span></span>
<span data-ttu-id="1f37e-147">无</span><span class="sxs-lookup"><span data-stu-id="1f37e-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f37e-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f37e-148">JSON representation</span></span>

<span data-ttu-id="1f37e-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f37e-149">The following is a JSON representation of the resource.</span></span>

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
